# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fb312c40aa25e492c71648ecdc124af73a09993a](https://github.com/JuliaLang/julia/commit/fb312c40aa25e492c71648ecdc124af73a09993a) vs [JuliaLang/julia@333ff80e852aa20e9568e47d395ded82ad73f8d0](https://github.com/JuliaLang/julia/commit/333ff80e852aa20e9568e47d395ded82ad73f8d0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/fb312c40aa25e492c71648ecdc124af73a09993a#commitcomment-21489896)

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
| `["array","index",("sum","3darray")]` | 5.44 (50%) :x: | Inf (1%) :x: |
| `["array","reductions",("maxabs","Float64")]` | 1.15 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("maxabs","Int64")]` | 1.04 (15%)  | Inf (1%) :x: |
| `["array","reductions",("mean","Float64")]` | 6.60 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("mean","Int64")]` | 6.78 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sum","Float64")]` | 6.73 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sum","Int64")]` | 7.07 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Float64")]` | 6.07 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Int64")]` | 3.85 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Float64")]` | 4.26 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Int64")]` | 2.10 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("var","Float64")]` | 4.32 (15%) :x: | 1.88 (1%) :x: |
| `["array","reductions",("var","Int64")]` | 2.03 (15%) :x: | 1.78 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.29 (15%) :x: | 1.01 (1%)  |
| `["shootout","nbody_vec"]` | 7.31 (15%) :x: | 2.41 (1%) :x: |

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
Julia Version 0.6.0-pre.alpha.260
Commit fb312c4 (2017-03-25 22:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3036.0625 MB free)
Uptime: 2.6162928e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   49211598 s          0 s    9763084 s  2549723829 s         74 s
#2  3501 MHz  190946825 s          0 s    5951282 s  2417873345 s         11 s
#3  3501 MHz   43406598 s          0 s    5232513 s  2566414357 s         54 s
#4  3501 MHz   40914890 s          0 s    5374155 s  2568761897 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.259
Commit 333ff80 (2017-03-25 17:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2897.9296875 MB free)
Uptime: 2.6168775e7 sec
Load Avg:  1.078125  1.03564453125  1.0498046875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   49302294 s          0 s    9773092 s  2550205599 s         74 s
#2  3501 MHz  191475766 s          0 s    5960003 s  2417919808 s         11 s
#3  3501 MHz   43490396 s          0 s    5241009 s  2566906059 s         54 s
#4  3501 MHz   40997878 s          0 s    5382528 s  2569254689 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
