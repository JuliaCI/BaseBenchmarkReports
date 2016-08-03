# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@eb1162d08e0f235d8b3a1597655d18e1a334623e](https://github.com/JuliaLang/julia/commit/eb1162d08e0f235d8b3a1597655d18e1a334623e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/eb1162d08e0f235d8b3a1597655d18e1a334623e#commitcomment-18498190)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-03 vs 2016-08-02

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
| `["linalg","blas","gbmv!"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gbmv"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gemv!"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gemv"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","ger!"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","symv!"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","syr!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.26 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc0+148
Commit eb1162d (2016-08-03 02:53 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12935.76171875 MB free)
Uptime: 5.846637e6 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6950863 s          0 s    1420633 s  575007418 s         20 s
#2  3501 MHz   17549191 s          0 s    1243550 s  565295791 s          5 s
#3  3501 MHz    6133492 s          0 s     896710 s  577316878 s          9 s
#4  3501 MHz    4557429 s          0 s     874107 s  578956091 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
