# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e3ad45e87d857834c597f6a96fa6a8aaca6fa34f](https://github.com/JuliaLang/julia/commit/e3ad45e87d857834c597f6a96fa6a8aaca6fa34f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/e3ad45e87d857834c597f6a96fa6a8aaca6fa34f#commitcomment-23238409)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-07-22 vs 2017-07-20

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
| `["broadcast","sparse",((1000,1000),1)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["problem","ziggurat","ziggurat"]` | 0.90 (15%)  | 0.99 (1%) :white_check_mark: |
| `["scalar","arithmetic",("rem type","Bool","Bool")]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 0.07 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4096)]` | 0.07 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float64",4095)]` | 0.06 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float64",4096)]` | 0.06 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int32",4095)]` | 0.04 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int32",4096)]` | 0.04 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int64",4095)]` | 0.05 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int64",4096)]` | 0.06 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
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
Julia Version 0.7.0-DEV.1083
Commit e3ad45e (2017-07-22 02:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78062524 s          0 s   14315317 s  3531850237 s         84 s
       #2  3501 MHz  318880311 s          0 s    8884710 s  3304946311 s         13 s
       #3  3501 MHz   68220481 s          0 s    7938333 s  3556931670 s         70 s
       #4  3501 MHz   65026673 s          0 s    8125930 s  3559920552 s         16 s
       
  Memory: 31.383651733398438 GB (4777.3046875 MB free)
  Uptime: 3.6348307e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
