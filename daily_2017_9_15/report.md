# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ac714a1d118d0664890b683635cc47123aa52c22](https://github.com/JuliaLang/julia/commit/ac714a1d118d0664890b683635cc47123aa52c22)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ac714a1d118d0664890b683635cc47123aa52c22#commitcomment-24316804)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-09-15 vs 2017-09-14

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
| `["array","setindex!",("setindex!",5)]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 0.64 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.74 (15%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.00 (25%)  | 1.01 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 1.01 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 0.51 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.86 (15%)  | 0.95 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","integer",10)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 0.53 (15%) :white_check_mark: | 0.80 (1%) :white_check_mark: |

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
- `["sparse","constructors"]`
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
Julia Version 0.7.0-DEV.1783
Commit ac714a1 (2017-09-14 19:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92536284 s          0 s   16428487 s  3988956253 s         92 s
       #2  3501 MHz  391634024 s          0 s   10574539 s  3705344950 s         19 s
       #3  3501 MHz   80317015 s          0 s    9148577 s  4018495746 s         76 s
       #4  3501 MHz   76785658 s          0 s    9340750 s  4021836489 s         18 s
       
  Memory: 31.383651733398438 GB (5668.046875 MB free)
  Uptime: 4.1099422e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
