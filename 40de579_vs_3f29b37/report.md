# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@40de579053349de334f266af071415755d7cdc2a](https://github.com/JuliaLang/julia/commit/40de579053349de334f266af071415755d7cdc2a) vs [JuliaLang/julia@3f29b3789244e78fa3b1cd0f917cbd06194f4b79](https://github.com/JuliaLang/julia/commit/3f29b3789244e78fa3b1cd0f917cbd06194f4b79)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18196#issuecomment-241691365)

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
| `["array","cat",("catnd",5)]` | 1.89 (15%) :x: | 1.20 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 4.56 (15%) :x: | 1.33 (1%) :x: |
| `["array","cat",("hcat",5)]` | 15.15 (15%) :x: | 1.52 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 71.46 (15%) :x: | 2.00 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 38.00 (15%) :x: | 1.65 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 42.73 (15%) :x: | 1.67 (1%) :x: |
| `["array","cat",("vcat",5)]` | 12.77 (15%) :x: | 1.70 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 48.32 (15%) :x: | 1.75 (1%) :x: |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BitArray{2}")]` | 40.66 (40%) :x: | 3.00 (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 4.03 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 4.57 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 4.06 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 4.63 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 4.17 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 4.33 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 3.92 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 4.99 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 6.47 (40%) :x: | 1.62 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 6.64 (40%) :x: | 1.18 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 7.59 (40%) :x: | 1.18 (1%) :x: |
| `["array","index",("sumeach","Array{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","Array{Int32,2}")]` | 1.06 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.06 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.96 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.92 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","100000000:-1:1")]` | 6.04 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.02 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.90 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 748.20 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 881.98 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 147.23 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 139.77 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 144.06 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 139.61 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 40.46 (40%) :x: | 3.00 (1%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 283.62 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 281.47 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.38 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 84.54 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 84.75 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 84.57 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 85.27 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 157.30 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 157.91 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 1.49 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","100000000:-1:1")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1:100000000")]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 3.64 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 3.64 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 3.71 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 3.71 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 3.64 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 3.61 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 3.74 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 3.70 (40%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.90 (40%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 5.48 (40%) :x: | 1.22 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 5.39 (40%) :x: | 1.22 (1%) :x: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 1.52 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 4.02 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 4.39 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 3.91 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 4.74 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 3.90 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 4.64 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 4.06 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 4.76 (40%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 3.75 (40%) :x: | 1.27 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 6.58 (40%) :x: | 1.17 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 7.26 (40%) :x: | 1.17 (1%) :x: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 24.72 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 24.94 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 24.26 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 24.76 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 21.87 (40%) :x: | 1.89 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 21.85 (40%) :x: | 1.89 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 24.73 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 24.49 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector","BitArray{2}")]` | 4.67 (40%) :x: | 1.44 (1%) :x: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 43.77 (40%) :x: | 4.00 (1%) :x: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 45.05 (40%) :x: | 4.00 (1%) :x: |
| `["array","reverse","rev_load_fast!"]` | 2.61 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",2)]` | 2.16 (15%) :x: | 1.18 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 2.35 (15%) :x: | 1.23 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 2.80 (15%) :x: | 1.59 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 3.37 (15%) :x: | 2.00 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 3.21 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 3.22 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 1.21 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.32 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",1024)]` | 1.07 (30%)  | 23789.86 (1%) :x: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",256)]` | 1.09 (30%)  | 428.05 (1%) :x: |
| `["linalg","blas","gemm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","ger!"]` | 0.92 (40%)  | Inf (1%) :x: |
| `["linalg","blas","her!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","herk!"]` | 0.99 (40%)  | Inf (1%) :x: |
| `["linalg","blas","symm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","syr!"]` | 0.93 (40%)  | Inf (1%) :x: |
| `["linalg","blas","syrk!"]` | 1.01 (40%)  | Inf (1%) :x: |
| `["linalg","blas","trmm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","trsm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 2.39 (25%) :x: | 1.04 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 4.74 (25%) :x: | 1.10 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.99 (25%) :x: | 1.01 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 2.25 (25%) :x: | 1.03 (1%) :x: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.33 (25%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 2.14 (25%) :x: | 1.03 (1%) :x: |
| `["micro","mandel"]` | 1.20 (15%) :x: | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 3.15 (15%) :x: | 1.09 (1%) :x: |
| `["problem","go","go_game"]` | 10.05 (15%) :x: | 2.36 (1%) :x: |
| `["problem","imdb","centrality"]` | 0.97 (15%)  | 0.95 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.95 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.56 (15%) :x: | 1.02 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.58 (15%) :x: | 1.01 (1%)  |
| `["problem","simplex","simplex"]` | 1.04 (15%)  | 1.57 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 0.91 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 30.80 (50%) :x: | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 46.25 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 46.08 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 0.96 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.84 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 23.09 (50%) :x: | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 1.06 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 0.92 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 0.96 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 0.97 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 0.90 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 0.90 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigInt}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.81 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.85 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.99 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 1.07 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.84 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 31.14 (50%) :x: | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 22.87 (50%) :x: | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 46.31 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 1.06 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 47.46 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.85 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 0.96 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.99 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 0.92 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 0.91 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 1.07 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.01 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.03 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.04 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 1.06 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 1.06 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 1.04 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","Float64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Int64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","Float32")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Int64")]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","UInt64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 1.03 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Float64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Int64")]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","UInt64")]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 1.01 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Int64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","UInt64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.02 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.01 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 1.04 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.01 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.01 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.01 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.02 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{Float64}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigInt}")]` | 0.98 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 0.82 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigInt")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.86 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 1.07 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{UInt64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 1.02 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 1.01 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 0.99 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.88 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 0.90 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 0.95 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 0.95 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 0.96 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 0.92 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 0.90 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigInt}")]` | 0.98 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.84 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.97 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 1.08 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.97 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.85 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 34.11 (50%) :x: | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 23.89 (50%) :x: | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 53.40 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 1.10 (50%)  | 1.29 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 52.46 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float32}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.89 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 1.00 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 0.97 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","Complex{BigInt}")]` | 0.99 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 0.92 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigInt}")]` | 0.98 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","predicate",("iseven","UInt64")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Float32")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Float64")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float32}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","UInt64")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 1.99 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["shootout","spectralnorm"]` | 4.06 (15%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 38.04 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float32",4096)]` | 39.04 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4095)]` | 16.23 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4096)]` | 16.32 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Int32",4095)]` | 239.01 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 254.49 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 113.46 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 109.15 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 2.53 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 2.71 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 2.53 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 2.72 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 2.04 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 2.44 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 2.23 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 2.01 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 2.08 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 2.32 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 2.26 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 2.06 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 2.53 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 2.53 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 2.47 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 2.46 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 2.60 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 2.60 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 2.54 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 2.56 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.70 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 5.90 (15%) :x: | 1.13 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 5.50 (15%) :x: | 1.11 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 3.65 (15%) :x: | 1.05 (1%) :x: |
| `["sparse","index",("spmat","row","array",10)]` | 5.09 (15%) :x: | 1.20 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.58 (15%) :x: | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.18 (15%) :x: | 1.07 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 5.22 (15%) :x: | 1.14 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.89 (15%) :x: | 1.07 (1%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.09 (15%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","range",10)]` | 5.36 (15%) :x: | 1.22 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.71 (15%) :x: | 1.14 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.23 (15%) :x: | 1.07 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 12.05 (25%) :x: | 1.62 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 3.08 (25%) :x: | 1.62 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.00 (25%)  | 1.52 (1%) :x: |
| `["sparse","index",("spvec","array",1000)]` | 1.72 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",10000)]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",100000)]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.82 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.369
Commit 40de579 (2016-08-23 10:30 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20682.93359375 MB free)
Uptime: 7.598454e6 sec
Load Avg:  1.0029296875  1.0146484375  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13167634 s          0 s    2313123 s  742635556 s         24 s
#2  3501 MHz   31013863 s          0 s    1975444 s  726009929 s          6 s
#3  3501 MHz   11416965 s          0 s    1437784 s  746587033 s         12 s
#4  3501 MHz    8941290 s          0 s    1391836 s  749171999 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.366
Commit 3f29b37 (2016-08-23 02:20 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20533.33203125 MB free)
Uptime: 7.603127e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13208148 s          0 s    2319072 s  743055104 s         24 s
#2  3501 MHz   31207651 s          0 s    1983844 s  726274243 s          6 s
#3  3501 MHz   11560128 s          0 s    1448857 s  746899509 s         12 s
#4  3501 MHz    8999955 s          0 s    1398100 s  749573760 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
