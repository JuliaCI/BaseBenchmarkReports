# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@ca6f4a9cfeb359d0babbac03c9214e3a27d07393](https://github.com/pabloferz/julia/commit/ca6f4a9cfeb359d0babbac03c9214e3a27d07393) vs [JuliaLang/julia@16ad3a4931d354ae5621f039cd55df2dee43edcf](https://github.com/JuliaLang/julia/commit/16ad3a4931d354ae5621f039cd55df2dee43edcf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17798#issuecomment-237412910)

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
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.84 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.94 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.98 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.88 (15%)  | 0.95 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.94 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.98 (15%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 0.27 (30%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 0.54 (30%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 0.23 (30%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 0.51 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 0.23 (30%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 0.51 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 0.51 (30%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 0.23 (30%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 0.51 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 0.27 (30%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 0.54 (30%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 0.52 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 0.07 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 0.07 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 0.53 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 0.25 (30%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 0.51 (30%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 0.07 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 0.24 (30%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 0.52 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.82 (15%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.26 (15%) :white_check_mark: | 0.48 (1%) :white_check_mark: |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.96 (15%)  | 0.94 (1%) :white_check_mark: |

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
Julia Version 0.5.0-rc0+181
Commit ca6f4a9 (2016-08-04 00:01 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (30912.99609375 MB free)
Uptime: 5.919507e6 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    7386397 s          0 s    1777122 s  581155447 s         19 s
#2  3501 MHz   20757238 s          0 s    1068357 s  569768521 s          2 s
#3  3501 MHz    7599188 s          0 s     980619 s  583093095 s         10 s
#4  3501 MHz    6265020 s          0 s     959890 s  584436112 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-rc0+179
Commit 16ad3a4 (2016-08-03 23:58 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (31005.4375 MB free)
Uptime: 5.924431e6 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    7501835 s          0 s    1787434 s  581501436 s         19 s
#2  3501 MHz   21004894 s          0 s    1080952 s  569975410 s          2 s
#3  3501 MHz    7634525 s          0 s     986236 s  583542229 s         10 s
#4  3501 MHz    6300486 s          0 s     965158 s  584887017 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
