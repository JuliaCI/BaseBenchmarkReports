# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e7132b70686236e906461413a8ac69e626c26d56](https://github.com/JuliaLang/julia/commit/e7132b70686236e906461413a8ac69e626c26d56) vs [JuliaLang/julia@6445c82d0060dbe82b88436f0f4371a4ee64d918](https://github.com/JuliaLang/julia/commit/6445c82d0060dbe82b88436f0f4371a4ee64d918)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20993#issuecomment-292549510)

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
| `["array","bool","bitarray_bool_load!"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","bool","boolarray_bool_load!"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 0.61 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array","cat",("catnd",500)]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 0.62 (15%) :white_check_mark: | 1.06 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 0.84 (15%) :white_check_mark: | 1.06 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 0.65 (15%) :white_check_mark: | 1.06 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Complex{Float64}","Int")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Float64","Int")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_single!",256)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","3d"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","4d"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","5d"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","sub2ind"]` | 0.20 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:100000.0")]` | 2.16 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","Array{Float32,2}")]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 2.35 (50%) :x: | 1.21 (1%) :x: |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1:100000")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 2.44 (50%) :x: | 1.21 (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 1.06 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000:-1:1")]` | 0.83 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000")]` | 0.69 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 0.36 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 0.35 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.35 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.36 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.35 (50%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.35 (50%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.35 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.35 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 0.66 (50%)  | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.35 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.35 (50%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 0.61 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 0.61 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.61 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.61 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.61 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.61 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.59 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.61 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 0.66 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.36 (50%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.37 (50%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["array","index",("sumrange","1.0:1.0:100000.0")]` | 2.16 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BitArray{2}")]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","Array{Float32,2}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.82 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumvector_view","1.0:1.0:100000.0")]` | 0.95 (50%)  | 1.07 (1%) :x: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("mean","Float64")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("norm","Int64")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sum","Float64")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs","Float64")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs2","Float64")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reverse","rev_load_fast!"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reverse","rev_load_slow!"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 2.12 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 2.33 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.98 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.48 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.14 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.21 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.30 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.65 (15%) :white_check_mark: | 0.45 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 1.08 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),2)]` | 0.66 (15%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["broadcast","sparse",((10000000,),1)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((10000000,),2)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","Date"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.36 (15%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.35 (15%) :white_check_mark: | 0.56 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.03 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.51 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.58 (15%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["io","read","readstring"]` | 0.76 (15%) :white_check_mark: | 0.86 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.35 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.38 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.90 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.90 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.94 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.93 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.92 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",1024)]` | 0.39 (45%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",256)]` | 0.37 (45%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 0.98 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 0.76 (45%)  | 0.84 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 0.60 (45%)  | 0.59 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",1024)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 0.04 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.01 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",256)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 0.05 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.06 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Diagonal",256)]` | 0.51 (45%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","factorization",("eig","Matrix",1024)]` | 1.94 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",256)]` | 2.29 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 0.05 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.06 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 0.49 (45%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.95 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 2.28 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.70 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",1024)]` | 2.10 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",256)]` | 2.36 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 2.09 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 2.36 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Bidiagonal",1024)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.26 (45%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 0.88 (45%)  | 0.68 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.26 (45%)  | 0.72 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 0.91 (45%)  | 0.72 (1%) :white_check_mark: |
| `["micro","parseint"]` | 0.69 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["micro","pisum"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","Int")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 2.72 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","parse","Int"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 0.03 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["misc","repeat",(200,24,1)]` | 0.05 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["nullable","basic",("get2","Nullable{Float32}()")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(false)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(true)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}()")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(false)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(true)")]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(0.0)")]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(1.0)")]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}()")]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(0.0)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}()")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(0.0)")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(1.0)")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(1.0)")]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}()")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(0)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(1)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}()")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(0)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(0)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(1)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}()")]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(0)")]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(1)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 0.29 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int64")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int8")]` | 0.26 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Complex{Float64}")]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 0.39 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 0.29 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 0.17 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 0.06 (50%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.18 (15%) :x: | 1.26 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.19 (15%) :x: | 1.45 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.17 (15%) :x: | 1.13 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.18 (15%) :x: | 1.33 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.18 (15%) :x: | 1.44 (1%) :x: |
| `["problem","go","go_game"]` | 1.24 (15%) :x: | 1.11 (1%) :x: |
| `["problem","imdb","centrality"]` | 0.80 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.79 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.85 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.25 (15%) :x: | 0.40 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 2.24 (15%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_devec"]` | 0.87 (15%)  | 0.50 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.74 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 1.10 (15%)  | 1.02 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 0.64 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["problem","stockcorr","stockcorr"]` | 2.11 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.78 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.78 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.76 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.92 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 2.84 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 2.67 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 2.75 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 2.69 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.95 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.91 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.79 (50%) :x: | 1.71 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.78 (50%) :x: | 1.71 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.96 (50%) :x: | 1.91 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.97 (50%) :x: | 1.91 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.46 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.46 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.51 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.51 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 0.68 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.65 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.91 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{Int64}")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Complex{UInt64}")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.92 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.04 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.03 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.04 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.02 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.78 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.79 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.80 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.80 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.78 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.79 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.78 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.77 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.79 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.77 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.79 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.78 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.77 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.80 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Float32")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.89 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.86 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.74 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.76 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.76 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.76 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.85 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 0.31 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","normal path, k = 2","Float 64")]` | 0.39 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float32")]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float64")]` | 0.18 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.03 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 0.03 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float32")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float64")]` | 0.41 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float32")]` | 0.07 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float64")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float32")]` | 0.29 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float64")]` | 0.28 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","binary_trees"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["shootout","fasta"]` | 1.00 (15%)  | 0.90 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.67 (15%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["shootout","meteor_contest"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.18 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 2.22 (15%) :x: | 1.00 (1%)  |
| `["shootout","regex_dna"]` | 0.98 (15%)  | 1.05 (1%) :x: |
| `["shootout","revcomp"]` | 1.56 (25%) :x: | 0.97 (1%) :white_check_mark: |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.48 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 1.85 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 1.96 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 1.72 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 1.95 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Int64",4095)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 0.67 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.60 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 0.67 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ascending")]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 2.48 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","random")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(600,600))]` | 0.49 (30%) :white_check_mark: | 0.99 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 2.07 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 2.06 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 1.98 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.97 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 0.63 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.64 (30%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.35 (30%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["sparse","index",("spvec","array",1000)]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","replace"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(2,2),(2,2))]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(16,16))]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.63
Commit e7132b7 (2017-04-07 01:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6565.19921875 MB free)
Uptime: 2.7225979e7 sec
Load Avg:  1.064453125  1.02978515625  1.04931640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   55938590 s          0 s    8664680 s  2652228319 s         79 s
#2  3501 MHz  208597170 s          0 s    9493853 s  2500017469 s         30 s
#3  3501 MHz   46987030 s          0 s    5490158 s  2668902513 s         43 s
#4  3501 MHz   42597753 s          0 s    5428066 s  2673608958 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.1
Commit 6445c82 (2017-03-05 13:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9317.73828125 MB free)
Uptime: 2.7234793e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   56015589 s          0 s    8675955 s  2653018103 s         79 s
#2  3501 MHz  209426495 s          0 s    9512704 s  2500050089 s         30 s
#3  3501 MHz   47063455 s          0 s    5498141 s  2669698765 s         44 s
#4  3501 MHz   42676941 s          0 s    5435542 s  2674403070 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
