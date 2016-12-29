# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1d187c800ae9b150ba0fd5a2464163b36f18347f](https://github.com/JuliaLang/julia/commit/1d187c800ae9b150ba0fd5a2464163b36f18347f) vs [JuliaLang/julia@99fcb5bad6457b9cdd12f158a34300a1202429a0](https://github.com/JuliaLang/julia/commit/99fcb5bad6457b9cdd12f158a34300a1202429a0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19746#issuecomment-269577868)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","5d"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 1.37 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 2.30 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 2.16 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 2.01 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 1.98 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 2.35 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 2.09 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 1.94 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.77 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 2.06 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 2.36 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 1.77 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 1.73 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.34 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 2.34 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 2.13 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 1.99 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 2.03 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 2.34 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 2.00 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 1.99 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.76 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 1.96 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 2.29 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 2.16 (45%) :x: | 1.02 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1748
Commit 1d187c8 (2016-12-29 04:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5891.0625 MB free)
Uptime: 1.8639356e7 sec
Load Avg:  1.01318359375  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25390171 s          0 s    6001304 s  1827212884 s         59 s
#2  3501 MHz   80600687 s          0 s    3650994 s  1778573484 s          8 s
#3  3501 MHz   24455656 s          0 s    3153648 s  1835468718 s         38 s
#4  3501 MHz   22019730 s          0 s    3245190 s  1837792926 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1742
Commit 99fcb5b (2016-12-29 03:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5492.953125 MB free)
Uptime: 1.864562e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25453437 s          0 s    6009621 s  1827765741 s         59 s
#2  3501 MHz   80946339 s          0 s    3657239 s  1778847365 s          8 s
#3  3501 MHz   24497415 s          0 s    3159806 s  1836046413 s         38 s
#4  3501 MHz   22164690 s          0 s    3256020 s  1838263122 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
