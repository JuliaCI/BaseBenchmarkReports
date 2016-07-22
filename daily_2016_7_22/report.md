# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5fe9e5342b06ef0cec58e67b9f7e4e82a9f0a860](https://github.com/JuliaLang/julia/commit/5fe9e5342b06ef0cec58e67b9f7e4e82a9f0a860)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/5fe9e5342b06ef0cec58e67b9f7e4e82a9f0a860#commitcomment-18349840)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-07-22 vs 2016-07-21

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
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 1.86 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 2.15 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 1.65 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 1.79 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.68 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 2.13 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.91 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.40 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.73 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 2.04 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.94 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.24 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 1.61 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 1.86 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 2.15 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 1.64 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Int32,2}")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.74 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 2.13 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.01 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.25 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.75 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 2.13 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.89 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.19 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 1.61 (40%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 1.19 (15%) :x: | 1.40 (1%) :x: |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 254.15 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 263.62 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",100)]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 1.68 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.20 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-pre+5606
Commit 5fe9e53 (2016-07-21 19:23 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17864.09765625 MB free)
Uptime: 4.809861e6 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6420056 s          0 s    1447175 s  471837360 s         18 s
#2  3501 MHz   17682043 s          0 s     904147 s  462116212 s          2 s
#3  3501 MHz    6481593 s          0 s     832413 s  473438347 s          8 s
#4  3501 MHz    5540850 s          0 s     831457 s  474363498 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
