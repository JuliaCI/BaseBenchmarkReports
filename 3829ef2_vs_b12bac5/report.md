# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3829ef26be15e032b55baeb7d8cd62f1ac3a242d](https://github.com/JuliaLang/julia/commit/3829ef26be15e032b55baeb7d8cd62f1ac3a242d) vs [JuliaLang/julia@b12bac5c342483779abb1233faa8f5e4ee600659](https://github.com/JuliaLang/julia/commit/b12bac5c342483779abb1233faa8f5e4ee600659)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22481#issuecomment-310864487)

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
| `["array","cat",("catnd",5)]` | 0.75 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 0.62 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["array","convert",("Int","Complex{Float64}")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.16 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.34 (50%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","1.0:0.00010001000100010001:2.0")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","1.0:1.0:100000.0")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","BitArray{2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.72 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumelt","BitArray{2}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.16 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.72 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.81 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.86 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","1.0:0.00010001000100010001:2.0")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1.0:1.0:100000.0")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BitArray{2}")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.16 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 0.45 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",10)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.62 (15%) :x: | 1.30 (1%) :x: |
| `["dates","query",("dayofweek","Date")]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","DateTime")]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","read"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.48 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc","afoldl","Complex{Float64}"]` | 0.69 (15%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["misc","afoldl","Float64"]` | 0.05 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","afoldl","Int"]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","Int")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 0.68 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.35 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 0.35 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Bool")]` | 0.15 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 0.27 (50%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.99 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.99 (15%)  | 0.97 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.98 (15%)  | 0.97 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 0.95 (15%)  | 0.74 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","norm","Float64")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 1.49 (25%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 0.22 (1%) :white_check_mark: |
| `["simd",("two_reductions","Int32",4095)]` | 0.16 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 0.16 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 0.98 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 0.99 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 0.99 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.99 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.00 (30%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 0.99 (30%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.00 (30%)  | 1.38 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.00 (30%)  | 1.38 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.00 (30%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 0.99 (30%)  | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","ascending")]` | 3.52 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","random")]` | 3.60 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.10 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.09 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.02 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 0.99 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 1.00 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 1.00 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 0.99 (30%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 0.98 (30%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 0.98 (30%)  | 1.25 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 0.98 (30%)  | 1.25 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 0.99 (30%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 0.98 (30%)  | 1.20 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",100)]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 0.51 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",3,Float64)]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",3,Float32)]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(16,16),(16,16))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(2,2),(2,2))]` | 3.28 (15%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matvec",(2,2),(2,))]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,))]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(8,))]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.709
Commit 3829ef2 (2017-06-24 20:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   70826428 s          0 s   10893344 s  3309790597 s         93 s
       #2  3501 MHz  278449483 s          0 s   11948450 s  3102258658 s         39 s
       #3  3501 MHz   60765496 s          0 s    7063469 s  3329436457 s         51 s
       #4  3501 MHz   56182136 s          0 s    6976064 s  3334437800 s         18 s
       
  Memory: 31.383651733398438 GB (2590.4609375 MB free)
  Uptime: 3.3988069e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.706
Commit b12bac5 (2017-06-24 19:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   70905104 s          0 s   10902183 s  3310228331 s         93 s
       #2  3501 MHz  278935350 s          0 s   11956096 s  3102292160 s         39 s
       #3  3501 MHz   60847112 s          0 s    7070804 s  3329874158 s         51 s
       #4  3501 MHz   56256939 s          0 s    6983472 s  3334882866 s         18 s
       
  Memory: 31.383651733398438 GB (2546.1953125 MB free)
  Uptime: 3.3993347e7 sec
  Load Avg:  1.0029296875  1.015625  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
