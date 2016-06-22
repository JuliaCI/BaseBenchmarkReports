# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@45fa65f1f950609e471ad5f15f31bea103f8c823](https://github.com/JuliaLang/julia/commit/45fa65f1f950609e471ad5f15f31bea103f8c823)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/45fa65f1f950609e471ad5f15f31bea103f8c823#commitcomment-17962134)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-22 vs 2016-06-21

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
| `["array","setindex!",("setindex!",2)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.30 (15%) :x: | 0.99 (1%)  |
| `["sort","issorted",("forwards","ascending")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4893
Commit 45fa65f (2016-06-22 01:51 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (26700.515625 MB free)
Uptime: 2.217833e6 sec
Load Avg:  0.9228515625  0.998046875  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2631336 s          0 s     631216 s  217949611 s          7 s
#2  3501 MHz    8787056 s          0 s     459429 s  212395476 s          1 s
#3  3501 MHz    3491382 s          0 s     438268 s  217728884 s          1 s
#4  3501 MHz    2852814 s          0 s     419294 s  218386137 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
