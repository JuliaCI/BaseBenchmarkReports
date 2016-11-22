# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@75790f52beeab7ccc5719c0c6d4a57a173d32040](https://github.com/JuliaLang/julia/commit/75790f52beeab7ccc5719c0c6d4a57a173d32040) vs [JuliaLang/julia@68af05e2ff1d9f17b52aeac06a43854a91cb212d](https://github.com/JuliaLang/julia/commit/68af05e2ff1d9f17b52aeac06a43854a91cb212d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17057#issuecomment-262154879)

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
| `["array","bool","bitarray_bool_load!"]` | 2.45 (15%) :x: | 1.00 (1%)  |
| `["array","bool","bitarray_true_load!"]` | 4.14 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 1.77 (15%) :x: | 1.48 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 1.56 (15%) :x: | 1.25 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 16.08 (15%) :x: | 1.75 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 23.73 (15%) :x: | 2.33 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 25.40 (15%) :x: | 2.33 (1%) :x: |
| `["array","cat",("vcat",5)]` | 6.29 (15%) :x: | 2.49 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 20.74 (15%) :x: | 2.56 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sum","3darray")]` | 10.34 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sum","3dsubarray")]` | 334.63 (50%) :x: | 8574.14 (1%) :x: |
| `["array","index",("sumcartesian","100000000:-1:1")]` | 1.00 (50%)  | Inf (1%) :x: |
| `["array","index",("sumcartesian","1:100000000")]` | 1.00 (50%)  | Inf (1%) :x: |
| `["array","index",("sumeach","100000000:-1:1")]` | 38.36 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","1:100000000")]` | 113.80 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 223.07 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 87.87 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 1.00 (50%)  | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 1.17 (50%)  | Inf (1%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 38.21 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear","1:100000000")]` | 130.25 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 31.60 (50%) :x: | 3.91 (1%) :x: |
| `["array","index",("sumlogical","100000000:-1:1")]` | 34.67 (50%) :x: | 3.91 (1%) :x: |
| `["array","index",("sumlogical","1:100000000")]` | 35.20 (50%) :x: | 3.91 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.69 (50%) :x: | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.65 (50%) :x: | 1.01 (1%) :x: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 27.42 (50%) :x: | 3.91 (1%) :x: |
| `["array","index",("sumrange","Array{Float32,2}")]` | 2.47 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 2.74 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 2.45 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 2.54 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.38 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.47 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 2.39 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 2.81 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 5.26 (50%) :x: | 3.14 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.55 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.60 (50%) :x: | 1.13 (1%) :x: |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 4.69 (50%) :x: | 1.63 (1%) :x: |
| `["array","index",("sumvector","100000000:-1:1")]` | 13.60 (50%) :x: | 3.83 (1%) :x: |
| `["array","index",("sumvector","1:100000000")]` | 16.93 (50%) :x: | 4.83 (1%) :x: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 4.35 (50%) :x: | 1.63 (1%) :x: |
| `["array","reductions",("mean","Float64")]` | 7.84 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("mean","Int64")]` | 8.22 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sum","Float64")]` | 7.85 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sum","Int64")]` | 8.35 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Float64")]` | 7.46 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Int64")]` | 4.49 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Float64")]` | 6.59 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Int64")]` | 2.91 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("var","Float64")]` | 5.37 (15%) :x: | 4.50 (1%) :x: |
| `["array","reductions",("var","Int64")]` | 2.49 (15%) :x: | 4.11 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.66 (15%) :x: | 1.05 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.66 (15%) :x: | 1.05 (1%) :x: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 1.00 (15%)  | 28.00 (1%) :x: |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.99 (15%)  | 3.30 (1%) :x: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 0.99 (15%)  | 3.00 (1%) :x: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 0.87 (15%)  | 7.00 (1%) :x: |
| `["broadcast","sparse",((1000,1000),2)]` | 1.15 (15%) :x: | 1.02 (1%) :x: |
| `["dates","parse","Date"]` | 1.83 (15%) :x: | 1.95 (1%) :x: |
| `["dates","parse","DateTime"]` | 2.02 (15%) :x: | 2.10 (1%) :x: |
| `["dates","parse",("Date","DateFormat")]` | 1.32 (15%) :x: | 1.35 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.51 (15%) :x: | 1.54 (1%) :x: |
| `["dates","string","Date"]` | 2.46 (15%) :x: | 1.77 (1%) :x: |
| `["dates","string","DateTime"]` | 3.94 (15%) :x: | 2.43 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.12 (45%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.37 (45%)  | 1.10 (1%) :x: |
| `["linalg","arithmetic",("/","Matrix","Matrix",1024)]` | 3.89 (45%) :x: | 3.02 (1%) :x: |
| `["linalg","arithmetic",("/","Matrix","Matrix",256)]` | 6.73 (45%) :x: | 3.02 (1%) :x: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",1024)]` | 1.14 (45%)  | 113415.86 (1%) :x: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",256)]` | 1.14 (45%)  | 2487.86 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.12 (45%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.38 (45%)  | 1.10 (1%) :x: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",1024)]` | 63.90 (45%) :x: | 16.65 (1%) :x: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 58.34 (45%) :x: | 15.70 (1%) :x: |
| `["linalg","factorization",("eig","LowerTriangular",1024)]` | 2.29 (45%) :x: | 1.84 (1%) :x: |
| `["linalg","factorization",("eig","LowerTriangular",256)]` | 3.14 (45%) :x: | 1.84 (1%) :x: |
| `["linalg","factorization",("eig","Matrix",1024)]` | 0.95 (45%)  | 1.10 (1%) :x: |
| `["linalg","factorization",("eig","Matrix",256)]` | 1.02 (45%)  | 1.30 (1%) :x: |
| `["linalg","factorization",("eigfact","LowerTriangular",1024)]` | 2.32 (45%) :x: | 1.84 (1%) :x: |
| `["linalg","factorization",("eigfact","LowerTriangular",256)]` | 3.15 (45%) :x: | 1.84 (1%) :x: |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.01 (45%)  | 1.10 (1%) :x: |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 1.02 (45%)  | 1.30 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.31 (45%)  | 1.04 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 2.61 (45%) :x: | 1.14 (1%) :x: |
| `["linalg","factorization",("svd","Bidiagonal",1024)]` | 2.52 (45%) :x: | 1.56 (1%) :x: |
| `["linalg","factorization",("svd","Bidiagonal",256)]` | 1.89 (45%) :x: | 1.56 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 41.89 (45%) :x: | 16.86 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 124.12 (45%) :x: | 41.80 (1%) :x: |
| `["linalg","factorization",("svd","LowerTriangular",1024)]` | 1.02 (45%)  | 1.42 (1%) :x: |
| `["linalg","factorization",("svd","LowerTriangular",256)]` | 1.30 (45%)  | 1.42 (1%) :x: |
| `["linalg","factorization",("svd","Matrix",1024)]` | 1.08 (45%)  | 1.48 (1%) :x: |
| `["linalg","factorization",("svd","Matrix",256)]` | 1.28 (45%)  | 1.48 (1%) :x: |
| `["linalg","factorization",("svd","UpperTriangular",1024)]` | 1.01 (45%)  | 1.42 (1%) :x: |
| `["linalg","factorization",("svd","UpperTriangular",256)]` | 1.30 (45%)  | 1.42 (1%) :x: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 37.94 (45%) :x: | 15.09 (1%) :x: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 116.43 (45%) :x: | 36.58 (1%) :x: |
| `["micro","mandel"]` | 3.13 (15%) :x: | 97.16 (1%) :x: |
| `["micro","randmatstat"]` | 1.63 (15%) :x: | 1.10 (1%) :x: |
| `["misc","parse","DateTime"]` | 1.87 (15%) :x: | 2.09 (1%) :x: |
| `["nullable","basic",("get2","Nullable{Bool}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Bool}(true)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float32}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float32}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float64}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int64}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int8}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int8}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(false)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(true)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(false)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(true)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(0.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(0.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(0.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(0.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Bool}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Bool}(true)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float32}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float32}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float64}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int64}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int8}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int8}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.28 (15%) :x: | 1.27 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.25 (15%) :x: | 1.45 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.22 (15%) :x: | 1.13 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.25 (15%) :x: | 1.34 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.25 (15%) :x: | 1.43 (1%) :x: |
| `["problem","fem","sparse_fem"]` | 2.01 (15%) :x: | 1.60 (1%) :x: |
| `["problem","go","go_game"]` | 3.65 (15%) :x: | 2.32 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 2.02 (15%) :x: | 1.14 (1%) :x: |
| `["problem","imdb","centrality"]` | 1.34 (15%) :x: | 2.37 (1%) :x: |
| `["problem","json","parse_json"]` | 1.24 (15%) :x: | 1.29 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 149.11 (15%) :x: | 55.78 (1%) :x: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.92 (15%) :x: | 3.28 (1%) :x: |
| `["problem","seismic",("seismic","Float32")]` | 4.88 (15%) :x: | 1.79 (1%) :x: |
| `["problem","seismic",("seismic","Float64")]` | 3.13 (15%) :x: | 1.40 (1%) :x: |
| `["problem","simplex","simplex"]` | 1.08 (15%)  | 2.38 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 4.20 (15%) :x: | 3.84 (1%) :x: |
| `["problem","stockcorr","stockcorr"]` | 1.11 (15%)  | 1.01 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Int64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Int64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{UInt64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{BigInt}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{BigInt}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{BigInt}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","fasta"]` | 1.07 (15%)  | 1.03 (1%) :x: |
| `["shootout","k_nucleotide"]` | 4.09 (15%) :x: | 3.15 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.64 (1%) :x: |
| `["shootout","nbody"]` | 1.00 (15%)  | 1.43 (1%) :x: |
| `["shootout","revcomp"]` | 1.23 (25%)  | 1.61 (1%) :x: |
| `["simd",("conditional_loop!","Float32",4095)]` | 1.32 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float32",4096)]` | 1.33 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4095)]` | 1.19 (20%)  | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4096)]` | 1.19 (20%)  | Inf (1%) :x: |
| `["simd",("conditional_loop!","Int32",4095)]` | 5.03 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Int32",4096)]` | 5.20 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Int64",4095)]` | 4.05 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Int64",4096)]` | 3.89 (20%) :x: | Inf (1%) :x: |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.79 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 4.06 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.78 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 4.03 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.51 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 3.60 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.51 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 3.59 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 2.85 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 2.95 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 2.87 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 2.95 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 1.31 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 1.30 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 1.31 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 1.30 (20%) :x: | 7.50 (1%) :x: |
| `["simd",("manual_example!","Float32",4095)]` | 2.82 (20%) :x: | Inf (1%) :x: |
| `["simd",("manual_example!","Float32",4096)]` | 2.89 (20%) :x: | Inf (1%) :x: |
| `["simd",("manual_example!","Float64",4095)]` | 2.38 (20%) :x: | Inf (1%) :x: |
| `["simd",("manual_example!","Float64",4096)]` | 2.40 (20%) :x: | Inf (1%) :x: |
| `["simd",("manual_example!","Int32",4095)]` | 2.65 (20%) :x: | Inf (1%) :x: |
| `["simd",("manual_example!","Int32",4096)]` | 2.70 (20%) :x: | Inf (1%) :x: |
| `["simd",("manual_example!","Int64",4095)]` | 1.77 (20%) :x: | Inf (1%) :x: |
| `["simd",("manual_example!","Int64",4096)]` | 1.74 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Float32",4095)]` | 13.80 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Float32",4096)]` | 13.19 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Float64",4095)]` | 7.91 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Float64",4096)]` | 7.77 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Int32",4095)]` | 14.82 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Int32",4096)]` | 14.41 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Int64",4095)]` | 8.40 (20%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Int64",4096)]` | 8.33 (20%) :x: | Inf (1%) :x: |
| `["simd",("two_reductions","Float32",4095)]` | 1.98 (20%) :x: | Inf (1%) :x: |
| `["simd",("two_reductions","Float32",4096)]` | 2.00 (20%) :x: | Inf (1%) :x: |
| `["simd",("two_reductions","Float64",4095)]` | 1.53 (20%) :x: | Inf (1%) :x: |
| `["simd",("two_reductions","Float64",4096)]` | 1.54 (20%) :x: | Inf (1%) :x: |
| `["simd",("two_reductions","Int32",4095)]` | 1.11 (20%)  | Inf (1%) :x: |
| `["simd",("two_reductions","Int32",4096)]` | 1.11 (20%)  | Inf (1%) :x: |
| `["simd",("two_reductions","Int64",4095)]` | 2.43 (20%) :x: | Inf (1%) :x: |
| `["simd",("two_reductions","Int64",4096)]` | 2.42 (20%) :x: | Inf (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 1.01 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.02 (30%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.99 (30%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.02 (30%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.04 (30%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.00 (30%)  | 1.25 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.02 (30%)  | 1.25 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 0.99 (30%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 0.96 (30%)  | 1.20 (1%) :x: |
| `["sort","issorted",("forwards","descending")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 1.95 (30%) :x: | 1.33 (1%) :x: |
| `["sort","issorted",("reverse","descending")]` | 1.03 (30%)  | 1.33 (1%) :x: |
| `["sort","issorted",("reverse","ones")]` | 1.01 (30%)  | 1.33 (1%) :x: |
| `["sort","issorted",("reverse","random")]` | 1.93 (30%) :x: | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.90 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.91 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.04 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.94 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 0.99 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 1.00 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.00 (30%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.00 (30%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 1.01 (30%)  | 1.25 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.01 (30%)  | 1.25 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 0.99 (30%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 0.99 (30%)  | 1.20 (1%) :x: |
| `["sparse","index",("spmat","array",10)]` | 1.32 (30%) :x: | 1.66 (1%) :x: |
| `["sparse","index",("spmat","array",100)]` | 1.26 (30%)  | 1.50 (1%) :x: |
| `["sparse","index",("spmat","array",1000)]` | 1.33 (30%) :x: | 1.26 (1%) :x: |
| `["sparse","index",("spmat","col","array",10)]` | 1.27 (30%)  | 1.26 (1%) :x: |
| `["sparse","index",("spmat","col","array",100)]` | 1.26 (30%)  | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","array",1000)]` | 1.01 (30%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","col","logical",10)]` | 3.15 (30%) :x: | 1.26 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 1.92 (30%) :x: | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.25 (30%)  | 1.03 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 13.21 (30%) :x: | 2.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 12.90 (30%) :x: | 1.95 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 8.57 (30%) :x: | 1.32 (1%) :x: |
| `["sparse","index",("spmat","range",10)]` | 3.76 (30%) :x: | 1.21 (1%) :x: |
| `["sparse","index",("spmat","range",100)]` | 1.25 (30%)  | 1.01 (1%) :x: |
| `["sparse","index",("spmat","row","range",10)]` | 4.96 (30%) :x: | 1.67 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.75 (30%) :x: | 1.43 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.12 (30%)  | 1.15 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.02 (30%)  | 2.04 (1%) :x: |
| `["sparse","index",("spvec","array",1000)]` | 1.02 (30%)  | 1.02 (1%) :x: |
| `["sparse","index",("spvec","logical",1000)]` | 1.29 (30%)  | 1.08 (1%) :x: |
| `["sparse","index",("spvec","range",1000)]` | 7.20 (30%) :x: | 1.48 (1%) :x: |
| `["sparse","index",("spvec","range",10000)]` | 4.31 (30%) :x: | 1.20 (1%) :x: |
| `["sparse","index",("spvec","range",100000)]` | 1.86 (30%) :x: | 1.08 (1%) :x: |

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
Julia Version 0.6.0-dev.1301
Commit 75790f5 (2016-11-22 05:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14928.08984375 MB free)
Uptime: 1.544625e7 sec
Load Avg:  0.9228515625  0.998046875  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   21505585 s          0 s    5003336 s  1513713671 s         44 s
#2  3501 MHz   64520681 s          0 s    3071050 s  1476085588 s          6 s
#3  3501 MHz   21342551 s          0 s    2681686 s  1519882679 s         32 s
#4  3501 MHz   18361545 s          0 s    2719289 s  1522799953 s          5 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1293
Commit 68af05e (2016-11-21 20:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14515.2890625 MB free)
Uptime: 1.5452075e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   21647088 s          0 s    5015365 s  1514140956 s         44 s
#2  3501 MHz   64854397 s          0 s    3078237 s  1476326655 s          6 s
#3  3501 MHz   21379903 s          0 s    2687643 s  1520421095 s         32 s
#4  3501 MHz   18399953 s          0 s    2726133 s  1523336519 s          5 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
