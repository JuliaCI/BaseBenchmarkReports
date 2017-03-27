# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@55f44179b9f9c75f8587c19f62cc17f031f5e3fd](https://github.com/JuliaLang/julia/commit/55f44179b9f9c75f8587c19f62cc17f031f5e3fd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/55f44179b9f9c75f8587c19f62cc17f031f5e3fd#commitcomment-21494947)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-03-27 vs 2017-03-26

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sum","3darray")]` | 0.19 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","reductions",("maxabs","Float64")]` | 0.99 (15%)  | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("maxabs","Int64")]` | 0.97 (15%)  | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("mean","Float64")]` | 0.17 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("mean","Int64")]` | 0.15 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sum","Float64")]` | 0.16 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sum","Int64")]` | 0.15 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs","Float64")]` | 0.16 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs","Int64")]` | 0.26 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs2","Float64")]` | 0.22 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs2","Int64")]` | 0.47 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("var","Float64")]` | 0.23 (15%) :white_check_mark: | 0.53 (1%) :white_check_mark: |
| `["array","reductions",("var","Int64")]` | 0.49 (15%) :white_check_mark: | 0.56 (1%) :white_check_mark: |
| `["array","setindex!",("setindex!",3)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.75 (15%) :white_check_mark: | 0.99 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.14 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.263
Commit 55f4417 (2017-03-27 00:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2881.15625 MB free)
Uptime: 2.6238211e7 sec
Load Avg:  1.01123046875  1.01953125  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   49561096 s          0 s    9815456 s  2556824274 s         74 s
#2  3501 MHz  193065817 s          0 s    5988580 s  2423241648 s         11 s
#3  3501 MHz   43739325 s          0 s    5268967 s  2573568883 s         54 s
#4  3501 MHz   41259041 s          0 s    5408733 s  2575908725 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
