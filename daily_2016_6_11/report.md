# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@feb911727c106074d295336143977832a935ebbd](https://github.com/JuliaLang/julia/commit/feb911727c106074d295336143977832a935ebbd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/feb911727c106074d295336143977832a935ebbd#commitcomment-17831378)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-11 vs 2016-06-10

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
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 0.98 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.97 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["shootout","binary_trees"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 4.75 (15%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4096)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float64",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float64",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Int32",4096)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Int64",4095)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Int64",4096)]` | 0.72 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 0.59 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.31 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4668
Commit feb9117 (2016-06-11 03:59 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27588.015625 MB free)
Uptime: 1.267451e6 sec
Load Avg:  1.025390625  1.0234375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     421941 s          0 s     209449 s  125818624 s          3 s
#2  3501 MHz    1152943 s          0 s     144895 s  125359512 s          0 s
#3  3501 MHz     306502 s          0 s     123135 s  126238532 s          1 s
#4  3501 MHz     282560 s          0 s     109730 s  126297416 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
