# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@806fb92bb4da23363f81471ac84a1efffbc90d2d](https://github.com/JuliaLang/julia/commit/806fb92bb4da23363f81471ac84a1efffbc90d2d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/806fb92bb4da23363f81471ac84a1efffbc90d2d#commitcomment-19839926)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-11-16 vs 2016-11-15

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
| `["dates","query",("firstdayofmonth","DateTime")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofmonth","Date")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.97 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.97 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.97 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.98 (15%)  | 0.98 (1%) :white_check_mark: |
| `["problem","go","go_game"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.01 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 2.90 (50%) :x: | 4.29 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 2.74 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 2.68 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 2.74 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.98 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.02 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.93 (50%) :x: | 1.79 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.93 (50%) :x: | 1.79 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 2.12 (50%) :x: | 2.00 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 2.12 (50%) :x: | 2.00 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.02 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 1.01 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.01 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.00 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.00 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.00 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.01 (50%)  | 1.03 (1%) :x: |

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
Julia Version 0.6.0-dev.1252
Commit 806fb92 (2016-11-16 01:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10825.70703125 MB free)
Uptime: 1.4923495e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   23691220 s          0 s    3944583 s  1461649248 s         46 s
#2  3501 MHz   65317654 s          0 s    4609885 s  1420167056 s         15 s
#3  3501 MHz   20733540 s          0 s    2646315 s  1468266470 s         25 s
#4  3501 MHz   17266827 s          0 s    2568262 s  1471934425 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
