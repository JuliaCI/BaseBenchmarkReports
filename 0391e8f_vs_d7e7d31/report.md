# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0391e8f9132bba57958f1befd51aa9471ecf46a1](https://github.com/JuliaLang/julia/commit/0391e8f9132bba57958f1befd51aa9471ecf46a1) vs [JuliaLang/julia@d7e7d313f9440734a3d15f3c85da2e814b74151e](https://github.com/JuliaLang/julia/commit/d7e7d313f9440734a3d15f3c85da2e814b74151e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23903)

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
| `["dates","parse",("DateTime","DateFormat")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.98 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","sequences",("randcycle","MersenneTwister","1000")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["random","sequences",("randperm","MersenneTwister","1000")]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["random","sequences",("shuffle!","MersenneTwister")]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","ImplicitRNG","Float64")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","ImplicitRNG","Int64")]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.98 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","BigFloat")]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 0.74 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4096)]` | 0.68 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["string","search","String"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(8,8))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1977
Commit 0391e8f (2017-09-27 16:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   86848672 s          0 s   13534402 s  4108281294 s        170 s
       #2  3501 MHz  347726094 s          0 s   14429662 s  3848563881 s         58 s
       #3  3501 MHz   72517474 s          0 s    8295412 s  4135485363 s         79 s
       #4  3501 MHz   67842234 s          0 s    8180738 s  4140673140 s         28 s
       
  Memory: 31.383651733398438 GB (2574.34765625 MB free)
  Uptime: 4.2181066e7 sec
  Load Avg:  1.1220703125  1.0439453125  1.05224609375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1975
Commit d7e7d31 (2017-09-27 14:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   86946556 s          0 s   13544672 s  4108899811 s        170 s
       #2  3501 MHz  348388272 s          0 s   14441192 s  3848618816 s         58 s
       #3  3501 MHz   72602840 s          0 s    8303196 s  4136120766 s         79 s
       #4  3501 MHz   67924857 s          0 s    8188407 s  4141311601 s         28 s
       
  Memory: 31.383651733398438 GB (2990.171875 MB free)
  Uptime: 4.218836e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
