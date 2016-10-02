# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@20b2ef9778e14d33d9c0698aa0d4835f4c3214da](https://github.com/JuliaLang/julia/commit/20b2ef9778e14d33d9c0698aa0d4835f4c3214da)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/20b2ef9778e14d33d9c0698aa0d4835f4c3214da#commitcomment-19258011)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-10-02 vs 2016-10-01

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 1.94 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 2.71 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 2.74 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 1.94 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 2.71 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 2.73 (40%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","BigInt")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Float32")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","descending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 1.93 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.77 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 1.29 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.853
Commit 20b2ef9 (2016-10-02 02:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16867.40625 MB free)
Uptime: 1.1030999e7 sec
Load Avg:  1.0029296875  1.013671875  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17783767 s          0 s    3012672 s  1079988455 s         34 s
#2  3501 MHz   44614497 s          0 s    3264543 s  1053659493 s         11 s
#3  3501 MHz   15492481 s          0 s    1988462 s  1085082800 s         17 s
#4  3501 MHz   13111461 s          0 s    1942978 s  1087606176 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
