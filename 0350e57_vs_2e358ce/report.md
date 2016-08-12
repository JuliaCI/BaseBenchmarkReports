# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7) vs [JuliaLang/julia@2e358ce975029ec97aba5994c17d4a2169c3b085](https://github.com/JuliaLang/julia/commit/2e358ce975029ec97aba5994c17d4a2169c3b085)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7#commitcomment-18621488)

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
| `["array","bool","boolarray_true_fill!"]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 1.32 (15%) :x: | 0.85 (1%) :white_check_mark: |
| `["array","cat",("catnd",500)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat",5)]` | 0.19 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.99 (15%)  | 1.13 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 0.79 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hvcat_setind",5)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 0.25 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.95 (15%)  | 1.13 (1%) :x: |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_single!",2048)]` | 1.78 (15%) :x: | 1.02 (1%) :x: |
| `["array","growth",("push_single!",256)]` | 1.89 (15%) :x: | 1.02 (1%) :x: |
| `["array","growth",("push_single!",8)]` | 1.82 (15%) :x: | 1.02 (1%) :x: |
| `["array","index","sub2ind"]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1:100000000")]` | 3.99 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.37 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 0.27 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 1.28 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 1.10 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.27 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.05 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.34 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.13 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.39 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.08 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.94 (40%)  | 1.08 (1%) :x: |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 0.23 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","Array{Int32,2}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 0.33 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BitArray{2}")]` | 0.33 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 0.04 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 0.25 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.35 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 2.06 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","Array{Int32,2}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.33 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.21 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.18 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.16 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.20 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.18 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.17 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.18 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.21 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.19 (40%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 0.27 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 1.29 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 1.07 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.25 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.08 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.31 (40%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.12 (40%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.20 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.12 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.89 (40%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 0.22 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 0.81 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumvector","100000000:-1:1")]` | 0.87 (40%)  | 1.06 (1%) :x: |
| `["array","index",("sumvector","1:100000000")]` | 0.79 (40%)  | 1.06 (1%) :x: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 0.86 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 0.89 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.79 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.83 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.78 (40%)  | 1.12 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.81 (40%)  | 1.12 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.85 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.83 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BitArray{2}")]` | 0.90 (40%)  | 1.12 (1%) :x: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 0.78 (40%)  | 1.05 (1%) :x: |
| `["array","reverse","rev_load_fast!"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_slow!"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 1.11 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 1.06 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 1.18 (15%) :x: | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 1.18 (15%) :x: | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 1.18 (15%) :x: | 1.38 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.63 (15%) :x: | 1.01 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.63 (15%) :x: | 1.01 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","read"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","readstring"]` | 0.42 (15%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.55 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.43 (30%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.62 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.43 (30%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",1024)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 0.95 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",256)]` | 0.94 (30%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 0.92 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 1.49 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 1.45 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",1024)]` | 0.92 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 0.94 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",256)]` | 0.93 (30%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 3.63 (30%) :x: | 2.01 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 3.69 (30%) :x: | 2.04 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 2.41 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 2.13 (30%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 2.47 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 2.65 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 1.98 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 2.21 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 2.52 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 2.37 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 3.83 (30%) :x: | 2.01 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 4.27 (30%) :x: | 2.04 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 2.26 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 2.07 (30%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 2.43 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 2.39 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 1.91 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 2.16 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 2.54 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 2.37 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.49 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.48 (30%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",1024)]` | 0.95 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 0.97 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",1024)]` | 0.95 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.95 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",1024)]` | 0.04 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",256)]` | 0.03 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Bidiagonal","Vector",256)]` | 0.88 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.50 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.48 (30%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.45 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.50 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",1024)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 1.10 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 1.30 (30%) :x: | 1.19 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 1.83 (30%) :x: | 1.70 (1%) :x: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",1024)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","blas","axpy!"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dotc"]` | 0.98 (40%)  | 1.20 (1%) :x: |
| `["linalg","blas","dotu"]` | 0.98 (40%)  | 1.20 (1%) :x: |
| `["linalg","factorization",("chol","Matrix",1024)]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("cholfact","Matrix",1024)]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Diagonal",256)]` | 1.60 (25%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("eig","Matrix",1024)]` | 0.97 (25%)  | 0.40 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Matrix",256)]` | 0.98 (25%)  | 0.41 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Diagonal",1024)]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 1.76 (25%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 0.99 (25%)  | 0.40 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 0.99 (25%)  | 0.41 (1%) :white_check_mark: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 1.08 (25%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 2.09 (25%) :x: | 1.02 (1%) :x: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.89 (25%) :x: | 1.01 (1%) :x: |
| `["micro","fib"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","mandel"]` | 0.94 (15%)  | 1.03 (1%) :x: |
| `["micro","parseint"]` | 1.14 (15%)  | 1.13 (1%) :x: |
| `["micro","randmatstat"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.98 (15%)  | 0.78 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.98 (15%)  | 0.68 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.97 (15%)  | 0.84 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.98 (15%)  | 0.67 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.00 (15%)  | 0.62 (1%) :white_check_mark: |
| `["problem","go","go_game"]` | 0.92 (15%)  | 1.42 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.88 (15%)  | 1.01 (1%) :x: |
| `["problem","imdb","centrality"]` | 0.90 (15%)  | 1.02 (1%) :x: |
| `["problem","json","parse_json"]` | 1.06 (15%)  | 1.23 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 3.90 (15%) :x: | 0.99 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 0.24 (15%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float32")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float64")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.93 (15%)  | 1.35 (1%) :x: |
| `["problem","stockcorr","stockcorr"]` | 1.26 (15%) :x: | 1.01 (1%)  |
| `["problem","ziggurat","ziggurat"]` | 1.08 (15%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.73 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 0.76 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 0.78 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigInt}")]` | 0.92 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.77 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.77 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 0.78 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.82 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.83 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 0.78 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.71 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 0.77 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 0.76 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 0.79 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 0.75 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigInt")]` | 0.93 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.71 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.74 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Int64}")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.70 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Int64")]` | 0.92 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 0.92 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.73 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.76 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.71 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.79 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.70 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 0.78 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigInt}")]` | 0.80 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.82 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 0.76 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.82 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 0.79 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{BigInt}")]` | 0.91 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 0.92 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.78 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.73 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 0.73 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 0.81 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 0.80 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.70 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.72 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.75 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 0.79 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 0.78 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 0.77 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.87 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.88 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.80 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.81 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 0.79 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 0.68 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 0.67 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 0.68 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 0.74 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.78 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.77 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.77 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float32}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Int64}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 0.81 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.78 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 0.68 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 0.73 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 0.87 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.87 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 0.86 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.88 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.71 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.71 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.86 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.86 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 0.73 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 0.72 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.75 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.77 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.86 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.87 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 0.72 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 0.68 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 0.69 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 0.66 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 0.74 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 0.68 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.70 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.71 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.77 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.77 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.75 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 0.69 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.72 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.76 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 0.66 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.72 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.88 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.76 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.85 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.76 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 0.76 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 0.66 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 0.69 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 0.69 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 0.73 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 0.76 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 0.76 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 0.69 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.68 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.80 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.79 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 0.76 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.69 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 0.74 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 0.78 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.69 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigInt")]` | 0.93 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.69 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.69 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.71 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Int64}")]` | 0.80 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.69 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Int64")]` | 0.92 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 0.92 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.74 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.71 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.75 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.71 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 0.55 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigInt}")]` | 0.58 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float32")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.82 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.67 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 0.76 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.82 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.67 (50%)  | 1.06 (1%) :x: |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float32}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 0.73 (40%)  | 1.06 (1%) :x: |
| `["scalar","fastmath",("div","Complex{Float32}")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Float64}")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","fannkuch"]` | 0.85 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["shootout","fasta"]` | 1.15 (15%)  | 1.10 (1%) :x: |
| `["shootout","k_nucleotide"]` | 1.09 (15%)  | 1.15 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.08 (1%) :x: |
| `["shootout","meteor_contest"]` | 0.80 (15%) :white_check_mark: | 0.99 (1%)  |
| `["shootout","nbody"]` | 0.95 (15%)  | 1.04 (1%) :x: |
| `["shootout","nbody_vec"]` | 0.88 (15%)  | 1.15 (1%) :x: |
| `["shootout","pidigits"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.86 (25%)  | 0.10 (1%) :white_check_mark: |
| `["simd",("axpy!","Float32",4095)]` | 0.37 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4096)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4095)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4096)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4095)]` | 0.47 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4096)]` | 0.45 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4096)]` | 0.80 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 0.48 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 0.47 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 0.10 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 0.10 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 0.11 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 0.10 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 0.55 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 0.54 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 0.54 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Int32",4095)]` | 0.51 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Int32",4096)]` | 0.50 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 18.00 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Float32",4096)]` | 18.20 (20%) :x: | 5.41 (1%) :x: |
| `["simd",("local_arrays","Float64",4095)]` | 19.32 (20%) :x: | 3.61 (1%) :x: |
| `["simd",("local_arrays","Float64",4096)]` | 19.36 (20%) :x: | 3.61 (1%) :x: |
| `["simd",("local_arrays","Int32",4095)]` | 26.83 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Int32",4096)]` | 26.67 (20%) :x: | 5.41 (1%) :x: |
| `["simd",("local_arrays","Int64",4095)]` | 16.05 (20%) :x: | 3.60 (1%) :x: |
| `["simd",("local_arrays","Int64",4096)]` | 16.04 (20%) :x: | 3.60 (1%) :x: |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.40 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.37 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.40 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.37 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.51 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4095)]` | 0.40 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4095)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4096)]` | 0.38 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4095)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4096)]` | 0.43 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 0.47 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4095)]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4096)]` | 0.45 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4095)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4096)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ascending")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ones")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","random")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","descending")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","random")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 0.60 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 0.98 (15%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 0.76 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 0.80 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 0.92 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 0.62 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 0.84 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 0.80 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 0.72 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.95 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 0.80 (15%) :white_check_mark: | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 0.94 (15%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.03 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 0.75 (15%) :white_check_mark: | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 0.76 (15%) :white_check_mark: | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 0.94 (15%)  | 1.11 (1%) :x: |
| `["sort","issorted",("forwards","ascending")]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ones")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 2.88 (30%) :x: | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","descending")]` | 0.59 (30%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","ones")]` | 0.78 (30%)  | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","random")]` | 2.77 (30%) :x: | 1.20 (1%) :x: |
| `["sort","mergesort",("sort forwards","ascending")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","descending")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","ones")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","ascending")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","descending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","ones")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ascending")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","descending")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ones")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ascending")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","descending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ones")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","ones")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.84 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.86 (15%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 0.86 (15%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 0.86 (15%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 0.86 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 0.83 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.66 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 0.87 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 0.94 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 0.94 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 0.96 (15%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 0.89 (15%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 0.94 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 0.94 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 0.93 (15%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 0.89 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spmat","array",10)]` | 4.67 (25%) :x: | 1.03 (1%) :x: |
| `["sparse","index",("spmat","array",100)]` | 3.95 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 2.98 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 4.27 (15%) :x: | 1.13 (1%) :x: |
| `["sparse","index",("spmat","col","array",100)]` | 3.12 (15%) :x: | 1.03 (1%) :x: |
| `["sparse","index",("spmat","col","array",1000)]` | 1.33 (15%) :x: | 1.01 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 0.90 (15%)  | 1.18 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 0.87 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","col","logical",1000)]` | 0.83 (15%) :white_check_mark: | 1.03 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 0.98 (15%)  | 1.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 1.01 (15%)  | 1.31 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 1.18 (15%) :x: | 1.81 (1%) :x: |
| `["sparse","index",("spmat","logical",10)]` | 0.81 (25%)  | 1.09 (1%) :x: |
| `["sparse","index",("spmat","range",10)]` | 0.86 (25%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","array",10)]` | 0.60 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 0.42 (15%) :white_check_mark: | 0.35 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.29 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 0.53 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.48 (15%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",1000)]` | 0.31 (15%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",10)]` | 0.46 (15%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",100)]` | 0.32 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",1000)]` | 0.22 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",10)]` | 0.75 (25%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 0.92 (25%)  | 0.81 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.95 (25%)  | 0.88 (1%) :white_check_mark: |
| `["sparse","index",("spvec","array",1000)]` | 1.40 (15%) :x: | 1.70 (1%) :x: |
| `["sparse","index",("spvec","array",10000)]` | 0.81 (15%) :white_check_mark: | 1.53 (1%) :x: |
| `["sparse","index",("spvec","array",100000)]` | 0.39 (15%) :white_check_mark: | 1.51 (1%) :x: |
| `["sparse","index",("spvec","integer",1000)]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.52 (15%) :x: | Inf (1%) :x: |
| `["sparse","index",("spvec","integer",100000)]` | 1.59 (15%) :x: | Inf (1%) :x: |
| `["sparse","index",("spvec","logical",1000)]` | 1.67 (15%) :x: | 0.61 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",10000)]` | 0.86 (15%)  | 0.52 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",100000)]` | 0.83 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",1000)]` | 0.01 (15%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",10000)]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",100000)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 0.95 (15%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 0.97 (15%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,400))]` | 0.94 (15%)  | 0.93 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,600))]` | 0.93 (15%)  | 0.95 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(600,400))]` | 0.88 (15%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(600,600))]` | 0.94 (15%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(600,400))]` | 1.01 (15%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(600,600))]` | 0.91 (15%)  | 0.93 (1%) :white_check_mark: |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.04 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float32)]` | 0.02 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 0.02 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float32)]` | 0.17 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float64)]` | 0.22 (40%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-rc2+0
Commit 0350e57 (2016-08-12 11:25 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21043.98046875 MB free)
Uptime: 6.656373e6 sec
Load Avg:  1.064453125  1.02978515625  0.96630859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   10738470 s          0 s    1962560 s  651384184 s         21 s
#2  3501 MHz   23812528 s          0 s    1521532 s  639629833 s          5 s
#3  3501 MHz    8306973 s          0 s    1113776 s  655864699 s         12 s
#4  3501 MHz    6264046 s          0 s    1080052 s  657992656 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.4.6
Commit 2e358ce (2016-06-19 17:16 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21025.875 MB free)
Uptime: 6.660859e6 sec
Load Avg:  0.9228515625  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   10806109 s          0 s    1969273 s  651757139 s         21 s
#2  3501 MHz   24053048 s          0 s    1529561 s  639829257 s          5 s
#3  3501 MHz    8367005 s          0 s    1120042 s  656246223 s         12 s
#4  3501 MHz    6320430 s          0 s    1086732 s  658377658 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
