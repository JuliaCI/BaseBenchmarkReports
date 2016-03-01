# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5e15cc3](https://github.com/JuliaLang/julia/commit/5e15cc3850b133be0247c8c56f9723e460cb6dd4) vs [JuliaLang/julia@0b6cab6](https://github.com/JuliaLang/julia/commit/0b6cab6104477be92377e77348cb710b3a118fec)

*Tag Predicate:* `"tuple"`

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15312#issuecomment-190934162)

## Results

Below is a table of this job's results. If available, the data used to generate this
table can be found in the JSON file in this directory.

Benchmark definitions can be found in [JuliaCI/BaseBenchmarks.jl](https://github.com/JuliaCI/BaseBenchmarks.jl).

The ratio values in the below table equal `primary_result / comparison_result` for each corresponding
metric. Thus, `x < 1.0` would denote an improvement, while `x > 1.0` would denote a regression.
Note that a default tolerance of `0.2` is applied to account for the variance of our test
hardware.

Regressions are marked with :x:, while improvements are marked with :white_check_mark:. GC
measurements are [not considered when determining regression status](https://github.com/JuliaCI/BenchmarkTrackers.jl/issues/5).

Only benchmarks with significant results - results that indicate regressions or improvements - are
shown below (an empty table means that all benchmark results remained invariant between builds).

| Group ID | Benchmark ID | time | time spent in GC | bytes allocated | number of allocations |
|----------|--------------|------|------------------|-----------------|-----------------------|

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+2961
Commit 5e15cc3 (2016-03-01 20:21 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (19989.0859375 MB free)
Uptime: 1.3244339e7 sec
Load Avg:  1.39794921875  3.42431640625  5.81396484375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5624798 s        530 s    2187358 s  1314351258 s         13 s
#2  3501 MHz    4934580 s        116 s    2028753 s  1315281058 s          1 s
#3  3501 MHz    4018329 s       1297 s    1688574 s  1317255516 s          2 s
#4  3501 MHz    3077883 s        318 s    1724017 s  1318233801 s          0 s
#5  3501 MHz    2154580 s       3907 s     735953 s  1321258817 s          0 s
#6  3501 MHz    1780866 s        739 s     742685 s  1320336830 s          0 s
#7  3501 MHz    2281819 s       1062 s     780571 s  1321024531 s          0 s
#8  3501 MHz    2074414 s       2720 s     648331 s  1321447451 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1

```

#### Comparison Build

```
Julia Version 0.5.0-dev+2959
Commit 0b6cab6 (2016-03-01 17:48 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (19957.390625 MB free)
Uptime: 1.324628e7 sec
Load Avg:  1.60986328125  3.53515625  6.81884765625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5683917 s        530 s    2196034 s  1314459283 s         13 s
#2  3501 MHz    5018487 s        116 s    2036290 s  1315360184 s          1 s
#3  3501 MHz    4079878 s       1297 s    1696338 s  1317355716 s          2 s
#4  3501 MHz    3138954 s        318 s    1730939 s  1318339302 s          0 s
#5  3501 MHz    2212417 s       3907 s     743415 s  1321376277 s          0 s
#6  3501 MHz    1840661 s        739 s     749727 s  1320454345 s          0 s
#7  3501 MHz    2339696 s       1062 s     787010 s  1321144709 s          0 s
#8  3501 MHz    2132264 s       2720 s     655278 s  1321566124 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1

```

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

