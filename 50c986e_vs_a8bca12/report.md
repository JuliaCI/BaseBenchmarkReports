# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@50c986e91c665a80565a5d8dcade92de38d545e0](https://github.com/JuliaLang/julia/commit/50c986e91c665a80565a5d8dcade92de38d545e0) vs [JuliaLang/julia@a8bca12667401757da552f9a74feec198ac21f7e](https://github.com/JuliaLang/julia/commit/a8bca12667401757da552f9a74feec198ac21f7e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17137#issuecomment-230965839)

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
| `["array","bool","bitarray_bool_load!"]` | 1.59 (15%) :x: | 1.00 (1%)  |
| `["array","bool","bitarray_true_load!"]` | 1.94 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 2.07 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 2.17 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 2.08 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 2.16 (30%) :x: | 1.00 (1%)  |
| `["problem","spellcheck"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 0.97 (15%)  | 1.01 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",100)]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5198
Commit 50c986e (2016-07-07 02:50 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21283.68359375 MB free)
Uptime: 3.509732e6 sec
Load Avg:  1.0830078125  1.0185546875  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3611927 s          0 s     810232 s  345764051 s         11 s
#2  3501 MHz    9782520 s          0 s     695988 s  340180140 s          4 s
#3  3501 MHz    3688156 s          0 s     548740 s  346532914 s          3 s
#4  3501 MHz    2555998 s          0 s     519742 s  347724042 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5186
Commit a8bca12 (2016-07-07 02:30 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21333.4609375 MB free)
Uptime: 3.514261e6 sec
Load Avg:  1.0166015625  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3650019 s          0 s     816364 s  346171452 s         11 s
#2  3501 MHz    9987598 s          0 s     703315 s  340419892 s          4 s
#3  3501 MHz    3823980 s          0 s     558150 s  346839911 s          3 s
#4  3501 MHz    2601108 s          0 s     525967 s  348125090 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
