# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8eca02717bcea524877fad01aacedc807898bcd1](https://github.com/JuliaLang/julia/commit/8eca02717bcea524877fad01aacedc807898bcd1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/8eca02717bcea524877fad01aacedc807898bcd1#commitcomment-21957881)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-04-29 vs 2017-04-28

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.72 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Month")]` | 1.16 (15%) :x: | Inf (1%) :x: |
| `["dates","arithmetic",("Date","Year")]` | 1.28 (15%) :x: | Inf (1%) :x: |
| `["dates","arithmetic",("DateTime","Month")]` | 1.20 (15%) :x: | Inf (1%) :x: |
| `["dates","arithmetic",("DateTime","Year")]` | 1.23 (15%) :x: | Inf (1%) :x: |
| `["dates","construction","Date"]` | 1.53 (15%) :x: | Inf (1%) :x: |
| `["dates","construction","DateTime"]` | 1.86 (15%) :x: | Inf (1%) :x: |
| `["dates","parse","Date"]` | 1.19 (15%) :x: | Inf (1%) :x: |
| `["dates","parse","DateTime"]` | 1.26 (15%) :x: | Inf (1%) :x: |
| `["dates","parse",("Date","ISODateFormat")]` | 1.19 (15%) :x: | Inf (1%) :x: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 1.30 (15%) :x: | Inf (1%) :x: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.01 (15%)  | 1.17 (1%) :x: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.08 (15%)  | 1.07 (1%) :x: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 1.51 (45%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 1.26 (15%) :x: | Inf (1%) :x: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.beta.412
Commit 8eca027 (2017-04-28 22:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2473.94921875 MB free)
Uptime: 2.9089033e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   58153281 s          0 s   11190399 s  2831094026 s         77 s
#2  3501 MHz  236803599 s          0 s    6974579 s  2663422868 s         11 s
#3  3501 MHz   52294452 s          0 s    6201194 s  2849008068 s         60 s
#4  3501 MHz   49514061 s          0 s    6346792 s  2851647007 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
