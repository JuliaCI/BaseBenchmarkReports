# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1f370d48ac71c28dda97ece5dd41d4d67ea11913](https://github.com/JuliaLang/julia/commit/1f370d48ac71c28dda97ece5dd41d4d67ea11913) vs [JuliaLang/julia@aecf426ab30a068be75b01e9466fe8ee4b9ca8be](https://github.com/JuliaLang/julia/commit/aecf426ab30a068be75b01e9466fe8ee4b9ca8be)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22752#issuecomment-322291031)

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
| `["problem","monte carlo","euro_option_devec"]` | 14.67 (15%) :x: | 2236.05 (1%) :x: |
| `["problem","monte carlo","euro_option_vec"]` | 18.21 (15%) :x: | 492.04 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:2^10000)")]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand!","ImplicitRNG","Float64")]` | 2.23 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand!","ImplicitRNG","Int64")]` | 2.48 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random","types",("randn!","ImplicitRNG","Float64")]` | 34.39 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn!","MersenneTwister","Complex{Float16}")]` | 3.54 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn!","MersenneTwister","Complex{Float32}")]` | 19.71 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn!","MersenneTwister","Complex{Float64}")]` | 44.36 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn!","MersenneTwister","Float16")]` | 5.39 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn!","MersenneTwister","Float32")]` | 16.15 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn!","MersenneTwister","Float64")]` | 34.74 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn!","RandomDevice","Float64")]` | 17.47 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn","ImplicitRNG","Float64")]` | 4.06 (25%) :x: | 2.00 (1%) :x: |
| `["random","types",("randn","ImplicitRNG","ImplicitFloat64")]` | 1.70 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn","MersenneTwister","Complex{Float16}")]` | 2.12 (25%) :x: | 8.00 (1%) :x: |
| `["random","types",("randn","MersenneTwister","Complex{Float32}")]` | 4.21 (25%) :x: | 8.00 (1%) :x: |
| `["random","types",("randn","MersenneTwister","Complex{Float64}")]` | 5.01 (25%) :x: | 5.00 (1%) :x: |
| `["random","types",("randn","MersenneTwister","Float16")]` | 1.58 (25%) :x: | 2.00 (1%) :x: |
| `["random","types",("randn","MersenneTwister","Float32")]` | 2.19 (25%) :x: | 2.00 (1%) :x: |
| `["random","types",("randn","MersenneTwister","Float64")]` | 5.17 (25%) :x: | 2.00 (1%) :x: |
| `["random","types",("randn","MersenneTwister","ImplicitFloat64")]` | 1.95 (25%) :x: | Inf (1%) :x: |
| `["random","types",("randn","RandomDevice","Float64")]` | 3.61 (25%) :x: | 2.00 (1%) :x: |
| `["random","types",("randn","RandomDevice","ImplicitFloat64")]` | 1.52 (25%) :x: | Inf (1%) :x: |

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
Julia Version 0.7.0-DEV.1350
Commit 1f370d4 (2017-08-14 19:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   80033213 s          0 s   12330049 s  3738066765 s        134 s
       #2  3501 MHz  319961805 s          0 s   13435847 s  3498560563 s         49 s
       #3  3501 MHz   68219092 s          0 s    7799730 s  3761135587 s         66 s
       #4  3501 MHz   63550892 s          0 s    7738462 s  3766217483 s         22 s
       
  Memory: 31.383651733398438 GB (3260.328125 MB free)
  Uptime: 3.8388376e7 sec
  Load Avg:  1.0029296875  1.11279296875  1.4443359375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1344
Commit aecf426 (2017-08-14 19:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   80129030 s          0 s   12337710 s  3738154333 s        135 s
       #2  3501 MHz  320089960 s          0 s   13446631 s  3498613026 s         49 s
       #3  3501 MHz   68302468 s          0 s    7806785 s  3761236432 s         66 s
       #4  3501 MHz   63627262 s          0 s    7745821 s  3766325056 s         22 s
       
  Memory: 31.383651733398438 GB (3180.73046875 MB free)
  Uptime: 3.8390295e7 sec
  Load Avg:  1.0458984375  1.1708984375  1.6787109375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
