# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d495c957653bca936a79fa66e71ae046ee259f99](https://github.com/JuliaLang/julia/commit/d495c957653bca936a79fa66e71ae046ee259f99) vs [JuliaLang/julia@0524a52165e617125893d5bcbf91bf8b7f4d6cf1](https://github.com/JuliaLang/julia/commit/0524a52165e617125893d5bcbf91bf8b7f4d6cf1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16851#issuecomment-233723661)

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
| `["array","cat",("catnd",5)]` | 0.73 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","blas","gbmv!"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","gbmv"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","gemv!"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","gemv"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","ger!"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","symv!"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","symv"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","syr!"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","trsv!"]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["linalg","blas","trsv"]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","descending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5513
Commit d495c95 (2016-07-19 18:29 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17961.4765625 MB free)
Uptime: 4.602938e6 sec
Load Avg:  1.0029296875  1.0078125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6279712 s          0 s    1401444 s  451381949 s         17 s
#2  3501 MHz   16963496 s          0 s     866859 s  442192020 s          2 s
#3  3501 MHz    6253168 s          0 s     795148 s  453025372 s          8 s
#4  3501 MHz    5326512 s          0 s     800047 s  453927047 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5510
Commit 0524a52 (2016-07-19 18:28 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17815.33203125 MB free)
Uptime: 4.607574e6 sec
Load Avg:  1.00439453125  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6323270 s          0 s    1407888 s  451794125 s         17 s
#2  3501 MHz   17245115 s          0 s     876795 s  442363569 s          2 s
#3  3501 MHz    6319150 s          0 s     802119 s  453415143 s          8 s
#4  3501 MHz    5369011 s          0 s     806350 s  454341171 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
