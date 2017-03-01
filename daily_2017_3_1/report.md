# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b1242dff002bbc8d26815b727fc122c1eb8aec01](https://github.com/JuliaLang/julia/commit/b1242dff002bbc8d26815b727fc122c1eb8aec01)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b1242dff002bbc8d26815b727fc122c1eb8aec01#commitcomment-21099385)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-03-01 vs 2017-02-28

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
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.40 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.39 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",1024)]` | 2.00 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",256)]` | 2.29 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.98 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 2.29 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",1024)]` | 2.12 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",256)]` | 2.37 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 2.12 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 2.37 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Bidiagonal",1024)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.5
Commit b1242df (2017-02-28 18:33 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2972.703125 MB free)
Uptime: 2.3995857e7 sec
Load Avg:  0.92431640625  1.0  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   40988070 s          0 s    8573047 s  2343087792 s         69 s
#2  3501 MHz  149582828 s          0 s    5130712 s  2243478790 s          9 s
#3  3501 MHz   36804920 s          0 s    4505691 s  2357155115 s         50 s
#4  3501 MHz   34417163 s          0 s    4650790 s  2359385676 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
