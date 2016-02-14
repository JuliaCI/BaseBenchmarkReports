# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@18e8de7](https://github.com/JuliaLang/julia/commit/18e8de79444be19bf91a699d2047df5cadb484d4) vs [JuliaLang/julia@8ffca32](https://github.com/JuliaLang/julia/commit/8ffca32a9b1623ae92d8f448e724b445095aa358)

*Tag Predicate:* `"array"`

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15071)

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
| `lapack qr` | `(:qrfact,4)` | **0.72** :white_check_mark: | 1.0 | 1.0 | 1.0 |
| `lapack schur` | `(:schurfact,16)` | **0.67** :white_check_mark: | 1.0 | 1.0 | 1.0 |
| `simd` | `(:conditional_loop!,"Int64",999)` | **0.77** :white_check_mark: | 1.0 | 1.0 | 1.0 |
| `simd` | `(:two_reductions,"Int32",255)` | **1.86** :x: | 1.0 | 1.0 | 1.0 |
| `sparse matrix row indexing` | `("dense logical",100,992,99)` | **0.48** :white_check_mark: | Inf | 1.0 | 1.0 |

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+2666
Commit 18e8de7 (2016-02-14 05:49 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.3 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (22934.84375 MB free)
Uptime: 1.1803244e7 sec
Load Avg:  3.32470703125  5.82568359375  6.0107421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9356801 s        786 s    5591294 s  1161083151 s          5 s
#2  3501 MHz    8585584 s        245 s    3487379 s  1166765433 s          1 s
#3  3501 MHz    8142195 s       1144 s    3657820 s  1167434969 s          1 s
#4  3501 MHz    7626446 s        303 s    3390373 s  1168456210 s          2 s
#5  3501 MHz    6422543 s       3339 s    3200689 s  1170432949 s          0 s
#6  3501 MHz    6419913 s        966 s    2979247 s  1170672799 s          0 s
#7  3501 MHz    6410488 s       2155 s    3191997 s  1170427478 s          0 s
#8  3501 MHz    6107931 s       1284 s    3175093 s  1170824707 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1

```

#### Comparison Build

```
Julia Version 0.5.0-dev+2663
Commit 8ffca32 (2016-02-14 05:38 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.3 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (23081.046875 MB free)
Uptime: 1.1806238e7 sec
Load Avg:  3.20458984375  5.6396484375  6.02978515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9424001 s        786 s    5664626 s  1161225434 s          5 s
#2  3501 MHz    8675571 s        245 s    3554118 s  1166883378 s          1 s
#3  3501 MHz    8247888 s       1144 s    3704689 s  1167561820 s          1 s
#4  3501 MHz    7732726 s        303 s    3443342 s  1168574502 s          2 s
#5  3501 MHz    6489034 s       3339 s    3273772 s  1170581161 s          0 s
#6  3501 MHz    6484324 s        966 s    3052610 s  1170824385 s          0 s
#7  3501 MHz    6475431 s       2155 s    3265140 s  1170575842 s          0 s
#8  3501 MHz    6193077 s       1284 s    3239234 s  1170964247 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1

```

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `array bool`
- `array cat`
- `array comprehension`
- `array growth`
- `array index load reverse`
- `array index setindex!`
- `array index sum`
- `array subarray`
- `blas 1`
- `blas 2`
- `blas 3`
- `lapack chol`
- `lapack eig`
- `lapack lu`
- `lapack qr`
- `lapack schur`
- `lapack svd`
- `problem laplacian`
- `simd`
- `sparse matrix column indexing`
- `sparse matrix row + column indexing`
- `sparse matrix row indexing`
- `sparse matrix transpose`
- `sparse vector indexing`
