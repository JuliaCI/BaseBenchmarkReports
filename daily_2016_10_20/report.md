# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0faf8ce200103839577171d28a4d1545fa827336](https://github.com/JuliaLang/julia/commit/0faf8ce200103839577171d28a4d1545fa827336)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/0faf8ce200103839577171d28a4d1545fa827336#commitcomment-19496490)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-10-20 vs 2016-10-19

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
| `["array","growth",("append!",256)]` | 0.99 (15%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.51 (45%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","Array")]` | 100.25 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","NullableArray")]` | 203.50 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","BigFloat")]` | 0.25 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","BigInt")]` | 0.26 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","BigFloat")]` | 0.46 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","BigInt")]` | 0.45 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 4.14 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 4.12 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 4.43 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 5.81 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 4.60 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Bool")]` | 5.10 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Complex{Float64}")]` | 5.10 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float32")]` | 5.10 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float64")]` | 5.05 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int64")]` | 5.10 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int8")]` | 5.10 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","BigInt")]` | 0.90 (45%)  | 0.99 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","NullableArray","BigInt")]` | 0.91 (45%)  | 0.99 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float32")]` | 6.67 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float64")]` | 3.58 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int64")]` | 4.20 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int8")]` | 26.15 (45%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1045
Commit 0faf8ce (2016-10-19 16:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14484.48046875 MB free)
Uptime: 1.2586939e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   19892954 s          0 s    4274051 s  1230952337 s         38 s
#2  3501 MHz   56731444 s          0 s    2713790 s  1198445648 s          5 s
#3  3501 MHz   19030498 s          0 s    2370681 s  1236686509 s         27 s
#4  3501 MHz   16587430 s          0 s    2389668 s  1239093657 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
