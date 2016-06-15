# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@20d376e7a3cf5b9ae0569906ad66c9f213b01f60](https://github.com/JuliaLang/julia/commit/20d376e7a3cf5b9ae0569906ad66c9f213b01f60)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/20d376e7a3cf5b9ae0569906ad66c9f213b01f60#commitcomment-17872178)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-15 vs 2016-06-14

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
| `["array","bool","bitarray_true_load!"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 0.95 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 0.92 (15%)  | 1.13 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 1.00 (15%)  | 1.12 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.01 (15%)  | 1.13 (1%) :x: |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("prerend!",8)]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1:100000000")]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.74 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.99 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.49 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.57 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.57 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.49 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.49 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["array","setindex!",("setindex!",3)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",4)]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.67 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.68 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.65 (30%) :white_check_mark: | 0.99 (1%)  |
| `["micro","parseint"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.01 (15%)  | 1.22 (1%) :x: |
| `["problem","simplex"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.72 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! reverse","ones")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ones")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","random")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","ones")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","ones")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ones")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ones")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ones")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.03 (25%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.06 (15%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","logical",100)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",10)]` | 1.01 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 0.92 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.82 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.05 (15%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.85 (15%) :white_check_mark: | 1.04 (1%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 0.76 (15%) :white_check_mark: | 1.01 (1%)  |
| `["sparse","index",("spmat","splogical",10)]` | 1.08 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 0.86 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.85 (25%)  | 1.05 (1%) :x: |
| `["sparse","index",("spvec","logical",1000)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",10000)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",100000)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 2.00 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4776
Commit 20d376e (2016-06-15 03:12 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27399.15625 MB free)
Uptime: 1.613015e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     923705 s          0 s     303574 s  159708724 s          4 s
#2  3501 MHz    2375318 s          0 s     246106 s  158544795 s          1 s
#3  3501 MHz    1168829 s          0 s     203973 s  159833943 s          1 s
#4  3501 MHz     711851 s          0 s     176445 s  160344453 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
