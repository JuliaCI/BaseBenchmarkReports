# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a8f1fcef97c70815e490ad96369a69c1c40551b2](https://github.com/JuliaLang/julia/commit/a8f1fcef97c70815e490ad96369a69c1c40551b2) vs [JuliaLang/julia@2390055133ac27ae7ff2ba11a42c11ef8221b3a8](https://github.com/JuliaLang/julia/commit/2390055133ac27ae7ff2ba11a42c11ef8221b3a8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18196#issuecomment-241790541)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.60 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","descending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",100)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",10)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",100)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","range",100)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.379
Commit a8f1fce (2016-08-23 16:17 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20286.7578125 MB free)
Uptime: 7.619514e6 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13401397 s          0 s    2343014 s  744472114 s         24 s
#2  3501 MHz   31932410 s          0 s    2011837 s  727158033 s          6 s
#3  3501 MHz   11729223 s          0 s    1468770 s  748346788 s         13 s
#4  3501 MHz    9227464 s          0 s    1422420 s  750958848 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.376
Commit 2390055 (2016-08-23 16:14 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19982.15234375 MB free)
Uptime: 7.624483e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13449299 s          0 s    2350417 s  744912155 s         24 s
#2  3501 MHz   32164047 s          0 s    2022786 s  727411592 s          6 s
#3  3501 MHz   11830872 s          0 s    1477303 s  748732702 s         13 s
#4  3501 MHz    9307734 s          0 s    1431302 s  751365992 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
