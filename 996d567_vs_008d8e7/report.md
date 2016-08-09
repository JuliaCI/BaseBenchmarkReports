# Benchmark Report

## Job Properties

*Commit(s):* [Sacha0/julia@996d56783daaef180ce5d4734ede7ba9d23d5a3c](https://github.com/Sacha0/julia/commit/996d56783daaef180ce5d4734ede7ba9d23d5a3c) vs [JuliaLang/julia@008d8e752cad0cf2c5890221f738d6c9ebcd8087](https://github.com/JuliaLang/julia/commit/008d8e752cad0cf2c5890221f738d6c9ebcd8087)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17302#issuecomment-238655772)

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
| `["array","subarray",("lucompletepivCopy!",100)]` | 16.24 (15%) :x: | 1.17 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.87 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 4.61 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",500)]` | 2.79 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 16.23 (15%) :x: | 1.17 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.87 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 4.78 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",500)]` | 2.78 (15%) :x: | 1.01 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 2.01 (15%) :x: | 1.01 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{UInt64}")]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.127
Commit 996d567 (2016-08-09 18:31 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22350.95703125 MB free)
Uptime: 6.419302e6 sec
Load Avg:  1.0361328125  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    8869127 s          0 s    1758134 s  629803927 s         21 s
#2  3501 MHz   18584005 s          0 s    1308641 s  621399863 s          5 s
#3  3501 MHz    6390469 s          0 s     928662 s  634283734 s         10 s
#4  3501 MHz    4762353 s          0 s     905427 s  635978742 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.112
Commit 008d8e7 (2016-08-09 16:45 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22012.515625 MB free)
Uptime: 6.42397e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    8932847 s          0 s    1766324 s  630197486 s         21 s
#2  3501 MHz   18769518 s          0 s    1315740 s  621673213 s          5 s
#3  3501 MHz    6528547 s          0 s     938347 s  634602165 s         10 s
#4  3501 MHz    4810694 s          0 s     911704 s  636390372 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
