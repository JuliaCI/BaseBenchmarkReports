# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@533393661d276fe5cf648ad6a482f0ff5b0ef5ad](https://github.com/JuliaLang/julia/commit/533393661d276fe5cf648ad6a482f0ff5b0ef5ad) vs [JuliaLang/julia@d3bac6e33ff8bb9fe39bd4945fcce45af665c272](https://github.com/JuliaLang/julia/commit/d3bac6e33ff8bb9fe39bd4945fcce45af665c272)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20165#issuecomment-274214587)

*Tag Predicate:* `"sparse"`

## Results

*Note: If Chrome is your browser, I strongly recommend installing the [Wide GitHub](https://chrome.google.com/webstore/detail/wide-github/kaalofacklcidaampbokdplbklpeldpj?hl=en)
extension, which makes the result table easier to read.*

Below is a table of this job's results, obtained by running the benchmarks found in
[JuliaCI/BaseBenchmarks.jl](https://github.com/JuliaCI/BaseBenchmarks.jl). The values
listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`,
and can be used to index into the BaseBenchmarks suite to retrieve the corresponding
benchmarks.

The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.

A ratio greater than `1.0` denotes a possible regression (marked with :x:), while a ratio less
than `1.0` denotes a possible improvement (marked with :white_check_mark:). Only significant results - results
that indicate possible regressions or improvements - are shown below (thus, an empty table means that all
benchmark results remained invariant between builds).

| ID | time ratio | memory ratio |
|----|------------|--------------|

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["broadcast","sparse"]`
- `["problem","fem"]`
- `["problem","laplacian"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.2239
Commit 5333936 (2017-01-21 00:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19464.71875 MB free)
Uptime: 2.0607559e7 sec
Load Avg:  0.9970703125  0.9560546875  0.91357421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   39000556 s          0 s    6069319 s  2011485847 s         62 s
#2  3501 MHz  131468379 s          0 s    7139415 s  1918708872 s         21 s
#3  3501 MHz   34460022 s          0 s    4173884 s  2021149878 s         36 s
#4  3501 MHz   30283548 s          0 s    4084600 s  2025607186 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2237
Commit d3bac6e (2017-01-21 00:15 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19538.06640625 MB free)
Uptime: 2.0611275e7 sec
Load Avg:  1.0029296875  0.97216796875  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   39112692 s          0 s    6078359 s  2011735427 s         62 s
#2  3501 MHz  131558460 s          0 s    7146774 s  1918982231 s         21 s
#3  3501 MHz   34534138 s          0 s    4182058 s  2021438301 s         36 s
#4  3501 MHz   30345621 s          0 s    4091764 s  2025908903 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
