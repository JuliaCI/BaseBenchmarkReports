# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e5b5a0924d60650246f4375bb8f7dfd97a7315d5](https://github.com/JuliaLang/julia/commit/e5b5a0924d60650246f4375bb8f7dfd97a7315d5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/e5b5a0924d60650246f4375bb8f7dfd97a7315d5#commitcomment-18103703)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-07-02 vs 2016-07-01

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
| `["array","bool","boolarray_bool_load!"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","reverse","rev_load_fast!"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_slow!"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["io","read"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 1.78 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 1.73 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","fasta"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.24 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["simd",("conditional_loop!","Float32",4095)]` | 0.19 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 0.19 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.37 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.37 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 0.02 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 0.02 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 0.04 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ones")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","ascending")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","descending")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","ones")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","random")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","ascending")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","descending")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","ones")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","random")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ascending")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","descending")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ones")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","random")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ascending")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","descending")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ones")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","random")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","random")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","random")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","random")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","random")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",1000)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",100)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","range",1000)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",1000)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5081
Commit e5b5a09 (2016-07-02 00:34 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (23892.51171875 MB free)
Uptime: 3.081768e6 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3630005 s          0 s     876923 s  302863175 s         12 s
#2  3501 MHz   10772114 s          0 s     578120 s  296638190 s          1 s
#3  3501 MHz    4048700 s          0 s     530597 s  303440253 s          3 s
#4  3501 MHz    3432801 s          0 s     524965 s  304052696 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
