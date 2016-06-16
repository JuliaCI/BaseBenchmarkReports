# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4accf8a4f5b68dc9bfe410ae332fdc9d7b237722](https://github.com/JuliaLang/julia/commit/4accf8a4f5b68dc9bfe410ae332fdc9d7b237722) vs [JuliaLang/julia@d398d4ee03818e83cad38940640c479d7c786534](https://github.com/JuliaLang/julia/commit/d398d4ee03818e83cad38940640c479d7c786534)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/4accf8a4f5b68dc9bfe410ae332fdc9d7b237722#commitcomment-17902197)

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
| `["array","bool","bitarray_true_load!"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","bool","boolarray_bool_load!"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array","bool","boolarray_true_fill!"]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 0.90 (15%)  | 0.72 (1%) :white_check_mark: |
| `["array","cat",("catnd",500)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 0.20 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.96 (15%)  | 1.13 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 0.83 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.26 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.90 (15%)  | 1.13 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("append!",8)]` | 1.30 (15%) :x: | 1.01 (1%)  |
| `["array","growth",("push_single!",2048)]` | 1.78 (15%) :x: | 1.01 (1%) :x: |
| `["array","growth",("push_single!",256)]` | 1.85 (15%) :x: | 1.02 (1%) :x: |
| `["array","growth",("push_single!",8)]` | 1.80 (15%) :x: | 1.02 (1%) :x: |
| `["array","index","sub2ind"]` | 1.70 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1:100000000")]` | 3.98 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 1.40 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 1.29 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.46 (40%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.27 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.48 (40%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.32 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.45 (40%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.37 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.96 (40%)  | 1.08 (1%) :x: |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 0.36 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","Array{Int32,2}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BitArray{2}")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.12 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.12 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.12 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.11 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 2.06 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","Array{Int32,2}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.07 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.07 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.24 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.23 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.20 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.27 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.28 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.26 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.24 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.22 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.14 (40%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 1.36 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 1.27 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.38 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.18 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.41 (40%) :x: | 1.04 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.28 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.43 (40%) :x: | 1.04 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.32 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.92 (40%)  | 1.06 (1%) :x: |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 0.36 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 0.86 (40%)  | 1.11 (1%) :x: |
| `["array","index",("sumvector","100000000:-1:1")]` | 0.97 (40%)  | 1.11 (1%) :x: |
| `["array","index",("sumvector","1:100000000")]` | 0.98 (40%)  | 1.11 (1%) :x: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 0.98 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 0.98 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.91 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.92 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.05 (40%)  | 1.12 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.03 (40%)  | 1.12 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.00 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.00 (40%)  | 1.14 (1%) :x: |
| `["array","index",("sumvector","BitArray{2}")]` | 0.97 (40%)  | 1.12 (1%) :x: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 0.79 (40%)  | 1.11 (1%) :x: |
| `["array","setindex!",("setindex!",1)]` | 0.99 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 1.02 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 1.40 (15%) :x: | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 1.40 (15%) :x: | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 1.39 (15%) :x: | 1.38 (1%) :x: |
| `["io","read","readstring"]` | 0.41 (15%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["io","read"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.48 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.39 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",1024)]` | 0.95 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 0.97 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",256)]` | 1.02 (30%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 0.95 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 1.79 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 1.42 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",1024)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",256)]` | 1.00 (30%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 2.95 (30%) :x: | 2.01 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 3.66 (30%) :x: | 2.04 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 1.59 (30%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 1.40 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.36 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 1.34 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 3.06 (30%) :x: | 2.01 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 3.77 (30%) :x: | 2.04 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 1.61 (30%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 1.41 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.45 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 1.44 (30%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.64 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.91 (30%)  | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",1024)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 0.97 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",1024)]` | 0.78 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.66 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Bidiagonal","Vector",256)]` | 0.88 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.64 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.89 (30%)  | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.59 (30%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.94 (30%)  | 0.52 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",1024)]` | 0.97 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 1.10 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 1.32 (30%) :x: | 1.19 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 2.04 (30%) :x: | 1.70 (1%) :x: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",1024)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 0.96 (30%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","blas","axpy!"]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dot"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dotc"]` | 0.69 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["linalg","blas","dotu"]` | 0.69 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["linalg","blas","scal!"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","scal"]` | 1.33 (15%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("eig","Diagonal",256)]` | 1.37 (25%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("eig","Matrix",1024)]` | 0.98 (25%)  | 0.40 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Matrix",256)]` | 0.99 (25%)  | 0.41 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 1.64 (25%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 0.99 (25%)  | 0.40 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 0.99 (25%)  | 0.41 (1%) :white_check_mark: |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 1.16 (25%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.27 (25%) :x: | 1.01 (1%) :x: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.23 (25%)  | 1.01 (1%) :x: |
| `["micro","fib"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","mandel"]` | 0.91 (15%)  | 1.02 (1%) :x: |
| `["micro","parseint"]` | 1.27 (15%) :x: | 1.13 (1%) :x: |
| `["micro","randmatstat"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.20 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 1.24 (15%) :x: | 0.71 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 1.18 (15%) :x: | 0.85 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 1.21 (15%) :x: | 0.70 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.22 (15%) :x: | 0.65 (1%) :white_check_mark: |
| `["problem","go","go_game"]` | 0.99 (15%)  | 1.42 (1%) :x: |
| `["problem","imdb","centrality"]` | 0.95 (15%)  | 0.98 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 1.00 (15%)  | 1.22 (1%) :x: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 3.98 (15%) :x: | 0.99 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 0.24 (15%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["problem","seismic",("seismic","Float32")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","simplex"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["problem","spellcheck"]` | 1.00 (15%)  | 1.07 (1%) :x: |
| `["problem","stockcorr"]` | 1.23 (15%) :x: | 1.01 (1%)  |
| `["problem","ziggurat"]` | 1.22 (15%) :x: | 1.03 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 1.05 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 1.02 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 1.05 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 1.05 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 1.05 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 1.04 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 1.05 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 1.06 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 1.04 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigInt}")]` | 1.29 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 1.11 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 1.13 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{UInt64}")]` | 1.26 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 1.03 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 1.18 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 1.10 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 1.04 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 1.04 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 1.04 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 1.04 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 1.05 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigInt")]` | 1.29 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 1.08 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigInt}")]` | 1.28 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 1.17 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 1.18 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{UInt64}")]` | 1.35 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 1.12 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 1.13 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 1.35 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 1.06 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 1.13 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 1.18 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 1.06 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 1.12 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 1.18 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 1.05 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 1.04 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigInt")]` | 1.26 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigInt}")]` | 1.33 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 1.03 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 1.12 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 1.08 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 1.05 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 1.12 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 1.04 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 1.03 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 1.35 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 1.06 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.06 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.12 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.05 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.15 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.07 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.14 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.14 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 1.08 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 1.08 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 1.15 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 1.14 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 1.12 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 1.12 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 1.19 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 1.17 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 1.15 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 1.12 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 1.11 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 1.12 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Int64}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 1.12 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 1.18 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 1.12 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 1.15 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.05 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.05 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 1.09 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.04 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.07 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 1.10 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.05 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.08 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 1.08 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 1.12 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 1.10 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 1.08 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 1.08 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigInt}")]` | 1.27 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 1.14 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 1.16 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Int64}")]` | 1.27 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{UInt64}")]` | 1.28 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 1.13 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigFloat}")]` | 1.16 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 1.13 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 1.10 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 1.09 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Int64}")]` | 1.16 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{UInt64}")]` | 1.17 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 1.12 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 1.12 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigInt")]` | 1.27 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 1.11 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigInt}")]` | 1.27 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 1.19 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 1.18 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Int64}")]` | 1.27 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{UInt64}")]` | 1.28 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 1.13 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 1.13 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Int64")]` | 1.27 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","UInt64")]` | 1.30 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 1.14 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 1.12 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 1.18 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 1.15 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 1.10 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 1.17 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 1.10 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigInt")]` | 1.27 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigFloat}")]` | 1.16 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigInt}")]` | 1.27 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigInt")]` | 1.27 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigFloat}")]` | 1.16 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigInt}")]` | 1.27 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 1.08 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 1.13 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 1.13 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 1.12 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigInt}")]` | 1.28 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 1.14 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigInt}")]` | 1.43 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 1.08 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 1.09 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 1.10 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 1.09 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Int64}")]` | 1.11 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{UInt64}")]` | 1.10 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 1.09 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 1.08 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 1.09 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 1.10 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigInt}")]` | 1.26 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 1.14 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 1.14 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{UInt64}")]` | 1.25 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 1.04 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 1.04 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 1.15 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 1.10 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 1.11 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 1.14 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 1.07 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 1.05 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 1.03 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 1.02 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 1.08 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigInt")]` | 1.31 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 1.12 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigInt}")]` | 1.34 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 1.18 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 1.18 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{UInt64}")]` | 1.35 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 1.11 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 1.11 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 1.33 (50%)  | 0.67 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 1.06 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 1.13 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 1.14 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 1.06 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 1.12 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 1.15 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 1.12 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 1.20 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 1.15 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigInt")]` | 1.09 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 1.22 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigInt}")]` | 1.17 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float32")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 1.07 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 1.10 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 1.12 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 1.08 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 1.09 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 1.12 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 1.16 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 1.16 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigInt}")]` | 1.14 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 1.19 (40%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{BigInt}")]` | 1.27 (40%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{Float32}")]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 1.21 (40%)  | 1.06 (1%) :x: |
| `["scalar","fastmath",("div","Complex{Float32}")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Float64}")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 1.12 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","Complex{BigInt}")]` | 1.28 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 1.14 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigInt}")]` | 1.28 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{BigFloat}")]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{BigFloat}")]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["shootout","fannkuch"]` | 0.84 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["shootout","fasta"]` | 1.24 (15%) :x: | 1.10 (1%) :x: |
| `["shootout","k_nucleotide"]` | 1.17 (15%) :x: | 1.15 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","nbody"]` | 0.95 (15%)  | 1.04 (1%) :x: |
| `["shootout","nbody_vec"]` | 0.93 (15%)  | 1.15 (1%) :x: |
| `["shootout","revcomp"]` | 23.50 (15%) :x: | 1.91 (1%) :x: |
| `["simd",("axpy!","Float32",4095)]` | 0.37 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4096)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4095)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4096)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4095)]` | 0.47 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4096)]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4095)]` | 0.80 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4096)]` | 0.80 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 2.95 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 2.97 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 0.10 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 0.10 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 0.10 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 0.11 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 0.55 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 0.55 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 0.54 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Int32",4095)]` | 0.52 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Int32",4096)]` | 0.51 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 18.67 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Float32",4096)]` | 18.99 (20%) :x: | 5.41 (1%) :x: |
| `["simd",("local_arrays","Float64",4095)]` | 18.85 (20%) :x: | 3.61 (1%) :x: |
| `["simd",("local_arrays","Float64",4096)]` | 18.57 (20%) :x: | 3.61 (1%) :x: |
| `["simd",("local_arrays","Int32",4095)]` | 29.47 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Int32",4096)]` | 27.83 (20%) :x: | 5.41 (1%) :x: |
| `["simd",("local_arrays","Int64",4095)]` | 17.18 (20%) :x: | 3.60 (1%) :x: |
| `["simd",("local_arrays","Int64",4096)]` | 16.30 (20%) :x: | 3.60 (1%) :x: |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.42 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.38 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.42 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.38 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.40 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.40 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.50 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.52 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.50 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4095)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4095)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4096)]` | 0.38 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4095)]` | 0.43 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4096)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 0.45 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4095)]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4096)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4095)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4096)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ascending")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","random")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","descending")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","random")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 0.60 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 0.98 (15%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 0.96 (15%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 0.80 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 0.91 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 0.62 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 0.94 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 0.80 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 0.82 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.95 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.07 (15%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 0.94 (15%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 0.98 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 0.82 (15%) :white_check_mark: | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.00 (15%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 0.94 (15%)  | 1.11 (1%) :x: |
| `["sort","issorted",("forwards","ascending")]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ones")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 2.85 (30%) :x: | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","descending")]` | 0.57 (30%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","ones")]` | 0.83 (30%)  | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","random")]` | 2.71 (30%) :x: | 1.20 (1%) :x: |
| `["sort","mergesort",("sort reverse","descending")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","descending")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","random")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","random")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","random")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","random")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ascending")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","descending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","ones")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.80 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.82 (15%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 0.93 (15%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 0.88 (15%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 0.90 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 0.88 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.73 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 0.87 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 0.99 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 0.99 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.05 (15%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 0.92 (15%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 0.99 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 0.99 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 1.05 (15%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 0.93 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spmat","array",10)]` | 4.64 (25%) :x: | 1.03 (1%) :x: |
| `["sparse","index",("spmat","array",100)]` | 4.09 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 3.00 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 4.49 (15%) :x: | 1.12 (1%) :x: |
| `["sparse","index",("spmat","col","array",100)]` | 3.15 (15%) :x: | 1.03 (1%) :x: |
| `["sparse","index",("spmat","col","array",1000)]` | 1.21 (15%) :x: | 1.01 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 1.04 (15%)  | 1.18 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 1.03 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","col","logical",1000)]` | 0.95 (15%)  | 1.03 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 1.16 (15%) :x: | 1.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 1.11 (15%)  | 1.31 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 1.09 (15%)  | 1.81 (1%) :x: |
| `["sparse","index",("spmat","integer",10)]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 0.97 (25%)  | 1.09 (1%) :x: |
| `["sparse","index",("spmat","range",10)]` | 0.94 (25%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","array",10)]` | 0.68 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 0.49 (15%) :white_check_mark: | 0.35 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.38 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 0.65 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.58 (15%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",1000)]` | 0.41 (15%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",10)]` | 0.50 (15%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",100)]` | 0.36 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",1000)]` | 0.28 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",10)]` | 1.00 (25%)  | 0.81 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 1.19 (25%)  | 0.81 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.18 (25%)  | 0.88 (1%) :white_check_mark: |
| `["sparse","index",("spvec","array",1000)]` | 1.31 (15%) :x: | 1.69 (1%) :x: |
| `["sparse","index",("spvec","array",10000)]` | 0.83 (15%) :white_check_mark: | 1.53 (1%) :x: |
| `["sparse","index",("spvec","array",100000)]` | 0.42 (15%) :white_check_mark: | 1.51 (1%) :x: |
| `["sparse","index",("spvec","integer",1000)]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.81 (15%) :x: | Inf (1%) :x: |
| `["sparse","index",("spvec","integer",100000)]` | 1.87 (15%) :x: | Inf (1%) :x: |
| `["sparse","index",("spvec","logical",1000)]` | 1.96 (15%) :x: | 0.61 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",10000)]` | 0.94 (15%)  | 0.52 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",100000)]` | 0.91 (15%)  | 0.50 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",1000)]` | 0.01 (15%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",10000)]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",100000)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 1.02 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,400))]` | 1.01 (15%)  | 0.93 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,600))]` | 1.03 (15%)  | 0.95 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(600,400))]` | 0.99 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(600,600))]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(600,400))]` | 1.08 (15%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(600,600))]` | 1.03 (15%)  | 0.93 (1%) :white_check_mark: |
| `["string","join"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 2.54 (15%) :x: | 1.01 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 0.05 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.04 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float32)]` | 0.02 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 0.02 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float32)]` | 0.22 (40%) :white_check_mark: | 1.00 (1%)  |
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
- `["io"]`
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
- `["problem"]`
- `["problem","seismic"]`
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
Julia Version 0.5.0-dev+4816
Commit 4accf8a (2016-06-16 19:29 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27307.57421875 MB free)
Uptime: 1.75784e6 sec
Load Avg:  1.0234375  1.01416015625  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1671969 s          0 s     450570 s  173216128 s          5 s
#2  3501 MHz    5170787 s          0 s     307612 s  170197709 s          1 s
#3  3501 MHz    2358837 s          0 s     312858 s  173012745 s          1 s
#4  3501 MHz    1956600 s          0 s     285819 s  173449472 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.4.6-pre+43
Commit d398d4e (2016-06-15 00:25 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27449.58203125 MB free)
Uptime: 1.761046e6 sec
Load Avg:  1.0029296875  1.0146484375  1.04638671875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1729580 s          0 s     457266 s  173471131 s          5 s
#2  3501 MHz    5348694 s          0 s     313729 s  170333713 s          1 s
#3  3501 MHz    2407850 s          0 s     318876 s  173277470 s          1 s
#4  3501 MHz    2037826 s          0 s     293193 s  173680936 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
