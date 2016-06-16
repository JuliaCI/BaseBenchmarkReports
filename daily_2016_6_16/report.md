# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3f4e1e7274993b32b4dab8bdabdc9b645993923c](https://github.com/JuliaLang/julia/commit/3f4e1e7274993b32b4dab8bdabdc9b645993923c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3f4e1e7274993b32b4dab8bdabdc9b645993923c#commitcomment-17889396)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-16 vs 2016-06-15

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
| `["parallel","remotecall",("identity",1024)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4805
Commit 3f4e1e7 (2016-06-16 01:29 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27345.60546875 MB free)
Uptime: 1.699427e6 sec
Load Avg:  1.0029296875  1.00927734375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1598320 s          0 s     435699 s  167477421 s          5 s
#2  3501 MHz    4972374 s          0 s     297588 s  164568720 s          1 s
#3  3501 MHz    2281448 s          0 s     301156 s  167264279 s          1 s
#4  3501 MHz    1875136 s          0 s     275775 s  167702456 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
