# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@08e6dcc2056c628b0e09af8308b2a3af5f555854](https://github.com/JuliaLang/julia/commit/08e6dcc2056c628b0e09af8308b2a3af5f555854) vs [JuliaLang/julia@1c605d27a0d4760f12178a280444c9f0e8f93836](https://github.com/JuliaLang/julia/commit/1c605d27a0d4760f12178a280444c9f0e8f93836)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19779#issuecomment-270023861)

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
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.44 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.43 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.48 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.47 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |

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
Julia Version 0.6.0-dev.1847
Commit 08e6dcc (2017-01-02 21:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4379.1015625 MB free)
Uptime: 1.9046124e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27051653 s          0 s    6235899 s  1865880023 s         60 s
#2  3501 MHz   87820640 s          0 s    3837681 s  1811818829 s          8 s
#3  3501 MHz   25612624 s          0 s    3300792 s  1874813873 s         40 s
#4  3501 MHz   23427494 s          0 s    3402478 s  1876881655 s          7 s

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
Memory: 31.383651733398438 GB (4156.09765625 MB free)
Uptime: 1.9052733e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27118567 s          0 s    6244490 s  1866463205 s         60 s
#2  3501 MHz   88207147 s          0 s    3845763 s  1812084626 s          8 s
#3  3501 MHz   25691661 s          0 s    3308704 s  1875386862 s         40 s
#4  3501 MHz   23522882 s          0 s    3411852 s  1877437140 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
