# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e776d78deafb3a5341233f1f77157a44628d940a](https://github.com/JuliaLang/julia/commit/e776d78deafb3a5341233f1f77157a44628d940a) vs [JuliaLang/julia@3c9d75391c72d7c32eea75ff187ce77b2d5effc8](https://github.com/JuliaLang/julia/commit/3c9d75391c72d7c32eea75ff187ce77b2d5effc8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/e776d78deafb3a5341233f1f77157a44628d940a#commitcomment-21127087)

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
| `["array","cat",("hcat",5)]` | 1.33 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 2.17 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 1.65 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hvcat_setind",5)]` | 1.76 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 1.21 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 1.99 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.79 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.85 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.78 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.83 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000)")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 1.02 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.93 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.89 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.92 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.85 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.76 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.85 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.84 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 1.01 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000:-1:1")]` | 1.02 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000")]` | 1.05 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.87 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.82 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 0.64 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 0.67 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 0.62 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.80 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 0.82 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 0.65 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000)")]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.94 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.98 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.44 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.98 (15%)  | 0.98 (1%) :white_check_mark: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 0.94 (15%)  | 0.95 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 0.99 (15%)  | 0.92 (1%) :white_check_mark: |
| `["shootout","meteor_contest"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.91 (15%)  | 0.93 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.03 (25%)  | 0.97 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 0.99 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 0.96 (30%)  | 0.98 (1%) :white_check_mark: |

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
Julia Version 0.5.1-pre+99
Commit e776d78 (2017-02-22 13:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9279.5703125 MB free)
Uptime: 2.4145646e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   42157210 s          0 s    8722245 s  2356695948 s         69 s
#2  3501 MHz  158157580 s          0 s    5291300 s  2249711342 s         10 s
#3  3501 MHz   37901847 s          0 s    4622287 s  2370908945 s         50 s
#4  3501 MHz   35524259 s          0 s    4767874 s  2373130183 s          9 s

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
Memory: 31.383651733398438 GB (9310.984375 MB free)
Uptime: 2.4153152e7 sec
Load Avg:  1.0830078125  1.03125  1.05078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   42231638 s          0 s    8732518 s  2357358946 s         69 s
#2  3501 MHz  158862032 s          0 s    5303549 s  2249744649 s         10 s
#3  3501 MHz   37979135 s          0 s    4630571 s  2371573356 s         50 s
#4  3501 MHz   35602360 s          0 s    4775410 s  2373794623 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
