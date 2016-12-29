# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7442a89219ecf395166028a0b51fa9675d6cc6a1](https://github.com/JuliaLang/julia/commit/7442a89219ecf395166028a0b51fa9675d6cc6a1) vs [JuliaLang/julia@b561cfbfbd2b845cb05e8263a86e22dd665fe723](https://github.com/JuliaLang/julia/commit/b561cfbfbd2b845cb05e8263a86e22dd665fe723)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19746#issuecomment-269627949)

*Tag Predicate:* `"linalg"`

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

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1751
Commit 7442a89 (2016-12-29 13:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5850.0859375 MB free)
Uptime: 1.8666151e7 sec
Load Avg:  0.9169921875  0.958984375  0.91064453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25484466 s          0 s    6017709 s  1829774236 s         59 s
#2  3501 MHz   81052370 s          0 s    3665867 s  1780784211 s          8 s
#3  3501 MHz   24635790 s          0 s    3170648 s  1837949202 s         39 s
#4  3501 MHz   22218093 s          0 s    3264048 s  1840253052 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1748
Commit b561cfb (2016-12-29 09:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5724.44921875 MB free)
Uptime: 1.8669884e7 sec
Load Avg:  1.00341796875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25626384 s          0 s    6028591 s  1829993951 s         59 s
#2  3501 MHz   81179835 s          0 s    3673635 s  1781021840 s          8 s
#3  3501 MHz   24676272 s          0 s    3176786 s  1838275103 s         39 s
#4  3501 MHz   22251028 s          0 s    3269801 s  1840587021 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
