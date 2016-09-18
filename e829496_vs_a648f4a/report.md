# Benchmark Report

## Job Properties

*Commit(s):* [TotalVerb/julia@e82949677090be71c3f1ace16d91f90a9957ec56](https://github.com/TotalVerb/julia/commit/e82949677090be71c3f1ace16d91f90a9957ec56) vs [JuliaLang/julia@a648f4a8eccd7c2bd8bd89c6835c3ee00bfad76a](https://github.com/JuliaLang/julia/commit/a648f4a8eccd7c2bd8bd89c6835c3ee00bfad76a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18572#issuecomment-247865792)

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
| `["array","cat",("catnd",5)]` | 0.66 (15%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["array","index",("sumelt","100000000:-1:1")]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 1.02 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.02 (15%)  | 0.99 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
Julia Version 0.6.0-dev.694
Commit e829496 (2016-09-18 18:46 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16726.75 MB free)
Uptime: 9.874671e6 sec
Load Avg:  1.0029296875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16392358 s          0 s    3426401 s  964827420 s         31 s
#2  3501 MHz   42932178 s          0 s    2131910 s  941758404 s          4 s
#3  3501 MHz   15182795 s          0 s    1868700 s  969943135 s         20 s
#4  3501 MHz   12851721 s          0 s    1869436 s  972257271 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.692
Commit a648f4a (2016-09-18 16:48 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16353.58984375 MB free)
Uptime: 9.879287e6 sec
Load Avg:  0.9658203125  0.99853515625  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16506448 s          0 s    3436154 s  965163870 s         31 s
#2  3501 MHz   43142684 s          0 s    2139766 s  942001171 s          4 s
#3  3501 MHz   15228685 s          0 s    1875341 s  970351463 s         20 s
#4  3501 MHz   12912079 s          0 s    1876420 s  972650993 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
