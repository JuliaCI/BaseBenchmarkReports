# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9874dd7ef9955d4580d37b64acb97d43ffada5a6](https://github.com/JuliaLang/julia/commit/9874dd7ef9955d4580d37b64acb97d43ffada5a6) vs [JuliaLang/julia@792ded802743830044198d2f525bded1f1c0bfb6](https://github.com/JuliaLang/julia/commit/792ded802743830044198d2f525bded1f1c0bfb6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/14763#issuecomment-249230434)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 1.86 (15%) :x: | 1.00 (1%)  |
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
Julia Version 0.6.0-dev.746
Commit 9874dd7 (2016-09-23 14:26 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17268.3828125 MB free)
Uptime: 1.0296503e7 sec
Load Avg:  1.0830078125  1.03125  0.9619140625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16319004 s          0 s    2805493 s  1008347827 s         32 s
#2  3501 MHz   40279518 s          0 s    2949526 s  985002876 s          9 s
#3  3501 MHz   14150052 s          0 s    1825570 s  1013171468 s         16 s
#4  3501 MHz   11835024 s          0 s    1781708 s  1015619760 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.743
Commit 792ded8 (2016-09-23 14:12 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16971.2734375 MB free)
Uptime: 1.0301221e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16461498 s          0 s    2816193 s  1008665215 s         32 s
#2  3501 MHz   40486690 s          0 s    2957500 s  985258820 s          9 s
#3  3501 MHz   14190552 s          0 s    1832022 s  1013595561 s         16 s
#4  3501 MHz   11885441 s          0 s    1788247 s  1016034091 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
