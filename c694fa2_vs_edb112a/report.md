# Benchmark Report

## Job Properties

*Commit(s):* [Sacha0/julia@c694fa2a03ab9cff8fd5505ef97182202806313d](https://github.com/Sacha0/julia/commit/c694fa2a03ab9cff8fd5505ef97182202806313d) vs [JuliaLang/julia@edb112af0b058d1f5a815fc6cb524f586cd18bdd](https://github.com/JuliaLang/julia/commit/edb112af0b058d1f5a815fc6cb524f586cd18bdd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17404#issuecomment-232811897)

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
| `["problem","laplacian","laplace_iter_sub"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5447
Commit c694fa2 (2016-07-14 21:41 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18191.4921875 MB free)
Uptime: 4.185486e6 sec
Load Avg:  1.0029296875  1.0146484375  0.95654296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5565532 s          0 s    1259122 s  410613476 s         16 s
#2  3501 MHz   15285892 s          0 s     791173 s  402221471 s          2 s
#3  3501 MHz    5660578 s          0 s     725006 s  411957724 s          6 s
#4  3501 MHz    4853475 s          0 s     726513 s  412748650 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5440
Commit edb112a (2016-07-14 21:40 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18063.1953125 MB free)
Uptime: 4.190074e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5692273 s          0 s    1269243 s  410934219 s         16 s
#2  3501 MHz   15492465 s          0 s     798437 s  402465985 s          2 s
#3  3501 MHz    5720275 s          0 s     731006 s  412350038 s          6 s
#4  3501 MHz    4890331 s          0 s     732219 s  413164346 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
