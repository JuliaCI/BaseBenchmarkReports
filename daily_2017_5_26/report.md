# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9e3318c9840e7a9e387582ba861408cefe5a4f75](https://github.com/JuliaLang/julia/commit/9e3318c9840e7a9e387582ba861408cefe5a4f75)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/9e3318c9840e7a9e387582ba861408cefe5a4f75#commitcomment-22288183)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-05-26 vs 2017-05-25

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
| `["array","bool","boolarray_true_load!"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","day"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 4.87 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 6.60 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 5.03 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 16.73 (50%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
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
- `["scalar","intfuncs"]`
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
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.357
Commit 9e3318c (2017-05-25 19:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4918.015625 MB free)
Uptime: 3.1421492e7 sec
Load Avg:  0.97900390625  1.0126953125  1.04345703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   65489059 s          0 s   12303144 s  3055200279 s         80 s
#2  3501 MHz  269952217 s          0 s    7734025 s  2862619183 s         12 s
#3  3501 MHz   58619868 s          0 s    6888104 s  3075121596 s         65 s
#4  3501 MHz   55679614 s          0 s    7041360 s  3077908591 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
