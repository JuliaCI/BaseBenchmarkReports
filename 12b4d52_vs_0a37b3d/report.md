# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@12b4d52f31e2955601ba98823d1b1e3807b4f31b](https://github.com/JuliaLang/julia/commit/12b4d52f31e2955601ba98823d1b1e3807b4f31b) vs [JuliaLang/julia@0a37b3d42a0b159aad0eebefbcf3280dda2966b4](https://github.com/JuliaLang/julia/commit/0a37b3d42a0b159aad0eebefbcf3280dda2966b4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22958#issuecomment-318103638)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:1)")]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 1.80 (25%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
- `["scalar","arithmetic"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
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
Julia Version 0.7.0-DEV.1125
Commit 12b4d52 (2017-07-26 14:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   79065776 s          0 s   14463470 s  3569533172 s         85 s
       #2  3501 MHz  322409718 s          0 s    8969924 s  3340255441 s         13 s
       #3  3501 MHz   68866850 s          0 s    8006708 s  3595147493 s         70 s
       #4  3501 MHz   65684673 s          0 s    8200326 s  3598114459 s         16 s
       
  Memory: 31.383651733398438 GB (2892.08984375 MB free)
  Uptime: 3.673777e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1123
Commit 0a37b3d (2017-07-26 13:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   79162511 s          0 s   14472451 s  3570092828 s         85 s
       #2  3501 MHz  323012550 s          0 s    8981306 s  3340308518 s         13 s
       #3  3501 MHz   68946666 s          0 s    8013910 s  3595727724 s         70 s
       #4  3501 MHz   65761536 s          0 s    8207210 s  3598698165 s         16 s
       
  Memory: 31.383651733398438 GB (2880.6953125 MB free)
  Uptime: 3.674445e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
