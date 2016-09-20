# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b87a416f6b0f988486406f95fad649bc1cc707e1](https://github.com/JuliaLang/julia/commit/b87a416f6b0f988486406f95fad649bc1cc707e1) vs [JuliaLang/julia@d7a703f521fff9f81d2a7aef007d582936169a90](https://github.com/JuliaLang/julia/commit/d7a703f521fff9f81d2a7aef007d582936169a90)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18591#issuecomment-248218342)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(false)")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(1)")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Complex{Float64}")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 1.34 (20%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.50 (40%) :x: | 1.00 (1%)  |

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
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
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
Julia Version 0.6.0-dev.713
Commit b87a416 (2016-09-20 04:49 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16096.4375 MB free)
Uptime: 1.0004566e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16799355 s          0 s    3484888 s  977318905 s         32 s
#2  3501 MHz   44109409 s          0 s    2181385 s  953511458 s          4 s
#3  3501 MHz   15422158 s          0 s    1906175 s  982648034 s         20 s
#4  3501 MHz   13214001 s          0 s    1914723 s  984830016 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.711
Commit d7a703f (2016-09-20 04:48 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15939.3828125 MB free)
Uptime: 1.0009255e7 sec
Load Avg:  1.05908203125  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16845629 s          0 s    3492230 s  977732473 s         32 s
#2  3501 MHz   44301217 s          0 s    2187552 s  953781870 s          4 s
#3  3501 MHz   15534165 s          0 s    1915619 s  982994806 s         20 s
#4  3501 MHz   13302255 s          0 s    1922692 s  985202205 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
