# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6b2a83adb1b7b9e69942d928b353a0311468ae99](https://github.com/JuliaLang/julia/commit/6b2a83adb1b7b9e69942d928b353a0311468ae99)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/6b2a83adb1b7b9e69942d928b353a0311468ae99#commitcomment-22801771)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-06-28 vs 2017-06-27

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
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.18 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 0.21 (60%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","agument reduction, k = 2","Float64")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","agument reduction, k = 83","Float32")]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","agument reduction, k = 83","Float64")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","direct approx, k = 0","Float32")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","direct approx, k = 0","Float64")]` | 0.14 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","no agument reduction, k = 1","Float32")]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","no agument reduction, k = 1","Float64")]` | 0.18 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","normal path -> small, k = -150","Float32")]` | 0.07 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","overflow","Float32")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","overflow","Float64")]` | 0.11 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","taylor expansion","Float32")]` | 0.06 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","underflow","Float32")]` | 0.07 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","underflow","Float64")]` | 0.06 (40%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matvec",(2,2),(2,))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.769
Commit 6b2a83a (2017-06-28 01:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71570668 s          0 s   13392548 s  3332346076 s         83 s
       #2  3501 MHz  301243264 s          0 s    8498756 s  3115511467 s         12 s
       #3  3501 MHz   64895822 s          0 s    7583688 s  3353133965 s         68 s
       #4  3501 MHz   61798052 s          0 s    7760054 s  3356041079 s         15 s
       
  Memory: 31.383651733398438 GB (2571.48046875 MB free)
  Uptime: 3.4272735e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
