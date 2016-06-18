# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f9f3726ed8be109fd95c49329b8790bca73b1b43](https://github.com/JuliaLang/julia/commit/f9f3726ed8be109fd95c49329b8790bca73b1b43) vs [JuliaLang/julia@2ac304dfba75fad148d4070ef4f8a2e400c305bb](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f9f3726ed8be109fd95c49329b8790bca73b1b43#commitcomment-17921591)

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
| `["array","bool","boolarray_true_load!"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_single!",8)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.40 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.40 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",2)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 1.90 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["linalg","blas","axpy!"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dot"]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gbmv!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gemv!"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","ger!"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","symv!"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",1024)]` | 2.62 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 2.50 (25%) :x: | 1.00 (1%)  |

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
Julia Version 0.4.6-pre+52
Commit f9f3726 (2016-06-17 03:54 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27258.30078125 MB free)
Uptime: 1.861142e6 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2103686 s          0 s     514792 s  183017644 s          5 s
#2  3501 MHz    6581736 s          0 s     362164 s  179054722 s          1 s
#3  3501 MHz    2799124 s          0 s     359830 s  182847559 s          1 s
#4  3501 MHz    2339260 s          0 s     333529 s  183342082 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

#### Comparison Build

```
Julia Version 0.4.5
Commit 2ac304d (2016-03-18 00:58 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27106.15234375 MB free)
Uptime: 1.864377e6 sec
Load Avg:  1.1630859375  1.0478515625  1.07080078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2150022 s          0 s     521217 s  183286963 s          5 s
#2  3501 MHz    6756481 s          0 s     368311 s  179196641 s          1 s
#3  3501 MHz    2885304 s          0 s     366940 s  183076965 s          1 s
#4  3501 MHz    2400948 s          0 s     340108 s  183596641 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
