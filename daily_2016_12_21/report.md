# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a041e6edc21d62f29bcefb4d9f20599581674c70](https://github.com/JuliaLang/julia/commit/a041e6edc21d62f29bcefb4d9f20599581674c70)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a041e6edc21d62f29bcefb4d9f20599581674c70#commitcomment-20256289)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-12-21 vs 2016-12-20

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
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.31 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.11 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.15 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.85 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 0.99 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.52 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),2)]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.94 (15%)  | 0.55 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.94 (15%)  | 0.68 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.98 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.97 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 0.75 (45%)  | 0.84 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 0.60 (45%)  | 0.60 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 0.63 (45%)  | 0.33 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.81 (45%)  | 0.32 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 0.64 (45%)  | 0.33 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.81 (45%)  | 0.32 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.71 (45%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 0.84 (45%)  | 0.68 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.77 (45%)  | 0.72 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 0.87 (45%)  | 0.72 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_devec"]` | 1.00 (15%)  | 0.50 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.70 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigFloat}")]` | 4.50 (40%) :x: | Inf (1%) :x: |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 10.75 (40%) :x: | Inf (1%) :x: |
| `["shootout","nbody_vec"]` | 0.17 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 0.74 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.81 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.84 (30%)  | 0.54 (1%) :white_check_mark: |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 1.71 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 1.53 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1639
Commit a041e6e (2016-12-20 23:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9445.67578125 MB free)
Uptime: 1.7957378e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   28438650 s          0 s    4690863 s  1758970987 s         54 s
#2  3501 MHz   84175221 s          0 s    5706444 s  1702878215 s         20 s
#3  3501 MHz   24892031 s          0 s    3168156 s  1766858710 s         29 s
#4  3501 MHz   20976398 s          0 s    3081434 s  1771006717 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
