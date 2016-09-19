# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f30c9499b62e4959d8265b1e22401702f073aa15](https://github.com/JuliaLang/julia/commit/f30c9499b62e4959d8265b1e22401702f073aa15) vs [JuliaLang/julia@e781d08180a96519e84793e872c96e095df95c79](https://github.com/JuliaLang/julia/commit/e781d08180a96519e84793e872c96e095df95c79)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f30c9499b62e4959d8265b1e22401702f073aa15#commitcomment-19082011)

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
| `["array","cat",("catnd",5)]` | 1.48 (15%) :x: | 1.10 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 0.99 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["sort","issorted",("forwards","descending")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
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
Julia Version 0.6.0-dev.664
Commit f30c949 (2016-09-16 04:29 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19031.2734375 MB free)
Uptime: 9.955785e6 sec
Load Avg:  1.0029296875  1.0146484375  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15553964 s          0 s    2689835 s  975225532 s         31 s
#2  3501 MHz   38116786 s          0 s    2806921 s  953293557 s          8 s
#3  3501 MHz   13435254 s          0 s    1732094 s  979928436 s         14 s
#4  3501 MHz   10897180 s          0 s    1677570 s  982603856 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.662
Commit e781d08 (2016-09-16 04:24 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18636.265625 MB free)
Uptime: 9.960497e6 sec
Load Avg:  0.9228515625  0.998046875  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15588594 s          0 s    2695956 s  975654444 s         31 s
#2  3501 MHz   38312117 s          0 s    2813566 s  953561948 s          8 s
#3  3501 MHz   13480563 s          0 s    1739052 s  980346582 s         14 s
#4  3501 MHz   11061845 s          0 s    1689481 s  982897994 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
