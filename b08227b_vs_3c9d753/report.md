# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b08227b24619737d0e5966e3863268267ecb9ad5](https://github.com/JuliaLang/julia/commit/b08227b24619737d0e5966e3863268267ecb9ad5) vs [JuliaLang/julia@3c9d75391c72d7c32eea75ff187ce77b2d5effc8](https://github.com/JuliaLang/julia/commit/3c9d75391c72d7c32eea75ff187ce77b2d5effc8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b08227b24619737d0e5966e3863268267ecb9ad5#commitcomment-21134282)

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
| `["array","cat",("hcat",5)]` | 0.93 (15%)  | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hvcat",5)]` | 0.94 (15%)  | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.99 (15%)  | 0.97 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.92 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.04 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.04 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.79 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.88 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.77 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.88 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 1.00 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.97 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.94 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.08 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.93 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.84 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.81 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000:-1:1")]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000")]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.89 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 0.69 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 0.69 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 0.72 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 0.73 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000)")]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.89 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.89 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 0.99 (45%)  | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 0.99 (45%)  | 0.53 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 0.99 (45%)  | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 0.99 (45%)  | 0.53 (1%) :white_check_mark: |
| `["micro","randmatstat"]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc","parse","DateTime"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 1.11 (15%)  | 0.95 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.99 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 0.99 (15%)  | 0.92 (1%) :white_check_mark: |
| `["shootout","nbody_vec"]` | 0.94 (15%)  | 0.93 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.10 (25%)  | 0.97 (1%) :white_check_mark: |
| `["sparse","index",("spmat","array",10)]` | 1.05 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.08 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",10000)]` | 1.35 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.1-pre+173
Commit b08227b (2017-03-01 14:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9278.390625 MB free)
Uptime: 2.4175471e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   42543858 s          0 s    8769905 s  2359232648 s         69 s
#2  3501 MHz  160885322 s          0 s    5337830 s  2249916611 s         10 s
#3  3501 MHz   38307018 s          0 s    4662100 s  2373443238 s         50 s
#4  3501 MHz   35930522 s          0 s    4808051 s  2375663325 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0
Commit 3c9d753 (2016-09-19 18:14 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9060.55859375 MB free)
Uptime: 2.4180716e7 sec
Load Avg:  1.0498046875  1.0283203125  1.0478515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   42625157 s          0 s    8778998 s  2359664809 s         69 s
#2  3501 MHz  161364812 s          0 s    5346444 s  2249952428 s         10 s
#3  3501 MHz   38384896 s          0 s    4669931 s  2373881355 s         50 s
#4  3501 MHz   36003505 s          0 s    4816006 s  2376106350 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
