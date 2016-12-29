# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d144f67a058dbd942a4dae7ebaf8cf1d7343ec13](https://github.com/JuliaLang/julia/commit/d144f67a058dbd942a4dae7ebaf8cf1d7343ec13) vs [JuliaLang/julia@309657f69c1a54fedfda5764b5b106286389383c](https://github.com/JuliaLang/julia/commit/309657f69c1a54fedfda5764b5b106286389383c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19545#issuecomment-269541996)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.34 (15%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.31 (15%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.03 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 2.10 (15%) :x: | 2.04 (1%) :x: |
| `["dates","string","DateTime"]` | 2.55 (15%) :x: | 3.05 (1%) :x: |
| `["linalg","factorization",("svdfact","Bidiagonal",1024)]` | 1.53 (45%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.84 (40%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","sparse"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
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
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1756
Commit d144f67 (2016-12-28 20:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6256.5703125 MB free)
Uptime: 1.861174e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25046505 s          0 s    5964488 s  1824840712 s         59 s
#2  3501 MHz   78897372 s          0 s    3616528 s  1777551780 s          8 s
#3  3501 MHz   24271070 s          0 s    3127740 s  1832920732 s         38 s
#4  3501 MHz   21621294 s          0 s    3208846 s  1835468063 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1738
Commit 309657f (2016-12-28 18:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5945.00390625 MB free)
Uptime: 1.8619182e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25103148 s          0 s    5973280 s  1825516878 s         59 s
#2  3501 MHz   79364148 s          0 s    3626321 s  1777818853 s          8 s
#3  3501 MHz   24319554 s          0 s    3134526 s  1833608941 s         38 s
#4  3501 MHz   21759513 s          0 s    3218663 s  1836063781 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
