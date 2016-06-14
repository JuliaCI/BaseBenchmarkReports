# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@2119ea6ff7c2e25ac5f587fad67241c6ecc1a8eb](https://github.com/JuliaLang/julia/commit/2119ea6ff7c2e25ac5f587fad67241c6ecc1a8eb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/2119ea6ff7c2e25ac5f587fad67241c6ecc1a8eb#commitcomment-17854748)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-14 vs 2016-06-13

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
| `["array","growth",("prerend!",8)]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",3)]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",4)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","random")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","descending")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","descending")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["io"]`
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
- `["problem"]`
- `["problem","seismic"]`
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
Julia Version 0.5.0-dev+4707
Commit 2119ea6 (2016-06-13 18:26 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27992.79296875 MB free)
Uptime: 1.526652e6 sec
Load Avg:  1.0029296875  1.0068359375  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     723782 s          0 s     271110 s  151324850 s          4 s
#2  3501 MHz    2055546 s          0 s     218346 s  150264552 s          1 s
#3  3501 MHz     836862 s          0 s     173160 s  151566555 s          1 s
#4  3501 MHz     552988 s          0 s     154705 s  151892530 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
