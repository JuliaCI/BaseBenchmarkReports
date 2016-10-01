# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3398c7e6cc8ab470496192b0f1c350073cace11a](https://github.com/JuliaLang/julia/commit/3398c7e6cc8ab470496192b0f1c350073cace11a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3398c7e6cc8ab470496192b0f1c350073cace11a#commitcomment-19251664)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-10-01 vs 2016-09-30

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
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","BigInt")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Float32")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Float64")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.844
Commit 3398c7e (2016-10-01 00:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16956.20703125 MB free)
Uptime: 1.0944282e7 sec
Load Avg:  1.0078125  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17739002 s          0 s    3001279 s  1071386343 s         34 s
#2  3501 MHz   44353154 s          0 s    3230081 s  1045304780 s         10 s
#3  3501 MHz   15407203 s          0 s    1978551 s  1076508398 s         17 s
#4  3501 MHz   13034944 s          0 s    1933070 s  1079022735 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
