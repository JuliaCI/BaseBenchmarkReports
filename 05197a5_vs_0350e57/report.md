# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@05197a51fa015dfcbec05ddba9f2e2e2a2945150](https://github.com/JuliaLang/julia/commit/05197a51fa015dfcbec05ddba9f2e2e2a2945150) vs [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/05197a51fa015dfcbec05ddba9f2e2e2a2945150#commitcomment-18718047)

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
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 1.03 (30%)  | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.59 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 3.94 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 9.42 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 4.25 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 10.29 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 3.09 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 6.52 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 4.21 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 9.69 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 4.20 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 10.03 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.71 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 8.22 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 4.20 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 9.69 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 3.09 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 6.03 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 4.04 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 9.59 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 4.04 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 9.58 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.57 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 8.05 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 4.03 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 9.45 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.34 (25%) :x: | 1.02 (1%) :x: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.34 (25%) :x: | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 5.12 (15%) :x: | 1.19 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.47 (15%) :x: | 1.02 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.46 (15%) :x: | 1.01 (1%) :x: |
| `["shootout","nbody_vec"]` | 118.36 (15%) :x: | 5.40 (1%) :x: |
| `["simd",("sum_reduce","Float32",4096)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 68.96 (15%) :x: | 3.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 63.01 (15%) :x: | 2.74 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 33.89 (15%) :x: | 1.58 (1%) :x: |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 1.77 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc2+10
Commit 05197a5 (2016-08-20 06:40 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21175.7421875 MB free)
Uptime: 7.464487e6 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12320302 s          0 s    2213667 s  730214406 s         24 s
#2  3501 MHz   28995300 s          0 s    1872808 s  714756908 s          6 s
#3  3501 MHz   10288563 s          0 s    1337385 s  734430153 s         12 s
#4  3501 MHz    8233836 s          0 s    1305108 s  736578904 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-rc2+0
Commit 0350e57 (2016-08-12 11:25 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20915.31640625 MB free)
Uptime: 7.469168e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12367924 s          0 s    2220536 s  730626730 s         24 s
#2  3501 MHz   29197555 s          0 s    1880598 s  715014209 s          6 s
#3  3501 MHz   10401859 s          0 s    1347099 s  734774593 s         12 s
#4  3501 MHz    8308184 s          0 s    1311828 s  736965357 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
