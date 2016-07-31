# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ca355ff994543ee0f630197110101323d9cc6dbd](https://github.com/JuliaLang/julia/commit/ca355ff994543ee0f630197110101323d9cc6dbd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ca355ff994543ee0f630197110101323d9cc6dbd#commitcomment-18462403)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-07-31 vs 2016-07-30

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
| `["linalg","blas","gbmv!"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","gbmv"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","gemv!"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","gemv"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","ger!"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","sbmv!"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","sbmv"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","symv!"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","syr!"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","trsv!"]` | 1.36 (20%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
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
Julia Version 0.5.0-rc0+72
Commit ca355ff (2016-07-30 15:32 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17909.8671875 MB free)
Uptime: 5.587504e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    7283504 s          0 s    1670791 s  548302551 s         19 s
#2  3501 MHz   20333198 s          0 s    1044216 s  537047498 s          2 s
#3  3501 MHz    7374573 s          0 s     954991 s  550150401 s         10 s
#4  3501 MHz    6144586 s          0 s     942323 s  551377787 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
