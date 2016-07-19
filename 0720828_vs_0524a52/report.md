# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@07208282fa78af9ea0661c44fd830bc80c44ccb9](https://github.com/JuliaLang/julia/commit/07208282fa78af9ea0661c44fd830bc80c44ccb9) vs [JuliaLang/julia@0524a52165e617125893d5bcbf91bf8b7f4d6cf1](https://github.com/JuliaLang/julia/commit/0524a52165e617125893d5bcbf91bf8b7f4d6cf1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17228#issuecomment-233734351)

*Tag Predicate:* `ALL`

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
| `["array","index",("sumcolon","100000000:-1:1")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 1.01 (40%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000000:-1:1")]` | 0.94 (40%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000000")]` | 0.93 (40%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 1.02 (40%)  | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.35 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.30 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.49 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.28 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.74 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.50 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.74 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.50 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.73 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.49 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.15 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5516
Commit 0720828 (2016-07-19 18:29 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13087.66796875 MB free)
Uptime: 4.605337e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5803070 s          0 s    1177422 s  452515153 s         17 s
#2  3501 MHz   14104215 s          0 s     958466 s  445049358 s          4 s
#3  3501 MHz    5071446 s          0 s     736584 s  454463121 s          6 s
#4  3501 MHz    3644718 s          0 s     692259 s  455980976 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5510
Commit 0524a52 (2016-07-19 18:28 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12954.91796875 MB free)
Uptime: 4.609974e6 sec
Load Avg:  1.0029296875  0.9921875  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5942456 s          0 s    1188210 s  452827534 s         17 s
#2  3501 MHz   14313029 s          0 s     966116 s  445296022 s          4 s
#3  3501 MHz    5121983 s          0 s     742177 s  454869818 s          6 s
#4  3501 MHz    3679393 s          0 s     697928 s  456403764 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
