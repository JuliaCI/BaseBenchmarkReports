# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b5fe42d446b311103b67f6190b62cf4b463adef2](https://github.com/JuliaLang/julia/commit/b5fe42d446b311103b67f6190b62cf4b463adef2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b5fe42d446b311103b67f6190b62cf4b463adef2#commitcomment-19437928)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-10-15 vs 2016-10-14

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
| `["array","bool","bitarray_true_load!"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 1.03 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","cat",("hcat",5)]` | 0.66 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.89 (15%)  | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hvcat",5)]` | 0.54 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hvcat_setind",5)]` | 0.52 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.75 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.46 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.83 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.98 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.12 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.11 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.12 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.13 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.13 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.15 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.08 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.11 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.12 (50%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.11 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.11 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.99 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 0.92 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000000:-1:1")]` | 0.94 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000000")]` | 0.92 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.88 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.89 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BitArray{2}")]` | 0.97 (50%)  | 0.90 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.62 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["io","read","readstring"]` | 0.80 (15%) :white_check_mark: | 0.86 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.99 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.50 (45%) :x: | 1.00 (1%)  |
| `["micro","parseint"]` | 0.99 (15%)  | 0.88 (1%) :white_check_mark: |
| `["micro","randmatstat"]` | 0.84 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 0.43 (45%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 1.01 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.01 (15%)  | 0.98 (1%) :white_check_mark: |
| `["problem","go","go_game"]` | 0.93 (15%)  | 0.89 (1%) :white_check_mark: |
| `["problem","imdb","centrality"]` | 0.94 (15%)  | 0.97 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.87 (15%) :x: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.97 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","fannkuch"]` | 1.01 (15%)  | 0.95 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.95 (15%)  | 0.88 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","meteor_contest"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 1.00 (15%)  | 0.97 (1%) :white_check_mark: |
| `["shootout","nbody_vec"]` | 0.80 (15%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["shootout","revcomp"]` | 1.05 (25%)  | 0.97 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.00 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 1.00 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 1.00 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.00 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 0.97 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.93 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.00 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.00 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.06 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.05 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort","issorted",("reverse","ascending")]` | 0.94 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","issorted",("reverse","descending")]` | 1.01 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","issorted",("reverse","ones")]` | 1.00 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","issorted",("reverse","random")]` | 0.97 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.02 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.02 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! forwards","ones")]` | 0.98 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! forwards","random")]` | 1.00 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.99 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! reverse","random")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 1.01 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.00 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.00 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 1.00 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.01 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sparse","index",("spmat","array",10)]` | 1.01 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.00 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",100)]` | 1.01 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","logical",10)]` | 0.74 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","logical",100)]` | 0.66 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 0.81 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.73 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.92 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse","index",("spmat","logical",10)]` | 0.71 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse","index",("spmat","logical",100)]` | 0.95 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","range",10)]` | 0.76 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 0.86 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.85 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",10)]` | 0.91 (30%)  | 0.87 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 0.97 (30%)  | 0.87 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.00 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",1000)]` | 0.95 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",1000)]` | 0.78 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",10000)]` | 0.86 (30%)  | 0.98 (1%) :white_check_mark: |
| `["string","join"]` | 1.69 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.977
Commit b5fe42d (2016-10-14 18:18 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15563.14453125 MB free)
Uptime: 1.2154842e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   19207187 s          0 s    4127360 s  1188693323 s         37 s
#2  3501 MHz   53569490 s          0 s    2609877 s  1158528797 s          5 s
#3  3501 MHz   18170951 s          0 s    2273031 s  1194455751 s         25 s
#4  3501 MHz   15816816 s          0 s    2289864 s  1196777365 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
