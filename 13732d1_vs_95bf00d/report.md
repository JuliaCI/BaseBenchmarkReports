# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@13732d19d7ebc5e3d0ea186aaff280a72849f1af](https://github.com/JuliaLang/julia/commit/13732d19d7ebc5e3d0ea186aaff280a72849f1af) vs [JuliaLang/julia@95bf00d61f4ef06f72ac6f8c18baf269f56f5bc4](https://github.com/JuliaLang/julia/commit/95bf00d61f4ef06f72ac6f8c18baf269f56f5bc4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21888#issuecomment-308244889)

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
| `["array","bool","boolarray_bool_load!"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","bool","boolarray_true_load!"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.70 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",8)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sum","3dsubarray")]` | 6.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 8313.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1:100000")]` | 19966.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","100000:-1:1")]` | 7836.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 27690.04 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 7.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 6.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 7.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 6.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 2.03 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 5.31 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 5.28 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 3.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 4.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 4.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","100000:-1:1")]` | 7210.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 27677.19 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1:100000")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_slow!"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",10)]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","Date")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["misc","afoldl","Float64"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.65 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{BigInt}(1)")]` | 1.66 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 2.13 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigInt}()")]` | 1.70 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigInt}(1)")]` | 2.14 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.83 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.81 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 1.70 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 1.71 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigFloat}()")]` | 1.98 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.97 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigInt}()")]` | 1.98 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigInt}(1)")]` | 1.94 (60%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 1.58 (40%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 1.98 (40%) :x: | 1.00 (1%)  |
| `["shootout","binary_trees"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","integer",100)]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",100)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(4,4),(4,4))]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
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
Julia Version 0.7.0-DEV.588
Commit 13732d1 (2017-06-13 20:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   69708894 s          0 s   12991874 s  3211545058 s         82 s
       #2  3501 MHz  290152445 s          0 s    8242264 s  3003521787 s         12 s
       #3  3501 MHz   62925539 s          0 s    7351216 s  3231983085 s         66 s
       #4  3501 MHz   59863414 s          0 s    7521160 s  3234865887 s         15 s
       
  Memory: 31.383651733398438 GB (2316.89453125 MB free)
  Uptime: 3.3038633e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.578
Commit 95bf00d (2017-06-13 20:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   69791215 s          0 s   13001901 s  3211983533 s         82 s
       #2  3501 MHz  290628702 s          0 s    8251249 s  3003568833 s         12 s
       #3  3501 MHz   63010686 s          0 s    7359704 s  3232421646 s         66 s
       #4  3501 MHz   59959134 s          0 s    7529655 s  3235293984 s         15 s
       
  Memory: 31.383651733398438 GB (2608.0 MB free)
  Uptime: 3.3043962e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
