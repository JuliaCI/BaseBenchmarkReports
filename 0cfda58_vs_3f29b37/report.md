# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0cfda5806c4a2bb2816cd0f3271211d36978b140](https://github.com/JuliaLang/julia/commit/0cfda5806c4a2bb2816cd0f3271211d36978b140) vs [JuliaLang/julia@3f29b3789244e78fa3b1cd0f917cbd06194f4b79](https://github.com/JuliaLang/julia/commit/3f29b3789244e78fa3b1cd0f917cbd06194f4b79)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18196)

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
| `["array","cat",("catnd",5)]` | 1.70 (15%) :x: | 1.20 (1%) :x: |
| `["array","cat",("catnd",500)]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 4.10 (15%) :x: | 1.33 (1%) :x: |
| `["array","cat",("catnd_setind",500)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 15.31 (15%) :x: | 1.52 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 70.67 (15%) :x: | 2.00 (1%) :x: |
| `["array","cat",("hcat_setind",500)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 38.19 (15%) :x: | 1.65 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 42.34 (15%) :x: | 1.67 (1%) :x: |
| `["array","cat",("vcat",5)]` | 12.94 (15%) :x: | 1.70 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 50.60 (15%) :x: | 1.75 (1%) :x: |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1:100000000")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BitArray{2}")]` | 116.03 (40%) :x: | 7.01 (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1338.75 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1447.17 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000000)")]` | 0.38 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 2.90 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 19.20 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 3.03 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 6.02 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 7.42 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 6.08 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 6.70 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 6.32 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 6.83 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 6.08 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 6.69 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 8.89 (40%) :x: | 1.92 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1305.64 (40%) :x: | 45.06 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1460.74 (40%) :x: | 45.06 (1%) :x: |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 2.54 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","100000000:-1:1")]` | 4285206.79 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000000")]` | 12823728.00 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","Array{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","Array{Int32,2}")]` | 1.06 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.06 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.91 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1339.61 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1447.78 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","100000000:-1:1")]` | 7.00 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.02 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.90 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.01 (40%)  | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 745.60 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 870.48 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 141.65 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 139.95 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 141.46 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 139.97 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 39.28 (40%) :x: | 3.00 (1%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 404.96 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 417.35 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.38 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 4274594.14 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000000")]` | 12823659.25 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 169.47 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 170.99 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 169.97 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 170.69 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 462.96 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 434.54 (40%) :x: | Inf (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 2.70 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","100000000:-1:1")]` | 4.24 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1:100000000")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 5.14 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 4.94 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 5.12 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 5.28 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 5.18 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 5.11 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 5.16 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 5.23 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 2.58 (40%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 278.26 (40%) :x: | 15.24 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 276.92 (40%) :x: | 15.24 (1%) :x: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 2.16 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 2.93 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 19.25 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 3.21 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 5.98 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 6.65 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 6.10 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 6.69 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 6.27 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 7.20 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 6.08 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 6.64 (40%) :x: | 1.09 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 6.21 (40%) :x: | 1.53 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1312.52 (40%) :x: | 44.42 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1430.75 (40%) :x: | 44.42 (1%) :x: |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 2.55 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 1.17 (40%)  | 1.10 (1%) :x: |
| `["array","index",("sumvector","100000000:-1:1")]` | 1.59 (40%) :x: | 1.11 (1%) :x: |
| `["array","index",("sumvector","1:100000000")]` | 1.20 (40%)  | 1.11 (1%) :x: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 35.73 (40%) :x: | 2.75 (1%) :x: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 37.88 (40%) :x: | 2.75 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 35.21 (40%) :x: | 2.75 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 36.47 (40%) :x: | 2.75 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 31.69 (40%) :x: | 2.55 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 32.15 (40%) :x: | 2.55 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 35.90 (40%) :x: | 2.75 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 36.64 (40%) :x: | 2.75 (1%) :x: |
| `["array","index",("sumvector","BitArray{2}")]` | 7.89 (40%) :x: | 2.11 (1%) :x: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 167.86 (40%) :x: | 13.23 (1%) :x: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 169.70 (40%) :x: | 13.23 (1%) :x: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 1.14 (40%)  | 1.10 (1%) :x: |
| `["array","reverse","rev_load_fast!"]` | 2.61 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",2)]` | 2.07 (15%) :x: | 1.18 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 2.36 (15%) :x: | 1.23 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 2.94 (15%) :x: | 1.59 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 3.38 (15%) :x: | 2.00 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 3.43 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 3.41 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 1.31 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.29 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",1024)]` | 1.11 (30%)  | 23789.86 (1%) :x: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",256)]` | 1.16 (30%)  | 428.05 (1%) :x: |
| `["linalg","blas","gemm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","ger!"]` | 1.11 (40%)  | Inf (1%) :x: |
| `["linalg","blas","her!"]` | 1.01 (40%)  | Inf (1%) :x: |
| `["linalg","blas","herk!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","symm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","syr!"]` | 1.08 (40%)  | Inf (1%) :x: |
| `["linalg","blas","syrk!"]` | 0.99 (40%)  | Inf (1%) :x: |
| `["linalg","blas","trmm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg","blas","trsm!"]` | 0.99 (40%)  | Inf (1%) :x: |
| `["linalg","factorization",("eig","Matrix",1024)]` | 1.01 (25%)  | 1.08 (1%) :x: |
| `["linalg","factorization",("eig","Matrix",256)]` | 1.07 (25%)  | 1.16 (1%) :x: |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.01 (25%)  | 1.08 (1%) :x: |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 1.07 (25%)  | 1.16 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.74 (25%) :x: | 1.04 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 4.66 (25%) :x: | 1.10 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.32 (25%) :x: | 1.01 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 2.29 (25%) :x: | 1.03 (1%) :x: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.41 (25%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 2.20 (25%) :x: | 1.03 (1%) :x: |
| `["micro","mandel"]` | 1.20 (15%) :x: | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 3.15 (15%) :x: | 1.09 (1%) :x: |
| `["problem","go","go_game"]` | 9.88 (15%) :x: | 2.36 (1%) :x: |
| `["problem","imdb","centrality"]` | 0.98 (15%)  | 0.95 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.96 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 258.75 (15%) :x: | 16.92 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.58 (15%) :x: | 1.01 (1%)  |
| `["problem","seismic",("seismic","Float32")]` | 5.55 (15%) :x: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float64")]` | 3.17 (15%) :x: | 1.00 (1%)  |
| `["problem","simplex","simplex"]` | 1.10 (15%)  | 1.57 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 0.92 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 30.50 (50%) :x: | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 45.65 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 45.93 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 0.96 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.88 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 23.12 (50%) :x: | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 1.07 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 0.94 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 0.97 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 0.97 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 0.93 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 0.94 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 1.01 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigInt}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.90 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 1.01 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 1.07 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.97 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.88 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{UInt64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 30.30 (50%) :x: | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 22.81 (50%) :x: | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 45.13 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 1.06 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 45.37 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.89 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 0.96 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.99 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 0.93 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 0.94 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 1.08 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.01 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.04 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.03 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.05 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.16 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.94 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 1.00 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 1.02 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 1.04 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 1.03 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.91 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","Float64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Int64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 0.99 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","Float32")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Int64")]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","UInt64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 1.00 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 1.02 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Float64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Int64")]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","UInt64")]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 1.01 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float32")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Int64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","UInt64")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.92 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.02 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.02 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 1.04 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.01 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.01 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.04 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{Float64}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 1.02 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigInt}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 1.02 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigInt")]` | 1.01 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.88 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float32}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.91 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 1.02 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 0.99 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 1.01 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 0.91 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 0.96 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 0.93 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 1.00 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 0.95 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 0.94 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 0.96 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigInt}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.88 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 1.02 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 1.08 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.97 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.89 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 32.62 (50%) :x: | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 23.85 (50%) :x: | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 51.68 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 1.10 (50%)  | 1.29 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 51.70 (50%) :x: | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float32}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 0.97 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.91 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 1.00 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 1.00 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 0.98 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","Complex{BigInt}")]` | 0.99 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 0.97 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigInt}")]` | 0.99 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","predicate",("iseven","UInt64")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Float32")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Float64")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float32}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float64}")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","UInt64")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 2.00 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["shootout","spectralnorm"]` | 4.06 (15%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4095)]` | 16.15 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4096)]` | 16.96 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4095)]` | 8.36 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4096)]` | 8.38 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4095)]` | 14.00 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4096)]` | 14.66 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4095)]` | 2.52 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4096)]` | 2.48 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 40.49 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float32",4096)]` | 41.56 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4095)]` | 17.07 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4096)]` | 17.22 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Int32",4095)]` | 273.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 291.10 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 127.95 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 123.54 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 13.52 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 13.94 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 7.21 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 7.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int32",4095)]` | 12.60 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int32",4096)]` | 13.05 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int64",4095)]` | 1.81 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int64",4096)]` | 1.79 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 28.96 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 31.32 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 28.97 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 31.48 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 14.77 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 14.94 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 14.81 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 14.94 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 21.10 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 22.03 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 21.10 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 22.15 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.12 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 3.12 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.11 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 3.10 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4095)]` | 16.02 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4096)]` | 16.51 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 8.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 8.21 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4095)]` | 15.76 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4096)]` | 16.19 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4095)]` | 4.66 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4096)]` | 4.71 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 13.33 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 13.56 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 6.40 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 5.92 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 19.10 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 18.64 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4095)]` | 10.54 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4096)]` | 10.54 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 7.16 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 7.26 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 3.60 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 3.60 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4095)]` | 7.65 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4096)]` | 7.73 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ascending")]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","descending")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ones")]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","random")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","ascending")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","descending")]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","ones")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","random")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 2.07 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","descending")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ones")]` | 1.61 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! reverse","descending")]` | 2.02 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! reverse","ones")]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.96 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 3.10 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ones")]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 3.10 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ones")]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 2.34 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 3.10 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 3.10 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 2.19 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.59 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","ascending")]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","descending")]` | 2.07 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","ones")]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","random")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","ascending")]` | 1.93 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","descending")]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","ones")]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","random")]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ascending")]` | 1.88 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","descending")]` | 2.14 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ones")]` | 1.82 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","random")]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ascending")]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","descending")]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ones")]` | 1.82 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","random")]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 3.06 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 3.23 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","random")]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 3.27 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 3.02 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.83 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","random")]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 3.16 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 3.28 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.94 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","random")]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 3.35 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 3.13 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.87 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","random")]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ones")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","ones")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","ones")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 2.94 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 3.03 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ones")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","random")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 2.86 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 2.85 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ones")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","random")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 3.03 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 3.03 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 2.95 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 3.04 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","random")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["sparse","index",("spmat","col","array",100)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.92 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 6.02 (15%) :x: | 1.13 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 5.93 (15%) :x: | 1.11 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 3.69 (15%) :x: | 1.05 (1%) :x: |
| `["sparse","index",("spmat","logical",100)]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",1000)]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",100)]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 1.60 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",10)]` | 5.15 (15%) :x: | 1.20 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.83 (15%) :x: | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.20 (15%) :x: | 1.07 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 5.23 (15%) :x: | 1.14 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 2.06 (15%) :x: | 1.07 (1%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.19 (15%) :x: | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","range",10)]` | 5.67 (15%) :x: | 1.22 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.99 (15%) :x: | 1.14 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.36 (15%) :x: | 1.07 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 11.63 (25%) :x: | 1.62 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 3.07 (25%) :x: | 1.62 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.99 (25%)  | 1.52 (1%) :x: |
| `["sparse","index",("spvec","array",1000)]` | 1.91 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",10000)]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",100000)]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(600,400))]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(600,600))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(600,400))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",3,Float32)]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",3,Float64)]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 6.64 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 7.15 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",60,Float32)]` | 5.91 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",60,Float64)]` | 6.50 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",8,Float32)]` | 5.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",8,Float64)]` | 5.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",3,Float32)]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",3,Float64)]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 6.20 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 6.64 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float32)]` | 5.91 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 5.91 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float32)]` | 5.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float64)]` | 3.75 (40%) :x: | 1.00 (1%)  |

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
Commit 0cfda58 (2016-08-23 05:54 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20570.33203125 MB free)
Uptime: 7.582207e6 sec
Load Avg:  1.025390625  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12724962 s          0 s    2603172 s  740723463 s         25 s
#2  3501 MHz   32340099 s          0 s    1603736 s  723755142 s          4 s
#3  3501 MHz   11225106 s          0 s    1408470 s  745220599 s         15 s
#4  3501 MHz    9710529 s          0 s    1410894 s  746723305 s          2 s

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
Memory: 31.383651733398438 GB (20195.54296875 MB free)
Uptime: 7.586897e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12789206 s          0 s    2610844 s  741119125 s         26 s
#2  3501 MHz   32539672 s          0 s    1611999 s  724015836 s          4 s
#3  3501 MHz   11295282 s          0 s    1415006 s  745612038 s         15 s
#4  3501 MHz    9814376 s          0 s    1419764 s  747078936 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
