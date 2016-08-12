# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3650b92e8612105290c8da4de451c86b562720f3](https://github.com/JuliaLang/julia/commit/3650b92e8612105290c8da4de451c86b562720f3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3650b92e8612105290c8da4de451c86b562720f3#commitcomment-18617416)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-12 vs 2016-08-11

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
| `["array","index",("sumcolon","100000000:-1:1")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Int32,2}")]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.47 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.48 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 0.95 (30%)  | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 0.65 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 0.22 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 0.10 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 0.33 (30%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 0.16 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 0.28 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 0.13 (30%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 0.33 (30%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 0.14 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 0.10 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 0.27 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 0.12 (30%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.74 (25%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.74 (25%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["micro","randmatstat"]` | 0.19 (15%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.69 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.70 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["shootout","nbody_vec"]` | 0.01 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 0.01 (15%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.02 (15%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.03 (15%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","range",100)]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.187
Commit 3650b92 (2016-08-12 02:33 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18729.90234375 MB free)
Uptime: 6.624323e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   10137780 s          0 s    2189391 s  648194339 s         22 s
#2  3501 MHz   25332784 s          0 s    1268304 s  635368037 s          3 s
#3  3501 MHz    9161497 s          0 s    1147586 s  651811596 s         12 s
#4  3501 MHz    7484406 s          0 s    1123116 s  653503820 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
