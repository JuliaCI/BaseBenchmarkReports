# Benchmark Report

## Job Properties

*Commit(s):* [martinholters/julia@f1726eccdbf22592066da40513eefff8ca25ccbf](https://github.com/martinholters/julia/commit/f1726eccdbf22592066da40513eefff8ca25ccbf) vs [JuliaLang/julia@efa23adbbefca173290c3fafe35ebde8e7f8fe6a](https://github.com/JuliaLang/julia/commit/efa23adbbefca173290c3fafe35ebde8e7f8fe6a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17313#issuecomment-231324395)

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
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 1.04 (30%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 1.58 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 1.05 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 1.89 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 1.03 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 1.96 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 1.05 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.70 (30%) :x: | 1.04 (1%) :x: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 1.06 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 2.00 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 1.07 (30%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.75 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 1.12 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 2.07 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 1.13 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 2.00 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 1.09 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.78 (30%) :x: | 1.04 (1%) :x: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 1.10 (30%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 2.07 (30%) :x: | 1.06 (1%) :x: |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 8.67 (15%) :x: | 1.53 (1%) :x: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","random")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5232
Commit f1726ec (2016-07-08 10:01 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20957.78515625 MB free)
Uptime: 3.622491e6 sec
Load Avg:  0.9169921875  0.96875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    4753931 s          0 s    1084582 s  355446942 s         13 s
#2  3501 MHz   13244762 s          0 s     690193 s  348098277 s          2 s
#3  3501 MHz    4619811 s          0 s     610256 s  356843824 s          4 s
#4  3501 MHz    4224760 s          0 s     629436 s  357202258 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5230
Commit efa23ad (2016-07-08 09:18 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20817.17578125 MB free)
Uptime: 3.627027e6 sec
Load Avg:  1.0439453125  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    4856654 s          0 s    1093393 s  355787660 s         13 s
#2  3501 MHz   13457462 s          0 s     697562 s  348331233 s          2 s
#3  3501 MHz    4684977 s          0 s     617504 s  357224124 s          5 s
#4  3501 MHz    4268543 s          0 s     635361 s  357605565 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
