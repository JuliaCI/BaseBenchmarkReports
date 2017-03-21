# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3b78b950d132f05b334a327ee2d90a18e92b8e5c](https://github.com/JuliaLang/julia/commit/3b78b950d132f05b334a327ee2d90a18e92b8e5c) vs [JuliaLang/julia@90cfb8292c5d8cdd25eb4b4653c03f6d382b42b1](https://github.com/JuliaLang/julia/commit/90cfb8292c5d8cdd25eb4b4653c03f6d382b42b1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21075#issuecomment-287974226)

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
| `["array","cat",("catnd",5)]` | 1.05 (15%)  | 1.02 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 1.27 (15%) :x: | 1.04 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:0.00010001000100010001:2.0")]` | 2.42 (50%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 2.41 (50%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumvector","100000:-1:1")]` | 2.23 (50%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumvector","1:100000")]` | 2.42 (50%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumvector_view","1.0:0.00010001000100010001:2.0")]` | 2.58 (50%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumvector_view","1.0:1.0:100000.0")]` | 2.58 (50%) :x: | 1.06 (1%) :x: |
| `["array","index",("sumvector_view","100000:-1:1")]` | 2.20 (50%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumvector_view","1:100000")]` | 2.58 (50%) :x: | 1.07 (1%) :x: |
| `["array","reductions",("mean","Float64")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 10.49 (15%) :x: | 1.01 (1%)  |
| `["problem","go","go_game"]` | 1.13 (15%)  | 1.02 (1%) :x: |
| `["problem","stockcorr","stockcorr"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.05 (30%)  | 1.01 (1%) :x: |
| `["sparse","index",("spmat","col","logical",10)]` | 1.73 (30%) :x: | 1.02 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 1.43 (30%) :x: | 1.01 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 1.71 (30%) :x: | 1.02 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","sparse"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
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
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.alpha.214
Commit 3b78b95 (2017-03-21 03:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7804.56640625 MB free)
Uptime: 2.5722776e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53526588 s          0 s    8311334 s  2504948895 s         77 s
#2  3501 MHz  194727220 s          0 s    8923755 s  2364453792 s         27 s
#3  3501 MHz   44504286 s          0 s    5218160 s  2521393335 s         41 s
#4  3501 MHz   40231921 s          0 s    5155306 s  2525964852 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.206
Commit 90cfb82 (2017-03-21 03:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7570.38671875 MB free)
Uptime: 2.5729104e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53605778 s          0 s    8321665 s  2505489894 s         77 s
#2  3501 MHz  195302286 s          0 s    8932625 s  2364502092 s         27 s
#3  3501 MHz   44601428 s          0 s    5226716 s  2521919723 s         41 s
#4  3501 MHz   40318310 s          0 s    5163346 s  2526502758 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
