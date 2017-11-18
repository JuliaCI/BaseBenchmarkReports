# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4d94acf5510e06f66376c8111120aa3783064421](https://github.com/JuliaLang/julia/commit/4d94acf5510e06f66376c8111120aa3783064421) vs [JuliaLang/julia@cf2ed6628afb38f64738d77f6214dc368c5ef943](https://github.com/JuliaLang/julia/commit/cf2ed6628afb38f64738d77f6214dc368c5ef943)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24519#issuecomment-345406200)

*Tag Predicate:* `"linalg" && "arithmetic"`

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

- `["linalg", "arithmetic"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.2-pre.48
Commit 4d94acf (2017-11-17 20:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10701.4453125 MB free)
Uptime: 4.6615723e7 sec
Load Avg:  0.9228515625  1.22265625  1.60205078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   94287142 s          0 s   14594044 s  4542287539 s        210 s
#2  3501 MHz  378528676 s          0 s   15926905 s  4258840050 s         73 s
#3  3501 MHz   77809773 s          0 s    8845073 s  4572995366 s         94 s
#4  3501 MHz   72990752 s          0 s    8722090 s  4578355725 s         40 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.2-pre.3
Commit cf2ed66 (2017-11-14 19:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10670.171875 MB free)
Uptime: 4.6617601e7 sec
Load Avg:  1.0029296875  1.24951171875  1.810546875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   94371202 s          0 s   14602673 s  4542381752 s        210 s
#2  3501 MHz  378657306 s          0 s   15935522 s  4258889842 s         73 s
#3  3501 MHz   77897420 s          0 s    8853684 s  4573086178 s         94 s
#4  3501 MHz   73090379 s          0 s    8730688 s  4578434649 s         40 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
