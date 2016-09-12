# Benchmark Report

## Job Properties

*Commit(s):* [Sacha0/julia@e9d31d309839177dd2b6ade0c6a49fa1100822c2](https://github.com/Sacha0/julia/commit/e9d31d309839177dd2b6ade0c6a49fa1100822c2) vs [JuliaLang/julia@9a4060704c686318195c5d4ccdce2a022ef2c696](https://github.com/JuliaLang/julia/commit/9a4060704c686318195c5d4ccdce2a022ef2c696)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17900#issuecomment-246238159)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",100)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 1.95 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",100000)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.601
Commit e9d31d3 (2016-09-12 03:57 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17207.94921875 MB free)
Uptime: 9.302978e6 sec
Load Avg:  1.0029296875  0.98681640625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15296976 s          0 s    3201426 s  909147167 s         29 s
#2  3501 MHz   39335219 s          0 s    1972868 s  888375400 s          4 s
#3  3501 MHz   13968395 s          0 s    1729174 s  914155132 s         17 s
#4  3501 MHz   11923085 s          0 s    1740546 s  916172885 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.599
Commit 9a40607 (2016-09-12 01:24 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16975.7109375 MB free)
Uptime: 9.30761e6 sec
Load Avg:  1.0830078125  1.03125  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15340845 s          0 s    3208238 s  909558107 s         29 s
#2  3501 MHz   39530214 s          0 s    1979570 s  888636419 s          4 s
#3  3501 MHz   14017780 s          0 s    1735322 s  914562096 s         17 s
#4  3501 MHz   12067821 s          0 s    1751450 s  916480066 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
