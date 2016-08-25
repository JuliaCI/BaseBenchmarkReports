# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@dd183172abb418082ebc3f97e5ec13bab33652c9](https://github.com/JuliaLang/julia/commit/dd183172abb418082ebc3f97e5ec13bab33652c9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/dd183172abb418082ebc3f97e5ec13bab33652c9#commitcomment-18770032)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-25 vs 2016-08-18

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
| `["array","index",("sumcartesian","BitArray{2}")]` | 1.41 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumeach","100000000:-1:1")]` | 0.45 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000000")]` | 0.14 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 1.44 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumelt","1:100000000")]` | 0.11 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BitArray{2}")]` | 1.49 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 1.35 (40%)  | 2.00 (1%) :x: |
| `["array","index",("sumlinear","100000000:-1:1")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000000")]` | 0.14 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BitArray{2}")]` | 1.45 (40%) :x: | 2.00 (1%) :x: |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 1.35 (1%) :x: |
| `["simd",("sum_reduce","Float32",4095)]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 1.28 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 1.28 (20%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ascending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.400
Commit dd18317 (2016-08-25 01:49 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20894.0390625 MB free)
Uptime: 7.747435e6 sec
Load Avg:  1.0029296875  0.98828125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13319481 s          0 s    2695680 s  756509674 s         27 s
#2  3501 MHz   34097264 s          0 s    1679779 s  738435270 s          4 s
#3  3501 MHz   11797976 s          0 s    1470469 s  761098524 s         16 s
#4  3501 MHz   10291652 s          0 s    1478904 s  762588525 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
