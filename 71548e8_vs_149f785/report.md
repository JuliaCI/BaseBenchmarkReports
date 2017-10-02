# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@71548e86afefe44920a2efcca5656fc75ce65cc7](https://github.com/JuliaLang/julia/commit/71548e86afefe44920a2efcca5656fc75ce65cc7) vs [JuliaLang/julia@149f7851299b9559aff32b1263a828026e41f16b](https://github.com/JuliaLang/julia/commit/149f7851299b9559aff32b1263a828026e41f16b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23897#issuecomment-333489989)

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
| `["array","convert",("Float64","Int")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("prerend!",2048)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","Float64"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.01 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","types",("rand","MersenneTwister","Complex{Int32}")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.90 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{Int64}")]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","positive argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","negative argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","positive argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y positive","x negative","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float32")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Bidiagonal",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Tridiagonal",100)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","atan2"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2034
Commit 71548e8 (2017-10-02 09:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87761359 s          0 s   13646184 s  4148211009 s        174 s
       #2  3501 MHz  353291097 s          0 s   14624992 s  3883748788 s         62 s
       #3  3501 MHz   73353624 s          0 s    8386451 s  4175578342 s         82 s
       #4  3501 MHz   68696948 s          0 s    8265431 s  4180755003 s         30 s
       
  Memory: 31.383651733398438 GB (4055.328125 MB free)
  Uptime: 4.2591417e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2031
Commit 149f785 (2017-10-02 09:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87845090 s          0 s   13656010 s  4148851965 s        174 s
       #2  3501 MHz  353980334 s          0 s   14636950 s  3883784251 s         62 s
       #3  3501 MHz   73436040 s          0 s    8394034 s  4176224855 s         83 s
       #4  3501 MHz   68777404 s          0 s    8273424 s  4181403258 s         30 s
       
  Memory: 31.383651733398438 GB (3722.54296875 MB free)
  Uptime: 4.2598791e7 sec
  Load Avg:  1.1630859375  1.0478515625  1.05615234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
