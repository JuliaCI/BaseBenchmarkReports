# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3de00078c67f3ef423602d8e183fc109a1d9ee09](https://github.com/JuliaLang/julia/commit/3de00078c67f3ef423602d8e183fc109a1d9ee09) vs [JuliaLang/julia@9b83cd695bb6ad612fcdf7f0b41127bb6f312069](https://github.com/JuliaLang/julia/commit/9b83cd695bb6ad612fcdf7f0b41127bb6f312069)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18413#issuecomment-246604162)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 1.22 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 1.24 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 1.26 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 1.21 (15%) :x: | 1.09 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 1.36 (15%) :x: | 1.09 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 0.99 (15%)  | 1.02 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 0.98 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 0.98 (15%)  | 1.02 (1%) :x: |
| `["problem","json","parse_json"]` | 1.73 (15%) :x: | 1.21 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.50 (15%) :x: | 1.13 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 1.79 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.609
Commit 3de0007 (2016-09-12 15:56 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17053.10546875 MB free)
Uptime: 9.403446e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15380250 s          0 s    3238861 s  919037778 s         29 s
#2  3501 MHz   39814775 s          0 s    1993062 s  897919730 s          4 s
#3  3501 MHz   14077452 s          0 s    1744931 s  924073546 s         18 s
#4  3501 MHz   12117434 s          0 s    1758794 s  926005132 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.601
Commit 9b83cd6 (2016-09-12 11:20 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16876.5625 MB free)
Uptime: 9.408069e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15414958 s          0 s    3244586 s  919458097 s         29 s
#2  3501 MHz   40077629 s          0 s    2002855 s  898108984 s          4 s
#3  3501 MHz   14168854 s          0 s    1753074 s  924435570 s         18 s
#4  3501 MHz   12159997 s          0 s    1765722 s  926417362 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
