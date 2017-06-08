# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d06ec8ebc56f6befb151009e00d1c542d308eb53](https://github.com/JuliaLang/julia/commit/d06ec8ebc56f6befb151009e00d1c542d308eb53) vs [JuliaLang/julia@7495f445feebb1ccb835832ce2d16b3e66e685ed](https://github.com/JuliaLang/julia/commit/7495f445feebb1ccb835832ce2d16b3e66e685ed)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22293)

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
| `["array","bool","boolarray_true_load!"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","NullableArray")]` | 4.95 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 4.44 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 6.02 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Complex{Float64}")]` | 2.09 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 2.30 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 3.34 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Bool")]` | 10.61 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Complex{Float64}")]` | 4.85 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float32")]` | 4.48 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float64")]` | 4.95 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int64")]` | 4.45 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int8")]` | 4.90 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 2.86 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Complex{Float64}")]` | 3.41 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float32")]` | 2.33 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float64")]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int64")]` | 4.00 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int8")]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 2.79 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",100)]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.91 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",1000)]` | 3.18 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",10000)]` | 2.01 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",100000)]` | 2.02 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
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
- `["scalar","intfuncs"]`
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
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.502
Commit d06ec8e (2017-06-08 16:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68497692 s          0 s   10517677 s  3173143500 s         92 s
       #2  3501 MHz  268182076 s          0 s   11536985 s  2973506526 s         38 s
       #3  3501 MHz   58771372 s          0 s    6825440 s  3192076339 s         49 s
       #4  3501 MHz   54291663 s          0 s    6762562 s  3196925708 s         17 s
       
  Memory: 31.383651733398438 GB (2737.9375 MB free)
  Uptime: 3.2591517e7 sec
  Load Avg:  1.01025390625  1.01904296875  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.500
Commit 7495f44 (2017-06-08 05:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68581971 s          0 s   10527720 s  3173580907 s         92 s
       #2  3501 MHz  268658116 s          0 s   11545941 s  2973554546 s         38 s
       #3  3501 MHz   58868477 s          0 s    6834126 s  3192503516 s         49 s
       #4  3501 MHz   54377807 s          0 s    6770959 s  3197364433 s         17 s
       
  Memory: 31.383651733398438 GB (2748.3984375 MB free)
  Uptime: 3.2596854e7 sec
  Load Avg:  1.0029296875  1.015625  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
