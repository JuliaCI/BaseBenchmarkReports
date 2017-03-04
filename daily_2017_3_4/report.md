# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@bb76add105e4dbda5185815fe0509b1b70fc0486](https://github.com/JuliaLang/julia/commit/bb76add105e4dbda5185815fe0509b1b70fc0486)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/bb76add105e4dbda5185815fe0509b1b70fc0486#commitcomment-21149961)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-03-04 vs 2017-03-03

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
| `["array","setindex!",("setindex!",4)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 2.48 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 3.09 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 2.69 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 2.54 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.98 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.46
Commit bb76add (2017-03-04 00:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8153.95703125 MB free)
Uptime: 2.4255046e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   42878431 s          0 s    8817372 s  2366784873 s         69 s
#2  3501 MHz  163072818 s          0 s    5375990 s  2255642498 s         10 s
#3  3501 MHz   38659972 s          0 s    4695902 s  2381009158 s         50 s
#4  3501 MHz   36239900 s          0 s    4844577 s  2383269143 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
