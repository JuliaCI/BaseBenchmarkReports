# Benchmark Report

## Job Properties

*Commit(s):* [TotalVerb/julia@d366ce09427cafd44c41a4cea2f0f2ec68a993b0](https://github.com/TotalVerb/julia/commit/d366ce09427cafd44c41a4cea2f0f2ec68a993b0) vs [JuliaLang/julia@a7e7a33ed297df2b026e05ab28496b65ed75dea3](https://github.com/JuliaLang/julia/commit/a7e7a33ed297df2b026e05ab28496b65ed75dea3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22825#issuecomment-334853622)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","2d"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 1.71 (45%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.98 (25%)  | 1.01 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.94 (25%)  | 0.99 (1%) :white_check_mark: |
| `["scalar","acos",("one","positive argument","Float32")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("small","negative argument","Float64")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("small","positive argument","Float64")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("zero","Float64")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float32")]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float64")]` | 1.93 (15%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","tan",("large","negative argument","Float32")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","tan",("medium","positive argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","tan",("small","negative argument","Float32")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","tan",("very small","negative argument","Float32")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","tan",("zero","Float32")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.50 (30%) :x: | 1.00 (1%)  |

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
- `["scalar","sincos"]`
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
Julia Version 0.7.0-DEV.2059
Commit d366ce0 (2017-10-06 19:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96918588 s          0 s   17193877 s  4170543587 s         93 s
       #2  3501 MHz  420149575 s          0 s   11152094 s  3863468661 s         20 s
       #3  3501 MHz   84297443 s          0 s    9549764 s  4201347018 s         78 s
       #4  3501 MHz   80483793 s          0 s    9745869 s  4204964803 s         19 s
       
  Memory: 31.383651733398438 GB (2935.984375 MB free)
  Uptime: 4.2972561e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2055
Commit a7e7a33 (2017-10-06 19:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   97000898 s          0 s   17203126 s  4171180773 s         93 s
       #2  3501 MHz  420814681 s          0 s   11163632 s  3863523157 s         20 s
       #3  3501 MHz   84391996 s          0 s    9557264 s  4201975914 s         78 s
       #4  3501 MHz   80565917 s          0 s    9753164 s  4205606561 s         19 s
       
  Memory: 31.383651733398438 GB (3016.1640625 MB free)
  Uptime: 4.2979878e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
