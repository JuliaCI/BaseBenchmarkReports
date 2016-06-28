# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6651f78ac63d779c3c1219c3f7ce33fff97c67fe](https://github.com/JuliaLang/julia/commit/6651f78ac63d779c3c1219c3f7ce33fff97c67fe)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/6651f78ac63d779c3c1219c3f7ce33fff97c67fe#commitcomment-18035364)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-28 vs 2016-06-27

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
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.38 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.38 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 1.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 1.34 (20%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4965
Commit 6651f78 (2016-06-28 02:53 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (26574.34765625 MB free)
Uptime: 2.736185e6 sec
Load Avg:  1.076171875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2632731 s          0 s     604274 s  269777359 s          9 s
#2  3501 MHz    7622575 s          0 s     552717 s  265183351 s          3 s
#3  3501 MHz    2909980 s          0 s     429470 s  270120939 s          2 s
#4  3501 MHz    2069608 s          0 s     414764 s  270997874 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
