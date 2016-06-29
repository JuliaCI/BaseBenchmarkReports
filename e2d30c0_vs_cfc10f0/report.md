# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e2d30c0fec397a97a522df6eda045cf6a393c01d](https://github.com/JuliaLang/julia/commit/e2d30c0fec397a97a522df6eda045cf6a393c01d) vs [JuliaLang/julia@cfc10f07431f5c762d4531333864b245a038480d](https://github.com/JuliaLang/julia/commit/cfc10f07431f5c762d4531333864b245a038480d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16622#issuecomment-229251598)

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
| `["array","cat",("catnd",5)]` | 1.79 (15%) :x: | 1.13 (1%) :x: |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",2)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.70 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 2.31 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 2.09 (25%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem","spellcheck"]` | 1.16 (15%) :x: | 1.26 (1%) :x: |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.85 (15%)  | 1.01 (1%) :x: |
| `["simd",("sum_reduce","Float32",4095)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.19 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5007
Commit e2d30c0 (2016-06-29 02:36 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (23990.875 MB free)
Uptime: 2.823303e6 sec
Load Avg:  1.0830078125  1.03125  0.98681640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3154128 s          0 s     790580 s  277653840 s         11 s
#2  3501 MHz    9920182 s          0 s     533817 s  271701077 s          1 s
#3  3501 MHz    3863422 s          0 s     501050 s  277818336 s          2 s
#4  3501 MHz    3245937 s          0 s     488534 s  278440524 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4992
Commit cfc10f0 (2016-06-29 01:57 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (23898.765625 MB free)
Uptime: 2.827862e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3284869 s          0 s     801104 s  277967220 s         11 s
#2  3501 MHz   10139542 s          0 s     541704 s  271929331 s          1 s
#3  3501 MHz    3896583 s          0 s     505969 s  278235338 s          2 s
#4  3501 MHz    3289729 s          0 s     494310 s  278846302 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
