# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e77a9e88bd3731bd3c8858bb9ba1ccc524340a2b](https://github.com/JuliaLang/julia/commit/e77a9e88bd3731bd3c8858bb9ba1ccc524340a2b) vs [JuliaLang/julia@493311b8b9371742ae4ec8b7021be932f0369e0d](https://github.com/JuliaLang/julia/commit/493311b8b9371742ae4ec8b7021be932f0369e0d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21888#issuecomment-308288523)

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
| `["array","bool","boolarray_bool_load!"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array","bool","boolarray_true_load!"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",8)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","reductions",("mean","Int64")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_slow!"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",10)]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 1.72 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","Date")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["misc","afoldl","Float64"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.65 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{BigInt}(1)")]` | 1.66 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigInt}()")]` | 1.72 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 1.81 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.71 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.71 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 1.71 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 1.71 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 1.71 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigFloat}()")]` | 1.98 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.99 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigInt}()")]` | 1.98 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigInt}(1)")]` | 1.98 (60%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 1.58 (40%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 1.66 (40%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",100)]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",1000)]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(4,4),(4,4))]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.595
Commit e77a9e8 (2017-06-14 00:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68931295 s          0 s   10623213 s  3218634995 s         92 s
       #2  3501 MHz  270214578 s          0 s   11648572 s  3017418008 s         38 s
       #3  3501 MHz   59213380 s          0 s    6886851 s  3237685201 s         49 s
       #4  3501 MHz   54717884 s          0 s    6815630 s  3242564292 s         17 s
       
  Memory: 31.383651733398438 GB (2302.50390625 MB free)
  Uptime: 3.3052813e7 sec
  Load Avg:  1.0458984375  1.02783203125  1.04736328125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.584
Commit 493311b (2017-06-13 21:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   69029535 s          0 s   10633100 s  3219059571 s         92 s
       #2  3501 MHz  270691975 s          0 s   11657447 s  3017465853 s         38 s
       #3  3501 MHz   59301188 s          0 s    6895439 s  3238122691 s         49 s
       #4  3501 MHz   54801102 s          0 s    6824096 s  3243006697 s         17 s
       
  Memory: 31.383651733398438 GB (2591.6953125 MB free)
  Uptime: 3.3058161e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
