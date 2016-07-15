# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a500d6a165b31d73b4e4ee5a8a672078f587e174](https://github.com/JuliaLang/julia/commit/a500d6a165b31d73b4e4ee5a8a672078f587e174) vs [JuliaLang/julia@54a6490cdd0e4fe6e93d53ac20c79b9b75d7c89a](https://github.com/JuliaLang/julia/commit/54a6490cdd0e4fe6e93d53ac20c79b9b75d7c89a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17228#issuecomment-233025624)

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
| `["array","setindex!",("setindex!",1)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.50 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.34 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.50 (30%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.32 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.76 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.53 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.75 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.52 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.75 (30%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.52 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.32 (20%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5450
Commit a500d6a (2016-07-15 18:07 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13284.046875 MB free)
Uptime: 4.256027e6 sec
Load Avg:  0.9228515625  0.998046875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5394736 s          0 s    1084342 s  418163544 s         15 s
#2  3501 MHz   12460252 s          0 s     862952 s  411892702 s          4 s
#3  3501 MHz    4530768 s          0 s     665518 s  420165279 s          5 s
#4  3501 MHz    3209994 s          0 s     630256 s  421561203 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5448
Commit 54a6490 (2016-07-15 08:36 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13150.73046875 MB free)
Uptime: 4.260619e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5436418 s          0 s    1091116 s  418572910 s         15 s
#2  3501 MHz   12736970 s          0 s     873904 s  412063757 s          4 s
#3  3501 MHz    4598338 s          0 s     671904 s  420549823 s          5 s
#4  3501 MHz    3254503 s          0 s     635368 s  421970190 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
