# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a0d75a49ceb6ea31b64fc85707916dc0b3e9300e](https://github.com/JuliaLang/julia/commit/a0d75a49ceb6ea31b64fc85707916dc0b3e9300e) vs [JuliaLang/julia@b80dad40ab36bcd7e11859d36b51c6afcf008148](https://github.com/JuliaLang/julia/commit/b80dad40ab36bcd7e11859d36b51c6afcf008148)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a0d75a49ceb6ea31b64fc85707916dc0b3e9300e#commitcomment-18655244)

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
| `["array","cat",("catnd",5)]` | 0.89 (15%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumeach","100000000:-1:1")]` | 2.07 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000000")]` | 6.50 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","1:100000000")]` | 8.67 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 2.07 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000000")]` | 6.75 (40%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.56 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.56 (15%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 1.05 (30%)  | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.60 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 3.93 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 9.36 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 4.14 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 9.96 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 3.01 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 5.94 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 4.13 (30%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 9.32 (30%) :x: | 1.25 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 3.99 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 9.05 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.58 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 7.88 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 4.01 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 9.13 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 2.96 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 6.00 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 4.14 (30%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 9.67 (30%) :x: | 1.25 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 4.00 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 9.06 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.55 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 7.76 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 4.02 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 9.09 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.31 (25%) :x: | 1.02 (1%) :x: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.31 (25%) :x: | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 5.17 (15%) :x: | 1.19 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.58 (15%) :x: | 1.02 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.59 (15%) :x: | 1.01 (1%) :x: |
| `["shootout","nbody_vec"]` | 115.21 (15%) :x: | 5.40 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 64.24 (15%) :x: | 3.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 63.03 (15%) :x: | 2.74 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 31.90 (15%) :x: | 1.58 (1%) :x: |

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
Julia Version 0.6.0-dev.225
Commit a0d75a4 (2016-08-15 18:56 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18184.9921875 MB free)
Uptime: 7.002448e6 sec
Load Avg:  1.0029296875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11061078 s          0 s    2333678 s  684844193 s         22 s
#2  3501 MHz   27905792 s          0 s    1390667 s  670459915 s          3 s
#3  3501 MHz    9739724 s          0 s    1234409 s  688936002 s         12 s
#4  3501 MHz    8276973 s          0 s    1225490 s  690398736 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.212
Commit b80dad4 (2016-08-14 17:12 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18035.65625 MB free)
Uptime: 7.007113e6 sec
Load Avg:  1.00634765625  1.0146484375  0.96728515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11093133 s          0 s    2340051 s  685270784 s         22 s
#2  3501 MHz   28190594 s          0 s    1401272 s  670630552 s          3 s
#3  3501 MHz    9800566 s          0 s    1240931 s  689334318 s         12 s
#4  3501 MHz    8335404 s          0 s    1233229 s  690798473 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
