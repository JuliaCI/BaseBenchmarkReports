# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@1040aa08063096bac42c5bdbdae6a5d13da4bae5](https://github.com/pabloferz/julia/commit/1040aa08063096bac42c5bdbdae6a5d13da4bae5) vs [JuliaLang/julia@acfd04c18b6d498a834c15c2dfa5d33acbbb91ee](https://github.com/JuliaLang/julia/commit/acfd04c18b6d498a834c15c2dfa5d33acbbb91ee)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17929#issuecomment-238741663)

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
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.93 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.90 (15%) :x: | 1.01 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.03 (15%)  | 1.02 (1%) :x: |
| `["shootout","k_nucleotide"]` | 1.24 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.123
Commit 1040aa0 (2016-08-10 01:23 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21599.11328125 MB free)
Uptime: 6.442578e6 sec
Load Avg:  1.0029296875  0.99951171875  0.9580078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9217333 s          0 s    1794092 s  631741509 s         21 s
#2  3501 MHz   19394554 s          0 s    1340265 s  622881369 s          5 s
#3  3501 MHz    6792427 s          0 s     961931 s  636173025 s         10 s
#4  3501 MHz    4957122 s          0 s     931537 s  638083123 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-rc1+1
Commit acfd04c (2016-08-05 15:23 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21363.62109375 MB free)
Uptime: 6.447251e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9257700 s          0 s    1800365 s  632160780 s         21 s
#2  3501 MHz   19664540 s          0 s    1349967 s  623068393 s          5 s
#3  3501 MHz    6874602 s          0 s     969930 s  636549376 s         10 s
#4  3501 MHz    5001555 s          0 s     938058 s  638498931 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
