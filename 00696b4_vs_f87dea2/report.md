# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@00696b4ee4cfec73c16a530eb55e4462de091ac9](https://github.com/JuliaLang/julia/commit/00696b4ee4cfec73c16a530eb55e4462de091ac9) vs [JuliaLang/julia@f87dea2d0075596a3548db1451db3594fdcd9422](https://github.com/JuliaLang/julia/commit/f87dea2d0075596a3548db1451db3594fdcd9422)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23205#issuecomment-321651829)

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

- `["problem","monte carlo"]`
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1320
Commit 00696b4 (2017-08-10 19:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84319792 s          0 s   15165785 s  3693594482 s         87 s
       #2  3501 MHz  349913418 s          0 s    9603276 s  3442458817 s         13 s
       #3  3501 MHz   73536548 s          0 s    8457717 s  3720371191 s         73 s
       #4  3501 MHz   70251507 s          0 s    8645894 s  3723456851 s         17 s
       
  Memory: 31.383651733398438 GB (3682.11328125 MB free)
  Uptime: 3.8041945e7 sec
  Load Avg:  0.9326171875  1.1201171875  1.44580078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1318
Commit f87dea2 (2017-08-10 17:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84396921 s          0 s   15173251 s  3693704476 s         87 s
       #2  3501 MHz  350044793 s          0 s    9613757 s  3442511862 s         13 s
       #3  3501 MHz   73631577 s          0 s    8464750 s  3720463957 s         73 s
       #4  3501 MHz   70332883 s          0 s    8652896 s  3723563436 s         17 s
       
  Memory: 31.383651733398438 GB (3587.56640625 MB free)
  Uptime: 3.8043899e7 sec
  Load Avg:  0.9970703125  1.12353515625  1.623046875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
