# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3ccfd1c9d884af8038f23ed7d1981161436c04f8](https://github.com/JuliaLang/julia/commit/3ccfd1c9d884af8038f23ed7d1981161436c04f8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3ccfd1c9d884af8038f23ed7d1981161436c04f8#commitcomment-21029965)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-02-24 vs 2017-02-23

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
| `["array","convert",("Float64","Int")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:0.00010001000100010001:2.0")]` | 0.31 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:0.00010001000100010001:2.0")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:0.00010001000100010001:2.0")]` | 0.31 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:0.00010001000100010001:2.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("norm","Int64")]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.41 (45%) :x: | 1.00 (1%)  |
| `["micro","pisum"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2945
Commit 3ccfd1c (2017-02-24 00:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2852.98046875 MB free)
Uptime: 2.3563814e7 sec
Load Avg:  1.00341796875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   40189865 s          0 s    8433617 s  2300934339 s         68 s
#2  3501 MHz  144522362 s          0 s    5028441 s  2205466687 s          9 s
#3  3501 MHz   36053618 s          0 s    4405981 s  2314827432 s         49 s
#4  3501 MHz   33672177 s          0 s    4554100 s  2317047745 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
