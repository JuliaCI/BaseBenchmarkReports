# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b555a8d4e42f4299d6360faf1bfe80ae94ca52b5](https://github.com/JuliaLang/julia/commit/b555a8d4e42f4299d6360faf1bfe80ae94ca52b5) vs [JuliaLang/julia@26c8d856a2dd2f6a699f5bae46eee9be8c13a53d](https://github.com/JuliaLang/julia/commit/26c8d856a2dd2f6a699f5bae46eee9be8c13a53d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19779#issuecomment-269850975)

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
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 1.36 (50%)  | 1.53 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 1.37 (50%)  | 1.53 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 1.27 (50%)  | 1.60 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 1.29 (50%)  | 1.60 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 1.09 (50%)  | 1.60 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 1.09 (50%)  | 1.60 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 1.06 (50%)  | 1.53 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 1.05 (50%)  | 1.53 (1%) :x: |

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
Julia Version 0.6.0-dev.1809
Commit b555a8d (2016-12-31 04:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3492.33203125 MB free)
Uptime: 1.881812e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   31845407 s          0 s    5119628 s  1841036344 s         55 s
#2  3501 MHz   96550536 s          0 s    6145910 s  1775984357 s         20 s
#3  3501 MHz   27179006 s          0 s    3438985 s  1850329509 s         31 s
#4  3501 MHz   23170820 s          0 s    3346351 s  1854589503 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1807
Commit 26c8d85 (2016-12-31 04:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3325.01171875 MB free)
Uptime: 1.8824744e7 sec
Load Avg:  1.0029296875  1.005859375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   31962205 s          0 s    5131274 s  1841568524 s         55 s
#2  3501 MHz   96940003 s          0 s    6155098 s  1776247328 s         20 s
#3  3501 MHz   27244397 s          0 s    3446058 s  1850918617 s         31 s
#4  3501 MHz   23228240 s          0 s    3353180 s  1855186946 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
