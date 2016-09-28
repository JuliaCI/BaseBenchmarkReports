# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a8bdc2e654f4fa0577d4bc46c37479ac0196f831](https://github.com/JuliaLang/julia/commit/a8bdc2e654f4fa0577d4bc46c37479ac0196f831) vs [JuliaLang/julia@3d8b39b54bc92b18b0fa915f1e462f82afa2e920](https://github.com/JuliaLang/julia/commit/3d8b39b54bc92b18b0fa915f1e462f82afa2e920)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a8bdc2e654f4fa0577d4bc46c37479ac0196f831#commitcomment-19205090)

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
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(0)")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ascending")]` | 1.20 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.660
Commit a8bdc2e (2016-09-16 04:22 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17822.05078125 MB free)
Uptime: 1.0707369e7 sec
Load Avg:  1.0029296875  1.0  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17082877 s          0 s    2903868 s  1048500413 s         34 s
#2  3501 MHz   42189941 s          0 s    3116448 s  1023926775 s         10 s
#3  3501 MHz   14732380 s          0 s    1901088 s  1053583839 s         16 s
#4  3501 MHz   12572318 s          0 s    1864887 s  1055872701 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.578
Commit 3d8b39b (2016-09-09 16:12 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17453.7890625 MB free)
Uptime: 1.0712021e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17124968 s          0 s    2911390 s  1048914617 s         34 s
#2  3501 MHz   42481258 s          0 s    3127984 s  1024088594 s         10 s
#3  3501 MHz   14788073 s          0 s    1906862 s  1053986783 s         16 s
#4  3501 MHz   12617402 s          0 s    1871372 s  1056285880 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
