# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@843e0fea2549add6a7d1d6c752c5906691d601d6](https://github.com/JuliaLang/julia/commit/843e0fea2549add6a7d1d6c752c5906691d601d6) vs [JuliaLang/julia@7126d894cac4112fe75203cf8ffdf7862cbcdf21](https://github.com/JuliaLang/julia/commit/7126d894cac4112fe75203cf8ffdf7862cbcdf21)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/843e0fea2549add6a7d1d6c752c5906691d601d6#commitcomment-18973210)

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
| `["simd",("sum_reduce","Float32",4095)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 0.60 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.65 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 0.67 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
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
Julia Version 0.6.0-dev.588
Commit 843e0fe (2016-09-10 01:21 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17668.20703125 MB free)
Uptime: 9.151633e6 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15076043 s          0 s    3157317 s  894314568 s         29 s
#2  3501 MHz   38580321 s          0 s    1933193 s  874045155 s          4 s
#3  3501 MHz   13803448 s          0 s    1699040 s  899226630 s         17 s
#4  3501 MHz   11742622 s          0 s    1712607 s  901254830 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.462
Commit 7126d89 (2016-09-03 18:30 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17241.640625 MB free)
Uptime: 9.156274e6 sec
Load Avg:  0.9169921875  0.96875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15130546 s          0 s    3165515 s  894714658 s         29 s
#2  3501 MHz   38831346 s          0 s    1943360 s  874247636 s          4 s
#3  3501 MHz   13852651 s          0 s    1704782 s  899634855 s         17 s
#4  3501 MHz   11821294 s          0 s    1719724 s  901632569 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
