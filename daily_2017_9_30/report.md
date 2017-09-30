# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f47acd590096f2f33a5e1d37e9c6f7331978d78a](https://github.com/JuliaLang/julia/commit/f47acd590096f2f33a5e1d37e9c6f7331978d78a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f47acd590096f2f33a5e1d37e9c6f7331978d78a#commitcomment-24666309)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-09-30 vs 2017-09-29

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.00 (25%)  | 0.97 (1%) :white_check_mark: |
| `["random","types",("randexp!","RandomDevice","Float64")]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 0.66 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4096)]` | 0.67 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2009
Commit f47acd5 (2017-09-30 02:04 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   95528010 s          0 s   16959372 s  4114714765 s         93 s
       #2  3501 MHz  410243130 s          0 s   10943236 s  3815997575 s         20 s
       #3  3501 MHz   82758042 s          0 s    9398982 s  4145443731 s         77 s
       #4  3501 MHz   79090268 s          0 s    9591760 s  4148921291 s         18 s
       
  Memory: 31.383651733398438 GB (2857.70703125 MB free)
  Uptime: 4.2396337e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
