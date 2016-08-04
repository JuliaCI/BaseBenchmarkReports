# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@40d298f5859e68414ea59a31674ba21f9b3b4185](https://github.com/JuliaLang/julia/commit/40d298f5859e68414ea59a31674ba21f9b3b4185)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/40d298f5859e68414ea59a31674ba21f9b3b4185#commitcomment-18514089)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-04 vs 2016-08-03

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
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 1.13 (30%)  | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.63 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 4.08 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 9.77 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 4.30 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 10.48 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 3.14 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 6.47 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 4.03 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 9.45 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 4.04 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 9.54 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.61 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 8.18 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 4.03 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 9.48 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 3.00 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 6.22 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 4.00 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 9.38 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 4.01 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 9.47 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.58 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 8.07 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 3.99 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 9.37 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.39 (25%) :x: | 1.02 (1%) :x: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.39 (25%) :x: | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 5.06 (15%) :x: | 1.19 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.10 (15%)  | 1.01 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.44 (15%) :x: | 1.01 (1%) :x: |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 119.10 (15%) :x: | 5.40 (1%) :x: |
| `["sort","issorted",("forwards","descending")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 67.57 (15%) :x: | 3.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 61.58 (15%) :x: | 2.74 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 33.57 (15%) :x: | 1.58 (1%) :x: |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc0+192
Commit 40d298f (2016-08-04 03:38 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (30953.7421875 MB free)
Uptime: 5.933355e6 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    7547247 s          0 s    1796362 s  582315423 s         19 s
#2  3501 MHz   21210011 s          0 s    1091952 s  570625779 s          2 s
#3  3501 MHz    7756433 s          0 s     995457 s  584301231 s         10 s
#4  3501 MHz    6362322 s          0 s     971315 s  585710454 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
