# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@50f30f48497425982129478ae616ad8f5f2eebe1](https://github.com/JuliaLang/julia/commit/50f30f48497425982129478ae616ad8f5f2eebe1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/50f30f48497425982129478ae616ad8f5f2eebe1#commitcomment-18683936)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-18 vs 2016-08-17

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
| `["array","cat",("hcat_setind",5)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 0.90 (30%)  | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 0.61 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 0.10 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 0.34 (30%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 0.17 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 0.28 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 0.13 (30%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 0.34 (30%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 0.17 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 0.26 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 0.29 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 0.13 (30%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 0.26 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.72 (25%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.72 (25%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.19 (15%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.58 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.56 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["shootout","nbody_vec"]` | 0.01 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 0.01 (15%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.02 (15%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.03 (15%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.272
Commit 50f30f4 (2016-08-18 03:18 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20090.44921875 MB free)
Uptime: 7.142643e6 sec
Load Avg:  1.0029296875  1.01220703125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11909046 s          0 s    2134140 s  698583034 s         23 s
#2  3501 MHz   28057271 s          0 s    1766103 s  683673789 s          6 s
#3  3501 MHz    9880532 s          0 s    1276024 s  702730569 s         12 s
#4  3501 MHz    7624737 s          0 s    1240664 s  705077228 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
