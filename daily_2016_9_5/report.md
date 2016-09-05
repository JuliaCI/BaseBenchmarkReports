# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6bb08bfec20c5678a1147022ce3ccc18db94601d](https://github.com/JuliaLang/julia/commit/6bb08bfec20c5678a1147022ce3ccc18db94601d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/6bb08bfec20c5678a1147022ce3ccc18db94601d#commitcomment-18895235)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-09-05 vs 2016-09-04

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
| `["array","growth",("prerend!",8)]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 30.93 (15%) :x: | 1.18 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.90 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 5.21 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",500)]` | 2.95 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 31.09 (15%) :x: | 1.18 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.92 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 5.34 (15%) :x: | 1.03 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",500)]` | 2.96 (15%) :x: | 1.01 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 2.08 (15%) :x: | 1.01 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ascending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.483
Commit 6bb08bf (2016-09-05 00:55 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19924.96484375 MB free)
Uptime: 8.697844e6 sec
Load Avg:  1.0029296875  1.0146484375  0.95947265625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   14077712 s          0 s    2485977 s  851312402 s         27 s
#2  3501 MHz   34144308 s          0 s    2329808 s  832231606 s          8 s
#3  3501 MHz   12457258 s          0 s    1587179 s  855299554 s         13 s
#4  3501 MHz    9957535 s          0 s    1537686 s  857917848 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
