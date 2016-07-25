# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0d7c0142aee6a47082ef954caf4215ff45f0e106](https://github.com/JuliaLang/julia/commit/0d7c0142aee6a47082ef954caf4215ff45f0e106)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/0d7c0142aee6a47082ef954caf4215ff45f0e106#commitcomment-18379302)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-07-25 vs 2016-07-24

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
| `["array","cat",("catnd",5)]` | 1.09 (15%)  | 1.07 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_devec"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Int64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",100)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 1.85 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-pre+5664
Commit 0d7c014 (2016-07-24 18:30 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13708.05078125 MB free)
Uptime: 5.105671e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6372379 s          0 s    1271231 s  501798271 s         18 s
#2  3501 MHz   15488558 s          0 s    1084636 s  493494473 s          4 s
#3  3501 MHz    5356062 s          0 s     788976 s  504141671 s          7 s
#4  3501 MHz    4043652 s          0 s     773446 s  505509053 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
