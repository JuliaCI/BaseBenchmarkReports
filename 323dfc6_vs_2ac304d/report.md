# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@323dfc62f43097e67c9f39e22af449d75a16203e](https://github.com/JuliaLang/julia/commit/323dfc62f43097e67c9f39e22af449d75a16203e) vs [JuliaLang/julia@2ac304dfba75fad148d4070ef4f8a2e400c305bb](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16980#issuecomment-226716415)

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
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",1024)]` | 2.66 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 2.57 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","BigInt")]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ones")]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.30 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.4.6-pre+74
Commit 323dfc6 (2016-06-17 08:43 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27474.40625 MB free)
Uptime: 1.802786e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1244008 s          0 s     361994 s  178261953 s          5 s
#2  3501 MHz    3388912 s          0 s     295799 s  176443299 s          1 s
#3  3501 MHz    1489921 s          0 s     248480 s  178431802 s          2 s
#4  3501 MHz     951640 s          0 s     217464 s  179029539 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

#### Comparison Build

```
Julia Version 0.4.5
Commit 2ac304d (2016-03-18 00:58 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27283.5390625 MB free)
Uptime: 1.806038e6 sec
Load Avg:  1.0029296875  1.0146484375  1.0478515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1282626 s          0 s     368241 s  178540930 s          5 s
#2  3501 MHz    3578888 s          0 s     302306 s  176571237 s          1 s
#3  3501 MHz    1588081 s          0 s     256030 s  178650483 s          2 s
#4  3501 MHz     995786 s          0 s     223192 s  179304162 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
