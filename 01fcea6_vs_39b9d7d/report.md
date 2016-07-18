# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@01fcea6a4bdd45c602122b9931a36d0286a6ec37](https://github.com/JuliaLang/julia/commit/01fcea6a4bdd45c602122b9931a36d0286a6ec37) vs [JuliaLang/julia@39b9d7d162cb80e411a38d2bc4d1661c78d214a3](https://github.com/JuliaLang/julia/commit/39b9d7d162cb80e411a38d2bc4d1661c78d214a3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16969#issuecomment-233209601)

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
| `["array","setindex!",("setindex!",1)]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",2)]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",3)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",4)]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5477
Commit 01fcea6 (2016-07-17 18:10 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13173.83984375 MB free)
Uptime: 4.446804e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5652016 s          0 s    1135268 s  436893744 s         16 s
#2  3501 MHz   13327818 s          0 s     917392 s  430024713 s          4 s
#3  3501 MHz    4910463 s          0 s     706615 s  438812204 s          6 s
#4  3501 MHz    3431243 s          0 s     663009 s  440376524 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5475
Commit 39b9d7d (2016-07-17 18:07 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13008.21484375 MB free)
Uptime: 4.451441e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5692758 s          0 s    1141330 s  437309247 s         16 s
#2  3501 MHz   13601734 s          0 s     927981 s  430203511 s          4 s
#3  3501 MHz    4988085 s          0 s     714088 s  439190078 s          6 s
#4  3501 MHz    3472663 s          0 s     668994 s  440792189 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
