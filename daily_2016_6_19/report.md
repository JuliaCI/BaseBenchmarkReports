# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@11d5ae0f0cd9ac59aa9f7c2d8c19c75342af4dfd](https://github.com/JuliaLang/julia/commit/11d5ae0f0cd9ac59aa9f7c2d8c19c75342af4dfd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/11d5ae0f0cd9ac59aa9f7c2d8c19c75342af4dfd#commitcomment-17925074)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-19 vs 2016-06-18

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
| `["array","index",("sumcolon","100000000:-1:1")]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 1.62 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 1.51 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 0.94 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 0.88 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.92 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.87 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.93 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.98 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.93 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.92 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.94 (40%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.93 (40%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.88 (40%)  | 0.99 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 21.98 (15%) :x: | 1.24 (1%) :x: |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","random")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4863
Commit 11d5ae0 (2016-06-19 03:00 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (26772.00390625 MB free)
Uptime: 1.958642e6 sec
Load Avg:  1.00732421875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2480621 s          0 s     577678 s  192297635 s          5 s
#2  3501 MHz    8277946 s          0 s     423722 s  187038604 s          1 s
#3  3501 MHz    3394509 s          0 s     417945 s  191935844 s          1 s
#4  3501 MHz    2747860 s          0 s     385872 s  192622574 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
