# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9f80eab7b4c26792bf7e2008436e90ac93890e19](https://github.com/JuliaLang/julia/commit/9f80eab7b4c26792bf7e2008436e90ac93890e19)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/9f80eab7b4c26792bf7e2008436e90ac93890e19#commitcomment-19328811)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-10-07 vs 2016-10-06

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.99 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.45 (45%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.89 (45%) :x: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ascending")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 2.47 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ascending")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.72 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.895
Commit 9f80eab (2016-10-07 01:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15752.6796875 MB free)
Uptime: 1.1463604e7 sec
Load Avg:  0.9228515625  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18936984 s          0 s    3163378 s  1121859065 s         35 s
#2  3501 MHz   48846170 s          0 s    3483399 s  1092392369 s         11 s
#3  3501 MHz   16554823 s          0 s    2109164 s  1127137109 s         18 s
#4  3501 MHz   13815542 s          0 s    2043856 s  1130044906 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
