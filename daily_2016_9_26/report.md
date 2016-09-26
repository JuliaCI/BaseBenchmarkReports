# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a853c81f60d44ce107e7066c39105d963311dcef](https://github.com/JuliaLang/julia/commit/a853c81f60d44ce107e7066c39105d963311dcef)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a853c81f60d44ce107e7066c39105d963311dcef#commitcomment-19167287)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-09-26 vs 2016-09-25

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
| `["array","cat",("catnd",5)]` | 0.70 (15%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","Array","Complex{Float64}")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 1.03 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.04 (15%)  | 0.99 (1%) :white_check_mark: |
| `["sort","issorted",("forwards","descending")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.786
Commit a853c81 (2016-09-26 03:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16782.75390625 MB free)
Uptime: 1.0512286e7 sec
Load Avg:  1.0029296875  0.99658203125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16890865 s          0 s    2880892 s  1029237355 s         33 s
#2  3501 MHz   41791567 s          0 s    3047769 s  1004929538 s          9 s
#3  3501 MHz   14639822 s          0 s    1884292 s  1034190171 s         16 s
#4  3501 MHz   12373022 s          0 s    1842287 s  1036592545 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
