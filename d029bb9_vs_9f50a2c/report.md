# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d029bb991db093a78c48c085ed50a40240ecc457](https://github.com/JuliaLang/julia/commit/d029bb991db093a78c48c085ed50a40240ecc457) vs [JuliaLang/julia@9f50a2cdbaf25a5431305b60b75db6cbc684fa07](https://github.com/JuliaLang/julia/commit/9f50a2cdbaf25a5431305b60b75db6cbc684fa07)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18583#issuecomment-248379389)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.93 (15%)  | 0.94 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.93 (15%)  | 0.97 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.94 (15%)  | 0.93 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.720
Commit d029bb9 (2016-09-20 17:26 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16043.0 MB free)
Uptime: 1.0044486e7 sec
Load Avg:  1.01513671875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16957185 s          0 s    3508984 s  981115320 s         32 s
#2  3501 MHz   44555991 s          0 s    2199977 s  957036604 s          4 s
#3  3501 MHz   15583922 s          0 s    1923767 s  986458365 s         21 s
#4  3501 MHz   13352053 s          0 s    1929648 s  988667504 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.718
Commit 9f50a2c (2016-09-20 15:35 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15844.5703125 MB free)
Uptime: 1.0049186e7 sec
Load Avg:  1.0029296875  1.0087890625  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16985906 s          0 s    3515209 s  981548781 s         32 s
#2  3501 MHz   44755320 s          0 s    2207445 s  957299321 s          4 s
#3  3501 MHz   15727132 s          0 s    1935154 s  986773064 s         21 s
#4  3501 MHz   13419839 s          0 s    1935967 s  989062757 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
