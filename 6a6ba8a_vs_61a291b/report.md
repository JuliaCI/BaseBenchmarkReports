# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6a6ba8a6accaa39c9286fc45f03540370de8702d](https://github.com/JuliaLang/julia/commit/6a6ba8a6accaa39c9286fc45f03540370de8702d) vs [JuliaLang/julia@61a291bf6c4b5997b9b1371a7d3f12a6ce86945a](https://github.com/JuliaLang/julia/commit/61a291bf6c4b5997b9b1371a7d3f12a6ce86945a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20025#issuecomment-281599300)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Float64","Int")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:0.00010001000100010001:2.0")]` | 0.31 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:0.00010001000100010001:2.0")]` | 0.31 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:0.00010001000100010001:2.0")]` | 0.35 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:0.00010001000100010001:2.0")]` | 0.31 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("norm","Int64")]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","pisum"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2904
Commit 6a6ba8a (2017-02-22 04:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8323.40234375 MB free)
Uptime: 2.3403184e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   48099833 s          0 s    7414101 s  2279885758 s         69 s
#2  3501 MHz  158949338 s          0 s    7945048 s  2169594027 s         24 s
#3  3501 MHz   39211628 s          0 s    4648161 s  2295394310 s         38 s
#4  3501 MHz   35092930 s          0 s    4584914 s  2299795052 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2899
Commit 61a291b (2017-02-22 04:15 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8134.21484375 MB free)
Uptime: 2.3409404e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   48182238 s          0 s    7424238 s  2280412892 s         69 s
#2  3501 MHz  159529918 s          0 s    7953514 s  2169626433 s         24 s
#3  3501 MHz   39296284 s          0 s    4656217 s  2295922883 s         38 s
#4  3501 MHz   35172875 s          0 s    4593008 s  2300328463 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
