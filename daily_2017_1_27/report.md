# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fa4ba22f2607d266e48900897fa5102e4dd435ff](https://github.com/JuliaLang/julia/commit/fa4ba22f2607d266e48900897fa5102e4dd435ff)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/fa4ba22f2607d266e48900897fa5102e4dd435ff#commitcomment-20636850)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-01-27 vs 2017-01-26

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
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 7.42 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:100000.0")]` | 2.19 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 7.45 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 2.78 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 7.42 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:100000.0")]` | 2.19 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.94 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumvector_view","1.0:1.0:100000.0")]` | 0.96 (50%)  | 1.07 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.21 (20%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","sparse"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
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
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.2400
Commit fa4ba22 (2017-01-27 01:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19017.46484375 MB free)
Uptime: 2.1145492e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   40383902 s          0 s    6252555 s  2063610131 s         63 s
#2  3501 MHz  139101406 s          0 s    7381366 s  1964517593 s         21 s
#3  3501 MHz   35850956 s          0 s    4318839 s  2073381941 s         37 s
#4  3501 MHz   32090178 s          0 s    4257335 s  2077403271 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
