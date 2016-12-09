# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@374c3d6b3c3e15c00f7d3df8b5cb7c8a763aa746](https://github.com/JuliaLang/julia/commit/374c3d6b3c3e15c00f7d3df8b5cb7c8a763aa746)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/374c3d6b3c3e15c00f7d3df8b5cb7c8a763aa746#commitcomment-20129689)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-12-09 vs 2016-12-06

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("append!",256)]` | 1.03 (15%)  | 1.03 (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["dates","accessor","day"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 0.25 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","month"]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","year"]` | 0.44 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Day")]` | 0.14 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Month")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Day")]` | 0.15 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Hour")]` | 0.14 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Millisecond")]` | 0.14 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Minute")]` | 0.15 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Second")]` | 0.14 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","conversion","Date -> DateTime"]` | 0.15 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","conversion","DateTime -> Date"]` | 0.14 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweek","Date")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweekofmonth","Date")]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweekofmonth","DateTime")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofyear","Date")]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofyear","DateTime")]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("daysofweekinmonth","Date")]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("daysofweekinmonth","DateTime")]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofmonth","Date")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofmonth","DateTime")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","DateTime")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("isleapyear","Date")]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("isleapyear","DateTime")]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofmonth","Date")]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofmonth","DateTime")]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 0.43 (25%) :white_check_mark: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_devec"]` | 1.36 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1528
Commit 374c3d6 (2016-12-08 22:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11732.03125 MB free)
Uptime: 1.6910602e7 sec
Load Avg:  0.9228515625  0.998046875  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26099699 s          0 s    4354841 s  1657181277 s         51 s
#2  3501 MHz   74254634 s          0 s    5268062 s  1608886572 s         18 s
#3  3501 MHz   22842193 s          0 s    2914177 s  1664533082 s         28 s
#4  3501 MHz   18902965 s          0 s    2826196 s  1668696034 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
