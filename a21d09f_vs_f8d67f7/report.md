# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a21d09f80c50677cfb8093cd11c2d2bdc15ad256](https://github.com/JuliaLang/julia/commit/a21d09f80c50677cfb8093cd11c2d2bdc15ad256) vs [JuliaLang/julia@f8d67f7521287d9325e91fd2142dad5f222e6eaf](https://github.com/JuliaLang/julia/commit/f8d67f7521287d9325e91fd2142dad5f222e6eaf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17355#issuecomment-231585257)

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
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.34 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.34 (40%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5263
Commit a21d09f (2016-07-10 11:56 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20848.87109375 MB free)
Uptime: 3.801626e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5047196 s          0 s    1151098 s  372947806 s         15 s
#2  3501 MHz   14207867 s          0 s     731000 s  364997957 s          2 s
#3  3501 MHz    5128178 s          0 s     657856 s  374193407 s          6 s
#4  3501 MHz    4574221 s          0 s     673144 s  374714660 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5260
Commit f8d67f7 (2016-07-10 01:41 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20708.5 MB free)
Uptime: 3.806142e6 sec
Load Avg:  1.0029296875  1.001953125  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5077478 s          0 s    1156874 s  373361918 s         15 s
#2  3501 MHz   14508482 s          0 s     742031 s  365137537 s          2 s
#3  3501 MHz    5180130 s          0 s     663744 s  374586304 s          6 s
#4  3501 MHz    4613683 s          0 s     679630 s  375119749 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
