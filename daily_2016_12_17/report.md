# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@56c009e1a26752107fec377e8de3bc7d562400b4](https://github.com/JuliaLang/julia/commit/56c009e1a26752107fec377e8de3bc7d562400b4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/56c009e1a26752107fec377e8de3bc7d562400b4#commitcomment-20222404)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-12-17 vs 2016-12-16

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
| `["array","reductions",("maxabs","Float64")]` | 257.73 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("maxabs","Int64")]` | 497.71 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Float64")]` | 4685.92 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Int64")]` | 2549.04 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Float64")]` | 4143.48 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Int64")]` | 1409.29 (15%) :x: | Inf (1%) :x: |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("significand","subnorm","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 1255.50 (15%) :x: | 15.14 (1%) :x: |

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
Julia Version 0.6.0-dev.1591
Commit 56c009e (2016-12-17 00:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9996.5859375 MB free)
Uptime: 1.761338e7 sec
Load Avg:  1.1630859375  1.03515625  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27448487 s          0 s    4549686 s  1725777115 s         53 s
#2  3501 MHz   79877960 s          0 s    5555099 s  1672981561 s         20 s
#3  3501 MHz   24164058 s          0 s    3071651 s  1733302448 s         29 s
#4  3501 MHz   20195114 s          0 s    2982022 s  1737501705 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
