# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f62ec6cf807b3909bff3fbcdad9fea6835f3d704](https://github.com/JuliaLang/julia/commit/f62ec6cf807b3909bff3fbcdad9fea6835f3d704) vs [JuliaLang/julia@4d44668a7ebd0eb118c0328cd9eb39c844ac19cf](https://github.com/JuliaLang/julia/commit/4d44668a7ebd0eb118c0328cd9eb39c844ac19cf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19745#issuecomment-269575588)

*Tag Predicate:* `"broadcast"`

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

- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","sparse"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1743
Commit f62ec6c (2016-12-29 01:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6843.1484375 MB free)
Uptime: 1.8629776e7 sec
Load Avg:  1.01171875  0.92724609375  0.8916015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   30547060 s          0 s    4962051 s  1823695454 s         55 s
#2  3501 MHz   92116832 s          0 s    6005824 s  1761760663 s         20 s
#3  3501 MHz   26171119 s          0 s    3338880 s  1832615316 s         30 s
#4  3501 MHz   22263304 s          0 s    3251959 s  1836765098 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1741
Commit 4d44668 (2016-12-29 01:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6812.6328125 MB free)
Uptime: 1.863302e7 sec
Load Avg:  0.9619140625  0.9716796875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   30583074 s          0 s    4968493 s  1823976567 s         55 s
#2  3501 MHz   92172854 s          0 s    6013028 s  1762021001 s         20 s
#3  3501 MHz   26305398 s          0 s    3348652 s  1832794955 s         30 s
#4  3501 MHz   22331205 s          0 s    3258755 s  1837014143 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
