# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9e1a4b62616536048c5b1ebfb8213709d50877b9](https://github.com/JuliaLang/julia/commit/9e1a4b62616536048c5b1ebfb8213709d50877b9) vs [JuliaLang/julia@44d76771999d6a8ac23ee09d37f4a5f812010844](https://github.com/JuliaLang/julia/commit/44d76771999d6a8ac23ee09d37f4a5f812010844)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19678#issuecomment-269009605)

*Tag Predicate:* `ALL`

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
| `["array","cat",("catnd",500)]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","6d"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","index","7d"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array","index","sub2ind"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","Int")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 3.51 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 0.21 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Complex{Float64}")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 0.17 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float64")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int64")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 0.21 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 0.06 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 0.71 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.38 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","sparse"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1674
Commit 9e1a4b6 (2016-12-23 05:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8742.875 MB free)
Uptime: 1.8160953e7 sec
Load Avg:  1.0107421875  1.0537109375  1.00830078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   24349259 s          0 s    5804726 s  1780743870 s         56 s
#2  3501 MHz   75914510 s          0 s    3529684 s  1735568323 s          8 s
#3  3501 MHz   23607054 s          0 s    3055562 s  1788595473 s         36 s
#4  3501 MHz   20867085 s          0 s    3115188 s  1791261478 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1671
Commit 44d7677 (2016-12-23 05:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9132.4765625 MB free)
Uptime: 1.8167279e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   24420221 s          0 s    5813166 s  1781294952 s         56 s
#2  3501 MHz   76294726 s          0 s    3536935 s  1735812902 s          8 s
#3  3501 MHz   23641451 s          0 s    3061626 s  1789186784 s         37 s
#4  3501 MHz   20983346 s          0 s    3124910 s  1791767649 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
