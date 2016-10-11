# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@29a29f94952abfc2e627aa8e6474e86350ca3a54](https://github.com/JuliaLang/julia/commit/29a29f94952abfc2e627aa8e6474e86350ca3a54) vs [JuliaLang/julia@496dd4041576c33a7568e2617f9906251220b73f](https://github.com/JuliaLang/julia/commit/496dd4041576c33a7568e2617f9906251220b73f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18444#issuecomment-252882365)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.97 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.55 (45%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Complex{Float64}")]` | 1.51 (45%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.52 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.71 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.935
Commit 29a29f9 (2016-10-11 06:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16338.6484375 MB free)
Uptime: 1.1834869e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18670324 s          0 s    4018084 s  1157425751 s         36 s
#2  3501 MHz   51230357 s          0 s    2522303 s  1128978719 s          5 s
#3  3501 MHz   17530772 s          0 s    2192192 s  1163200617 s         24 s
#4  3501 MHz   15151115 s          0 s    2208664 s  1165543851 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.928
Commit 496dd40 (2016-10-11 01:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15852.53515625 MB free)
Uptime: 1.1841427e7 sec
Load Avg:  0.9228515625  0.998046875  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18726831 s          0 s    4025626 s  1158015298 s         36 s
#2  3501 MHz   51614841 s          0 s    2533718 s  1129238099 s          5 s
#3  3501 MHz   17584035 s          0 s    2199395 s  1163795120 s         24 s
#4  3501 MHz   15277704 s          0 s    2218586 s  1166062594 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
