# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@0d98a916c5f1a5095fc05de2d159259294d4a80a](https://github.com/stevengj/julia/commit/0d98a916c5f1a5095fc05de2d159259294d4a80a) vs [JuliaLang/julia@923d23c594fca0082e7156d6dcf0485fdbd21868](https://github.com/JuliaLang/julia/commit/923d23c594fca0082e7156d6dcf0485fdbd21868)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17623#issuecomment-267213507)

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
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.29 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.11 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.14 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.67 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 1.11 (15%)  | 1.04 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.11 (15%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 0.75 (45%)  | 0.84 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 0.60 (45%)  | 0.60 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.81 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","norm","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("significand","subnorm","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 2.09 (15%) :x: | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 0.62 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.67 (30%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.75 (30%)  | 0.54 (1%) :white_check_mark: |

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
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1608
Commit 0d98a91 (2016-12-15 01:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10492.796875 MB free)
Uptime: 1.7418058e7 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26841615 s          0 s    4472374 s  1706964574 s         53 s
#2  3501 MHz   77144526 s          0 s    5449906 s  1656329263 s         20 s
#3  3501 MHz   23696590 s          0 s    3011650 s  1714307300 s         29 s
#4  3501 MHz   19522101 s          0 s    2912830 s  1718718833 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1564
Commit 923d23c (2016-12-14 20:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10264.91015625 MB free)
Uptime: 1.7423955e7 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26900424 s          0 s    4480987 s  1707485045 s         53 s
#2  3501 MHz   77535082 s          0 s    5458864 s  1656518804 s         20 s
#3  3501 MHz   23753238 s          0 s    3019602 s  1714831536 s         29 s
#4  3501 MHz   19573978 s          0 s    2919537 s  1719249243 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
