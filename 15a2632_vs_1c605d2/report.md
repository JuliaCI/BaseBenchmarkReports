# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@15a263245d05d9e6366f61262f7112d3f1f3657d](https://github.com/JuliaLang/julia/commit/15a263245d05d9e6366f61262f7112d3f1f3657d) vs [JuliaLang/julia@1c605d27a0d4760f12178a280444c9f0e8f93836](https://github.com/JuliaLang/julia/commit/1c605d27a0d4760f12178a280444c9f0e8f93836)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/15a263245d05d9e6366f61262f7112d3f1f3657d#commitcomment-20342104)

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
| `["array","cat",("catnd",5)]` | 0.86 (15%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 2.45 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 2.46 (50%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1845
Commit 15a2632 (2017-01-02 18:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3890.08203125 MB free)
Uptime: 1.90491e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33374037 s          0 s    5304607 s  1862366024 s         56 s
#2  3501 MHz  101033209 s          0 s    6313038 s  1794397641 s         20 s
#3  3501 MHz   28642885 s          0 s    3585708 s  1871799382 s         32 s
#4  3501 MHz   24202422 s          0 s    3469274 s  1876520516 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1845
Commit 1c605d2 (2017-01-02 18:59 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3729.5703125 MB free)
Uptime: 1.9055532e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96630859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33421458 s          0 s    5312090 s  1862952488 s         56 s
#2  3501 MHz  101408219 s          0 s    6321664 s  1794656459 s         20 s
#3  3501 MHz   28746045 s          0 s    3595492 s  1872328917 s         32 s
#4  3501 MHz   24287310 s          0 s    3477387 s  1877070194 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
