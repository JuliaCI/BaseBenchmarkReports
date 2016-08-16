# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1c700920119b4e7c55efced770f598bff5470af9](https://github.com/JuliaLang/julia/commit/1c700920119b4e7c55efced770f598bff5470af9) vs [JuliaLang/julia@b80dad40ab36bcd7e11859d36b51c6afcf008148](https://github.com/JuliaLang/julia/commit/b80dad40ab36bcd7e11859d36b51c6afcf008148)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/1c700920119b4e7c55efced770f598bff5470af9#commitcomment-18658120)

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
| `["array","cat",("catnd",5)]` | 0.93 (15%)  | 0.94 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","100000000:-1:1")]` | 2.14 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000000")]` | 6.75 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","1:100000000")]` | 8.67 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 2.31 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000000")]` | 6.75 (40%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.61 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.61 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 1.08 (30%)  | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.58 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 3.99 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 9.42 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 4.16 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 9.95 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 2.93 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 5.67 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 3.91 (30%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 9.24 (30%) :x: | 1.25 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 3.85 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 9.08 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.47 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 7.81 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 3.85 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 8.96 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 2.88 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 6.01 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 3.98 (30%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 9.38 (30%) :x: | 1.25 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 3.88 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 9.30 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.49 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 7.92 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 3.89 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 9.07 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.29 (25%) :x: | 1.02 (1%) :x: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.29 (25%) :x: | 1.02 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 5.14 (15%) :x: | 1.19 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 1.77 (15%) :x: | 1.02 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.85 (15%) :x: | 1.01 (1%) :x: |
| `["problem","monte carlo","euro_option_vec"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 119.48 (15%) :x: | 5.40 (1%) :x: |
| `["shootout","pidigits"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","descending")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 68.07 (15%) :x: | 3.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 60.61 (15%) :x: | 2.74 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 35.18 (15%) :x: | 1.58 (1%) :x: |

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
Julia Version 0.6.0-dev.223
Commit 1c70092 (2016-08-15 18:40 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18148.18359375 MB free)
Uptime: 7.013336e6 sec
Load Avg:  1.0029296875  1.0146484375  0.955078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11223020 s          0 s    2351542 s  685749885 s         22 s
#2  3501 MHz   28417868 s          0 s    1411360 s  671014998 s          3 s
#3  3501 MHz    9853458 s          0 s    1247455 s  689896422 s         13 s
#4  3501 MHz    8392727 s          0 s    1240220 s  691355817 s          2 s

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
Memory: 31.383651733398438 GB (18016.828125 MB free)
Uptime: 7.018005e6 sec
Load Avg:  0.9228515625  0.96875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11300990 s          0 s    2359694 s  686129267 s         22 s
#2  3501 MHz   28604848 s          0 s    1418674 s  671287218 s          3 s
#3  3501 MHz    9888473 s          0 s    1253250 s  690321787 s         13 s
#4  3501 MHz    8528382 s          0 s    1250523 s  691676425 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
