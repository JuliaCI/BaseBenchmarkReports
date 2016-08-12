# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f9fb4dae619ce2f9e7b3aa466b27e4c4f6aff11b](https://github.com/JuliaLang/julia/commit/f9fb4dae619ce2f9e7b3aa466b27e4c4f6aff11b) vs [JuliaLang/julia@2d24eda52727c6cbccec935d689d84d710366f5a](https://github.com/JuliaLang/julia/commit/2d24eda52727c6cbccec935d689d84d710366f5a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f9fb4dae619ce2f9e7b3aa466b27e4c4f6aff11b#commitcomment-18620222)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.70 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("prerend!",2048)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.85 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.86 (15%) :x: | 1.01 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.53 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ascending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,10000))]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.81 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float32)]` | 1.43 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.33
Commit f9fb4da (2016-08-05 16:40 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18757.0625 MB free)
Uptime: 6.646708e6 sec
Load Avg:  0.9619140625  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   10199569 s          0 s    2200069 s  650354839 s         22 s
#2  3501 MHz   25609185 s          0 s    1279579 s  637317475 s          3 s
#3  3501 MHz    9215412 s          0 s    1155114 s  653986725 s         12 s
#4  3501 MHz    7530954 s          0 s    1129782 s  655687805 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.28
Commit 2d24eda (2016-08-05 15:28 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18582.99609375 MB free)
Uptime: 6.651683e6 sec
Load Avg:  0.99560546875  1.017578125  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   10313755 s          0 s    2210138 s  650726682 s         22 s
#2  3501 MHz   25864772 s          0 s    1291574 s  637546969 s          3 s
#3  3501 MHz    9267888 s          0 s    1161064 s  654425002 s         12 s
#4  3501 MHz    7572830 s          0 s    1135730 s  656136892 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
