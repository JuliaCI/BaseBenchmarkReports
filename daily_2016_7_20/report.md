# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ee5e23116e8c4bef9607512179f9f900b99cce65](https://github.com/JuliaLang/julia/commit/ee5e23116e8c4bef9607512179f9f900b99cce65)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ee5e23116e8c4bef9607512179f9f900b99cce65#commitcomment-18310251)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-07-20 vs 2016-07-19

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
| `["array","index",("sumcolon","100000000:-1:1")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 1.64 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 1.01 (40%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000000:-1:1")]` | 0.93 (40%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000000")]` | 0.92 (40%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 1.01 (40%)  | 0.95 (1%) :white_check_mark: |
| `["array","setindex!",("setindex!",3)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.45 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.36 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.48 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.32 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.75 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.52 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.74 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.51 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.73 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.51 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["shootout","revcomp"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5539
Commit ee5e231 (2016-07-20 03:53 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17925.671875 MB free)
Uptime: 4.63708e6 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6382907 s          0 s    1418023 s  454667744 s         17 s
#2  3501 MHz   17445725 s          0 s     885994 s  445102351 s          2 s
#3  3501 MHz    6367537 s          0 s     809563 s  456307910 s          8 s
#4  3501 MHz    5494767 s          0 s     817445 s  457153159 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
