# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e89d150c9a1bd45fda40ddba58135aa3ac2f582d](https://github.com/JuliaLang/julia/commit/e89d150c9a1bd45fda40ddba58135aa3ac2f582d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/e89d150c9a1bd45fda40ddba58135aa3ac2f582d#commitcomment-23900592)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-27 vs 2017-08-26

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
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.93 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.94 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.02 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.02 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 1.02 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.02 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.01 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.04 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.07 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.04 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.04 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.03 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.03 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.02 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.98 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.01 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.98 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.38 (25%) :x: | 1.00 (1%)  |

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
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
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
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
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
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1519
Commit e89d150 (2017-08-26 22:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88278894 s          0 s   15799997 s  3830122933 s         90 s
       #2  3501 MHz  373529170 s          0 s   10158833 s  3559766470 s         15 s
       #3  3501 MHz   77635651 s          0 s    8853720 s  3857358231 s         75 s
       #4  3501 MHz   74227474 s          0 s    9041316 s  3860579058 s         17 s
       
  Memory: 31.383651733398438 GB (4453.11328125 MB free)
  Uptime: 3.945752e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
