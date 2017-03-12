# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4ac416d7e6dee80be7fa3e06a3de490f18f1c9de](https://github.com/JuliaLang/julia/commit/4ac416d7e6dee80be7fa3e06a3de490f18f1c9de) vs [JuliaLang/julia@6445c82d0060dbe82b88436f0f4371a4ee64d918](https://github.com/JuliaLang/julia/commit/6445c82d0060dbe82b88436f0f4371a4ee64d918)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20993)

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
| `["array","cat",("catnd",5)]` | 0.63 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("catnd",500)]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 1.28 (15%) :x: | 1.06 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.04 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.20 (15%) :x: | 1.06 (1%) :x: |
| `["array","convert",("Complex{Float64}","Int")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Float64","Int")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","3d"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","4d"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","5d"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","sub2ind"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:100000.0")]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 1.72 (50%) :x: | 1.21 (1%) :x: |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 1.70 (50%) :x: | 1.21 (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 1.18 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000:-1:1")]` | 0.95 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000")]` | 0.86 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 0.58 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 0.58 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.57 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.59 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.56 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.57 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.59 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.58 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 0.84 (50%)  | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.58 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.58 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 1.03 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 1.03 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.02 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.03 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.03 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.03 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.02 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.03 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 1.05 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.66 (50%)  | 0.54 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.67 (50%)  | 0.54 (1%) :white_check_mark: |
| `["array","index",("sumrange","1.0:1.0:100000.0")]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BitArray{2}")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.89 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumvector_view","1.0:1.0:100000.0")]` | 0.98 (50%)  | 1.07 (1%) :x: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("mean","Float64")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("norm","Int64")]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sum","Float64")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs","Float64")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs2","Float64")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",3)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.45 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.16 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.21 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.30 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.64 (15%) :white_check_mark: | 0.45 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 1.05 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),2)]` | 0.47 (15%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["broadcast","sparse",((10000000,),1)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((10000000,),2)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","Date"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.42 (15%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.40 (15%) :white_check_mark: | 0.56 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.03 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.53 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.56 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","read","readstring"]` | 0.81 (15%) :white_check_mark: | 0.86 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.30 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.37 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.88 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.89 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.94 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.92 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.92 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 0.98 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 0.76 (45%)  | 0.84 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 0.61 (45%)  | 0.59 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",1024)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 0.04 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.01 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",256)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 0.05 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.06 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Diagonal",256)]` | 0.55 (45%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","factorization",("eig","Matrix",1024)]` | 1.91 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",256)]` | 2.27 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 0.05 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.06 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 0.49 (45%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.91 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 2.28 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",1024)]` | 2.08 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",256)]` | 2.36 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 2.08 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 2.36 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.00 (45%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 0.82 (45%)  | 0.68 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.05 (45%)  | 0.72 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 0.85 (45%)  | 0.72 (1%) :white_check_mark: |
| `["micro","parseint"]` | 0.76 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["micro","pisum"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","Int")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 2.66 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","parse","Int"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 0.03 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["misc","repeat",(200,24,1)]` | 0.06 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(false)")]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(true)")]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}()")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}()")]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(0)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(1)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}()")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(0)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(0)")]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(1)")]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}()")]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 0.28 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int64")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int8")]` | 0.28 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 0.29 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 0.24 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 0.17 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 0.24 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 0.06 (50%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.29 (15%) :x: | 1.24 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.30 (15%) :x: | 1.43 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.26 (15%) :x: | 1.12 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.27 (15%) :x: | 1.31 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.28 (15%) :x: | 1.41 (1%) :x: |
| `["problem","go","go_game"]` | 1.12 (15%)  | 1.11 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.77 (15%) :white_check_mark: | 0.99 (1%)  |
| `["problem","imdb","centrality"]` | 0.74 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.80 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.85 (15%)  | 0.00 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.00 (15%)  | 0.40 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 2.10 (15%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_devec"]` | 0.85 (15%)  | 0.50 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.77 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 1.04 (15%)  | 1.02 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 0.60 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["problem","stockcorr","stockcorr"]` | 2.27 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.10 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 3.09 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 3.12 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 2.89 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 2.93 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.07 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.07 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.99 (50%) :x: | 1.71 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.94 (50%) :x: | 1.71 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.97 (50%) :x: | 1.91 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.91 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.45 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.45 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.90 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.92 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.51 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.51 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.91 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.91 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 0.75 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.72 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.10 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{Int64}")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Complex{UInt64}")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.78 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.06 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.80 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.03 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.07 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.91 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.91 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.88 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.94 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.94 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.92 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.92 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 0.27 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","normal path, k = 2","Float 64")]` | 0.39 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float32")]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float64")]` | 0.18 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.03 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 0.03 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float32")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float64")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float32")]` | 0.07 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float64")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float32")]` | 0.29 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float64")]` | 0.28 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","binary_trees"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","fasta"]` | 0.96 (15%)  | 0.90 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.58 (15%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["shootout","nbody_vec"]` | 0.17 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","regex_dna"]` | 1.01 (15%)  | 1.05 (1%) :x: |
| `["shootout","revcomp"]` | 1.54 (25%) :x: | 0.97 (1%) :white_check_mark: |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.48 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.48 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 0.66 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.71 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 0.67 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ascending")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 2.46 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.54 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(600,600))]` | 0.49 (30%) :white_check_mark: | 0.99 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.95 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 1.93 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 0.66 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.64 (30%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.32 (30%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["sparse","index",("spvec","array",1000)]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","replace"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.124
Commit 4ac416d (2017-03-12 10:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4369.07421875 MB free)
Uptime: 2.4965669e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52834645 s          0 s    8149817 s  2430263536 s         75 s
#2  3501 MHz  190441238 s          0 s    8751628 s  2293299230 s         26 s
#3  3501 MHz   43791719 s          0 s    5115725 s  2446532350 s         40 s
#4  3501 MHz   39576517 s          0 s    5054125 s  2451042650 s         13 s

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
Memory: 31.383651733398438 GB (9171.91796875 MB free)
Uptime: 2.4973205e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52913355 s          0 s    8160122 s  2430925303 s         76 s
#2  3501 MHz  191141248 s          0 s    8764773 s  2293338985 s         26 s
#3  3501 MHz   43874270 s          0 s    5123885 s  2447194440 s         40 s
#4  3501 MHz   39656085 s          0 s    5061591 s  2451708641 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
