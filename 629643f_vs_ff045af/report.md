# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@629643f165cf63929701494874f8833f1be6ffaf](https://github.com/JuliaLang/julia/commit/629643f165cf63929701494874f8833f1be6ffaf) vs [JuliaLang/julia@ff045afdfd448a28b43b764c4d67e6ef3ed42ed0](https://github.com/JuliaLang/julia/commit/ff045afdfd448a28b43b764c4d67e6ef3ed42ed0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24989#issuecomment-350492097)

*Tag Predicate:* `"random"`

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

- `["problem", "monte carlo"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2814
Commit 629643f (2017-12-09 17:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  107108962 s          0 s   18904202 s  4708766379 s         99 s
       #2  3501 MHz  457462221 s          0 s   12076304 s  4376562489 s         23 s
       #3  3501 MHz   90205482 s          0 s   10318041 s  4746057542 s         82 s
       #4  3501 MHz   86291634 s          0 s   10504716 s  4749779273 s         21 s
       
  Memory: 31.383651733398438 GB (4735.88671875 MB free)
  Uptime: 4.8489022e7 sec
  Load Avg:  0.9228515625  1.2060546875  1.57861328125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2812
Commit ff045af (2017-12-09 16:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  107197868 s          0 s   18911692 s  4708854981 s         99 s
       #2  3501 MHz  457585870 s          0 s   12085118 s  4376615077 s         23 s
       #3  3501 MHz   90303459 s          0 s   10325845 s  4746136692 s         82 s
       #4  3501 MHz   86373415 s          0 s   10512245 s  4749875061 s         21 s
       
  Memory: 31.383651733398438 GB (4499.625 MB free)
  Uptime: 4.8490878e7 sec
  Load Avg:  0.9228515625  1.240234375  1.826171875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
