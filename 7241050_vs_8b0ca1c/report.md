# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7241050320b448cd0d0c6f5425fcd80af79b6397](https://github.com/JuliaLang/julia/commit/7241050320b448cd0d0c6f5425fcd80af79b6397) vs [JuliaLang/julia@8b0ca1ca69c742976c038f6444828dbb916a30d0](https://github.com/JuliaLang/julia/commit/8b0ca1ca69c742976c038f6444828dbb916a30d0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20213#issuecomment-275026028)

*Tag Predicate:* `"dates"`

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

- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.2348
Commit 7241050 (2017-01-25 05:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20228.2421875 MB free)
Uptime: 2.097315e7 sec
Load Avg:  0.9638671875  0.91650390625  0.8837890625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33372871 s          0 s    7216718 s  2050722093 s         63 s
#2  3501 MHz  115108376 s          0 s    4469491 s  1976493643 s          8 s
#3  3501 MHz   31048027 s          0 s    3891072 s  2061377741 s         45 s
#4  3501 MHz   29030214 s          0 s    4021375 s  2063263382 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2344
Commit 8b0ca1c (2017-01-25 05:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20079.53515625 MB free)
Uptime: 2.0976773e7 sec
Load Avg:  0.9169921875  0.923828125  0.91259765625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33422649 s          0 s    7224369 s  2051026043 s         63 s
#2  3501 MHz  115165618 s          0 s    4475821 s  1976791919 s          8 s
#3  3501 MHz   31172308 s          0 s    3900117 s  2061606000 s         45 s
#4  3501 MHz   29129842 s          0 s    4029954 s  2063516929 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
