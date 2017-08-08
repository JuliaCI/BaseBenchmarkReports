# Benchmark Report

## Job Properties

*Commit(s):* [Jutho/julia@4f51228587f488617b82fb4d5ac90c1f51d35446](https://github.com/Jutho/julia/commit/4f51228587f488617b82fb4d5ac90c1f51d35446) vs [JuliaLang/julia@edbcb917d44f7f428a0d2e2b3db2cc20b207b097](https://github.com/JuliaLang/julia/commit/edbcb917d44f7f428a0d2e2b3db2cc20b207b097)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23174#issuecomment-321038694)

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
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand!","MersenneTwister","Int","1:1000")]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.05 (25%)  | 1.01 (1%) :x: |
| `["random","types",("rand","MersenneTwister","Complex{Float16}")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Complex{Float32}")]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Complex{UInt16}")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 1.00 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","Int64","-")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 1.70 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1295
Commit 4f51228 (2017-08-08 14:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78711428 s          0 s   12157143 s  3687763000 s        132 s
       #2  3501 MHz  310710336 s          0 s   13166133 s  3456254349 s         47 s
       #3  3501 MHz   66857568 s          0 s    7672281 s  3710729599 s         63 s
       #4  3501 MHz   62202485 s          0 s    7603386 s  3715806323 s         21 s
       
  Memory: 31.383651733398438 GB (3953.37109375 MB free)
  Uptime: 3.7869194e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1292
Commit edbcb91 (2017-08-08 14:40 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78790701 s          0 s   12166205 s  3688281822 s        132 s
       #2  3501 MHz  311257526 s          0 s   13177206 s  3456304886 s         47 s
       #3  3501 MHz   66953389 s          0 s    7679809 s  3711234870 s         63 s
       #4  3501 MHz   62283733 s          0 s    7610642 s  3716326785 s         21 s
       
  Memory: 31.383651733398438 GB (3289.3515625 MB free)
  Uptime: 3.7875289e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
