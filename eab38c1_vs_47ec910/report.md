# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@eab38c1f8c3640a8906f1c894bc4c9a14007d200](https://github.com/pabloferz/julia/commit/eab38c1f8c3640a8906f1c894bc4c9a14007d200) vs [JuliaLang/julia@47ec910d2db23ab96024569b5bd6bb75e8053251](https://github.com/JuliaLang/julia/commit/47ec910d2db23ab96024569b5bd6bb75e8053251)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16986#issuecomment-246835477)

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
| `["array","subarray",("lucompletepivCopy!",100)]` | 2.56 (15%) :x: | 1.02 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",100)]` | 2.55 (15%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 19.57 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 47.44 (30%) :x: | 1.47 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 18.94 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 40.88 (30%) :x: | 1.47 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 7.98 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 21.76 (30%) :x: | 1.47 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 8.00 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 21.72 (30%) :x: | 1.47 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 8.15 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 22.12 (30%) :x: | 1.47 (1%) :x: |
| `["sparse","index",("spvec","integer",1000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.613
Commit eab38c1 (2016-09-13 20:42 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16950.890625 MB free)
Uptime: 9.453267e6 sec
Load Avg:  0.9169921875  0.96875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15719922 s          0 s    3275754 s  923629339 s         29 s
#2  3501 MHz   40698445 s          0 s    2026290 s  901981340 s          4 s
#3  3501 MHz   14307352 s          0 s    1772996 s  928793750 s         18 s
#4  3501 MHz   12315189 s          0 s    1786916 s  930757475 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.608
Commit 47ec910 (2016-09-13 19:55 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16781.203125 MB free)
Uptime: 9.457887e6 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15775127 s          0 s    3283805 s  924026666 s         29 s
#2  3501 MHz   40977142 s          0 s    2036794 s  902153732 s          4 s
#3  3501 MHz   14372779 s          0 s    1779626 s  929182799 s         18 s
#4  3501 MHz   12347310 s          0 s    1792440 s  931181216 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
