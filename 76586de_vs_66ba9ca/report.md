# Benchmark Report

## Job Properties

*Commit(s):* [Sacha0/julia@76586dedc46ca0beb75cf36c5a98af396517995a](https://github.com/Sacha0/julia/commit/76586dedc46ca0beb75cf36c5a98af396517995a) vs [JuliaLang/julia@66ba9caba2f0933f932cbf094f6b06dc37934598](https://github.com/JuliaLang/julia/commit/66ba9caba2f0933f932cbf094f6b06dc37934598)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19540#issuecomment-266884637)

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
| `["array","index","5d"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("var","Float64")]` | 1.69 (15%) :x: | 1.25 (1%) :x: |
| `["array","reductions",("var","Int64")]` | 1.21 (15%) :x: | 1.22 (1%) :x: |
| `["array","setindex!",("setindex!",1)]` | 1.27 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 1.34 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 1.32 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 1.30 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 1.31 (15%) :x: | 1.09 (1%) :x: |
| `["dates","parse","Date"]` | 1.05 (15%)  | 1.02 (1%) :x: |
| `["dates","parse","DateTime"]` | 1.04 (15%)  | 1.02 (1%) :x: |
| `["dates","string","Date"]` | 1.98 (15%) :x: | 1.10 (1%) :x: |
| `["dates","string","DateTime"]` | 1.76 (15%) :x: | 1.12 (1%) :x: |
| `["misc","parse","DateTime"]` | 1.08 (15%)  | 1.02 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["problem","go","go_game"]` | 1.88 (15%) :x: | 1.22 (1%) :x: |
| `["problem","json","parse_json"]` | 1.75 (15%) :x: | 1.21 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.47 (15%) :x: | 1.13 (1%) :x: |
| `["scalar","floatexp",("exponent","norm","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["shootout","nbody"]` | 1.00 (15%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.01 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 1.01 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 0.95 (30%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.93 (30%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 0.99 (30%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 0.98 (30%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.00 (30%)  | 1.25 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 0.99 (30%)  | 1.25 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.01 (30%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.02 (30%)  | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","ascending")]` | 1.66 (30%) :x: | 1.33 (1%) :x: |
| `["sort","issorted",("reverse","descending")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","issorted",("reverse","ones")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","issorted",("reverse","random")]` | 1.63 (30%) :x: | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.89 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.89 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.02 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.01 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 0.98 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 0.99 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.00 (30%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 0.99 (30%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 1.00 (30%)  | 1.25 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.01 (30%)  | 1.25 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 1.00 (30%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 0.99 (30%)  | 1.20 (1%) :x: |
| `["sparse","index",("spmat","col","array",10)]` | 0.98 (30%)  | 1.01 (1%) :x: |
| `["sparse","index",("spmat","col","logical",10)]` | 1.64 (30%) :x: | 1.02 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 1.36 (30%) :x: | 1.01 (1%)  |

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
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1558
Commit 76586de (2016-12-13 22:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14022.9609375 MB free)
Uptime: 1.7320284e7 sec
Load Avg:  1.021484375  1.0234375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22879363 s          0 s    5502058 s  1698691238 s         54 s
#2  3501 MHz   70118786 s          0 s    3319309 s  1657554844 s          8 s
#3  3501 MHz   22477638 s          0 s    2897177 s  1705853403 s         33 s
#4  3501 MHz   19507461 s          0 s    2925259 s  1708787380 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1556
Commit 66ba9ca (2016-12-13 11:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13828.8671875 MB free)
Uptime: 1.7326178e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22912067 s          0 s    5508699 s  1699239131 s         54 s
#2  3501 MHz   70440901 s          0 s    3327330 s  1657813545 s          8 s
#3  3501 MHz   22627230 s          0 s    2908238 s  1706281444 s         33 s
#4  3501 MHz   19560822 s          0 s    2931806 s  1709316197 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
