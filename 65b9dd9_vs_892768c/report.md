# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@65b9dd914c6eae54af957289fe946d3c5759dcc8](https://github.com/JuliaLang/julia/commit/65b9dd914c6eae54af957289fe946d3c5759dcc8) vs [JuliaLang/julia@892768cf52aeb7542f70ad0b15123e27c5e07dfe](https://github.com/JuliaLang/julia/commit/892768cf52aeb7542f70ad0b15123e27c5e07dfe)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22954#issuecomment-317901168)

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
| `["array","convert",("Float64","Int")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) |x| < 2.0^20π/4","positive argument","Float64")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) |x| < 9π/4","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) |x| > 2.0^20*π/2","negative argument","Float64")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) |x| > 2.0^20*π/2","positive argument","Float64")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 2π/4","positive argument","Float64")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 9π/4","negative argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 9π/4","positive argument","Float64")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 2π/4","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) |x| > 2.0^20*π/2","negative argument","Float64")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) |x| > 2.0^20*π/2","positive argument","Float64")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1124
Commit 65b9dd9 (2017-07-25 22:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   75249520 s          0 s   11685362 s  3572771666 s        124 s
       #2  3501 MHz  295853171 s          0 s   12683459 s  3352551956 s         42 s
       #3  3501 MHz   64256482 s          0 s    7431040 s  3594377553 s         59 s
       #4  3501 MHz   59709796 s          0 s    7363379 s  3599332819 s         20 s
       
  Memory: 31.383651733398438 GB (14467.16015625 MB free)
  Uptime: 3.6676833e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1122
Commit 892768c (2017-07-25 22:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   75327606 s          0 s   11694982 s  3573363419 s        124 s
       #2  3501 MHz  296474274 s          0 s   12694481 s  3352601307 s         42 s
       #3  3501 MHz   64337005 s          0 s    7438108 s  3594971303 s         59 s
       #4  3501 MHz   59804512 s          0 s    7370580 s  3599912617 s         20 s
       
  Memory: 31.383651733398438 GB (14130.94921875 MB free)
  Uptime: 3.6683655e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
