# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e6ffc04fc4f23d8b7bd7bf11720be02c50622172](https://github.com/JuliaLang/julia/commit/e6ffc04fc4f23d8b7bd7bf11720be02c50622172) vs [JuliaLang/julia@b561cfbfbd2b845cb05e8263a86e22dd665fe723](https://github.com/JuliaLang/julia/commit/b561cfbfbd2b845cb05e8263a86e22dd665fe723)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19545#issuecomment-269614287)

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
| `["dates","parse","Date"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.33 (15%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.30 (15%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.03 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.86 (15%)  | 0.79 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.97 (15%)  | 0.90 (1%) :white_check_mark: |
| `["misc","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |

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
- `["broadcast","sparse"]`
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
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1767
Commit e6ffc04 (2016-12-29 11:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6444.6640625 MB free)
Uptime: 1.8660949e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   30696817 s          0 s    4986019 s  1826632552 s         55 s
#2  3501 MHz   92897512 s          0 s    6034688 s  1764061999 s         20 s
#3  3501 MHz   26478644 s          0 s    3364247 s  1835397415 s         30 s
#4  3501 MHz   22495250 s          0 s    3273790 s  1839626737 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1748
Commit b561cfb (2016-12-29 09:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6094.20703125 MB free)
Uptime: 1.8667299e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   30739722 s          0 s    4993693 s  1827214969 s         55 s
#2  3501 MHz   93262342 s          0 s    6041463 s  1764324718 s         20 s
#3  3501 MHz   26529069 s          0 s    3371084 s  1835974401 s         30 s
#4  3501 MHz   22641074 s          0 s    3284526 s  1840104714 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
