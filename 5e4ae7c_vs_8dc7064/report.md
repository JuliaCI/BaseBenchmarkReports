# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5e4ae7c26415e4591784e9c7950c07b8389c556f](https://github.com/JuliaLang/julia/commit/5e4ae7c26415e4591784e9c7950c07b8389c556f) vs [JuliaLang/julia@8dc7064be054706a847a7497a98aae707ea57073](https://github.com/JuliaLang/julia/commit/8dc7064be054706a847a7497a98aae707ea57073)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20933#issuecomment-284850370)

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
| `["broadcast","sparse",((1000,1000),1)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.27 (20%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.75
Commit 5e4ae7c (2017-03-07 20:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8542.8203125 MB free)
Uptime: 2.4569918e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   51889721 s          0 s    8035448 s  2391817082 s         74 s
#2  3501 MHz  185858712 s          0 s    8552272 s  2258601112 s         26 s
#3  3501 MHz   42810512 s          0 s    5019060 s  2408048568 s         39 s
#4  3501 MHz   38636370 s          0 s    4957908 s  2412513507 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.73
Commit 8dc7064 (2017-03-07 18:15 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8302.984375 MB free)
Uptime: 2.4576243e7 sec
Load Avg:  1.13427734375  1.04541015625  1.0537109375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   51969204 s          0 s    8045519 s  2392357567 s         74 s
#2  3501 MHz  186435903 s          0 s    8561081 s  2258646977 s         26 s
#3  3501 MHz   42904766 s          0 s    5027571 s  2408577544 s         39 s
#4  3501 MHz   38719655 s          0 s    4966116 s  2413053925 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
