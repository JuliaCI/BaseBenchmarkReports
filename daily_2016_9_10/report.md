# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@843e0fea2549add6a7d1d6c752c5906691d601d6](https://github.com/JuliaLang/julia/commit/843e0fea2549add6a7d1d6c752c5906691d601d6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/843e0fea2549add6a7d1d6c752c5906691d601d6#commitcomment-18972398)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-09-10 vs 2016-09-09

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
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.04 (15%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.23 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.42 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.04 (15%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.23 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.43 (15%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.55 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.588
Commit 843e0fe (2016-09-10 01:21 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18115.58203125 MB free)
Uptime: 9.129879e6 sec
Load Avg:  1.0029296875  1.01513671875  1.02978515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   14953061 s          0 s    3144352 s  892280448 s         29 s
#2  3501 MHz   38372229 s          0 s    1924413 s  872088292 s          4 s
#3  3501 MHz   13746396 s          0 s    1692616 s  897116234 s         17 s
#4  3501 MHz   11697661 s          0 s    1704531 s  899134242 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
