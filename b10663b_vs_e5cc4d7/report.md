# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b10663bd3b455ef3d4068566bde67d0dbde8d1df](https://github.com/JuliaLang/julia/commit/b10663bd3b455ef3d4068566bde67d0dbde8d1df) vs [JuliaLang/julia@e5cc4d7cdecf2eac83179564f4609e2b749321bf](https://github.com/JuliaLang/julia/commit/e5cc4d7cdecf2eac83179564f4609e2b749321bf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20005#issuecomment-313883705)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","index","ind2sub"]` | 0.13 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sum","3dsubarray")]` | 1.24 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.68 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.70 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Float32,2}")]` | 2.69 (50%) :x: | 1.60 (1%) :x: |
| `["array","index",("sumeach_view","Array{Int32,2}")]` | 2.69 (50%) :x: | 1.60 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Float32,2}")]` | 2.69 (50%) :x: | 1.60 (1%) :x: |
| `["array","index",("sumlinear_view","Array{Int32,2}")]` | 2.69 (50%) :x: | 1.60 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.51 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.51 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.07 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.07 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.13 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.16 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.94 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.02 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.94 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.99 (50%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.95 (50%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumrange","Array{Float32,2}")]` | 0.86 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 1.01 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.90 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.87 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.99 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.92 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.85 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.96 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.00 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.82 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.95 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.68 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.89 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.86 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.97 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.97 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.96 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.73 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.94 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.85 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumvector","1.0:0.00010001000100010001:2.0")]` | 0.82 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.84 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000:-1:1")]` | 0.91 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000")]` | 0.88 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.92 (50%)  | 0.87 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.89 (50%)  | 0.87 (1%) :white_check_mark: |
| `["array","reductions",("var","Float64")]` | 0.95 (15%)  | 0.83 (1%) :white_check_mark: |
| `["array","reductions",("var","Int64")]` | 0.98 (15%)  | 0.92 (1%) :white_check_mark: |
| `["broadcast","typeargs",("array",5)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.40 (45%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.72 (60%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.99 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.04 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 0.98 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.99 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.93 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 1.00 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.00 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.13 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 0.95 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 0.74 (50%)  | 1.02 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 0.74 (50%)  | 1.02 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.98 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 1.15 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 0.99 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.01 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.99 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.00 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["shootout","fasta"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(16,))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.873
Commit b10663b (2017-07-08 21:40 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   72792387 s          0 s   11148944 s  3428990445 s        110 s
       #2  3501 MHz  286399154 s          0 s   12358433 s  3215276497 s         40 s
       #3  3501 MHz   62366613 s          0 s    7238076 s  3449272719 s         55 s
       #4  3501 MHz   57842540 s          0 s    7180144 s  3454181353 s         19 s
       
  Memory: 31.383651733398438 GB (2218.99609375 MB free)
  Uptime: 3.5204572e7 sec
  Load Avg:  1.0234375  1.02392578125  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.870
Commit e5cc4d7 (2017-07-08 21:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   72888242 s          0 s   11158043 s  3429426622 s        110 s
       #2  3501 MHz  286885073 s          0 s   12366703 s  3215324814 s         40 s
       #3  3501 MHz   62446525 s          0 s    7245697 s  3449727658 s         55 s
       #4  3501 MHz   57920369 s          0 s    7187293 s  3454639053 s         19 s
       
  Memory: 31.383651733398438 GB (2684.7109375 MB free)
  Uptime: 3.5210005e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
