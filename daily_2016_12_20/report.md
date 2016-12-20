# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@194e4c96fec2e3ff8203cae1c9d8ffaf3dc3e61c](https://github.com/JuliaLang/julia/commit/194e4c96fec2e3ff8203cae1c9d8ffaf3dc3e61c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/194e4c96fec2e3ff8203cae1c9d8ffaf3dc3e61c#commitcomment-20242428)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-12-20 vs 2016-12-19

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
| `["array","index","5d"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("maxabs","Float64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("maxabs","Int64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs","Float64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs","Int64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs2","Float64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs2","Int64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("significand","subnorm","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.00 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |

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
Julia Version 0.6.0-dev.1626
Commit 194e4c9 (2016-12-20 00:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9518.1953125 MB free)
Uptime: 1.7863555e7 sec
Load Avg:  0.9228515625  0.998046875  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   28096476 s          0 s    4649046 s  1749991435 s         54 s
#2  3501 MHz   83191186 s          0 s    5668064 s  1694537243 s         20 s
#3  3501 MHz   24756294 s          0 s    3147599 s  1757636603 s         29 s
#4  3501 MHz   20754281 s          0 s    3057900 s  1761872620 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
