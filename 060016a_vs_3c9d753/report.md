# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@060016ae6423c967b82f7b72a8683b67ae1b0fd7](https://github.com/JuliaLang/julia/commit/060016ae6423c967b82f7b72a8683b67ae1b0fd7) vs [JuliaLang/julia@3c9d75391c72d7c32eea75ff187ce77b2d5effc8](https://github.com/JuliaLang/julia/commit/3c9d75391c72d7c32eea75ff187ce77b2d5effc8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/060016ae6423c967b82f7b72a8683b67ae1b0fd7#commitcomment-21131305)

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
| `["array","cat",("hcat",5)]` | 1.34 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 2.21 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 1.72 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hvcat_setind",5)]` | 1.83 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 1.22 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 2.10 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.04 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.03 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.75 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.80 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.74 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.82 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.85 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.98 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.99 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.86 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.76 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.80 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.84 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.92 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","Array{Float32,2}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","Array{Int32,2}")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.99 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000:-1:1")]` | 1.00 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000")]` | 1.05 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.88 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.88 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.74 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 0.65 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.82 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 0.77 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 0.64 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 0.65 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 0.81 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 0.66 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000)")]` | 0.99 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.98 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.99 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.45 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.01 (15%)  | 0.98 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","BigInt")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 0.86 (15%)  | 0.95 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.95 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 0.92 (1%) :white_check_mark: |
| `["shootout","meteor_contest"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.92 (15%)  | 0.93 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.98 (25%)  | 0.97 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 0.44 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 0.93 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 0.94 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","logical",100)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.40 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.1-pre+143
Commit 060016a (2017-03-01 10:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9251.421875 MB free)
Uptime: 2.4152637e7 sec
Load Avg:  0.984375  1.01318359375  1.0439453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   50005460 s          0 s    7780123 s  2352332321 s         72 s
#2  3501 MHz  172377878 s          0 s    8259638 s  2230712819 s         25 s
#3  3501 MHz   40894544 s          0 s    4819722 s  2368461733 s         39 s
#4  3501 MHz   36755725 s          0 s    4755851 s  2372888646 s         13 s

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
Memory: 31.383651733398438 GB (9047.375 MB free)
Uptime: 2.4160234e7 sec
Load Avg:  1.005859375  1.015625  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   50089564 s          0 s    7790946 s  2352994246 s         73 s
#2  3501 MHz  173081601 s          0 s    8270874 s  2230757001 s         25 s
#3  3501 MHz   40974594 s          0 s    4827664 s  2369132806 s         39 s
#4  3501 MHz   36835800 s          0 s    4764037 s  2373559591 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
