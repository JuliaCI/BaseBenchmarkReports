# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5d2e538c2be1c12f63a6865d41a2d4ce9e03ad1a](https://github.com/JuliaLang/julia/commit/5d2e538c2be1c12f63a6865d41a2d4ce9e03ad1a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/5d2e538c2be1c12f63a6865d41a2d4ce9e03ad1a#commitcomment-20354837)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-01-04 vs 2017-01-02

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
| `["array","growth",("append!",256)]` | 1.02 (15%)  | 1.04 (1%) :x: |
| `["array","growth",("prerend!",256)]` | 1.01 (15%)  | 0.99 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.43 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.43 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.47 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.47 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.76 (50%)  | 0.87 (1%) :white_check_mark: |

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
Julia Version 0.6.0-dev.1885
Commit 5d2e538 (2017-01-04 04:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (1772.453125 MB free)
Uptime: 1.9158269e7 sec
Load Avg:  1.0029296875  1.0146484375  0.99755859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33926450 s          0 s    5383061 s  1872621314 s         57 s
#2  3501 MHz  102761814 s          0 s    6352408 s  1803535840 s         20 s
#3  3501 MHz   28955882 s          0 s    3619490 s  1882363255 s         32 s
#4  3501 MHz   24646661 s          0 s    3509581 s  1886949633 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
