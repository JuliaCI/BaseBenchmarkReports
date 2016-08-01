# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d68448cefb207f00a3f3882decc0c8bcd042b17c](https://github.com/JuliaLang/julia/commit/d68448cefb207f00a3f3882decc0c8bcd042b17c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/d68448cefb207f00a3f3882decc0c8bcd042b17c#commitcomment-18466236)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-01 vs 2016-07-31

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
| `["linalg","blas","gbmv!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gbmv"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gemv!"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gemv"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","ger!"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","sbmv!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","sbmv"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","symv!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","syr!"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","trsv!"]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","descending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,10000))]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 1.93 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 1.47 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc0+86
Commit d68448c (2016-08-01 03:45 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17893.09765625 MB free)
Uptime: 5.673905e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    7335962 s          0 s    1703549 s  556825479 s         19 s
#2  3501 MHz   20544522 s          0 s    1052166 s  545466811 s          2 s
#3  3501 MHz    7483067 s          0 s     964102 s  558671458 s         10 s
#4  3501 MHz    6210396 s          0 s     949945 s  559943268 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
