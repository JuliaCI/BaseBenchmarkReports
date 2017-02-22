# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9973b8c8b10e4d3cb486ac8274a52ccbe4218cd2](https://github.com/JuliaLang/julia/commit/9973b8c8b10e4d3cb486ac8274a52ccbe4218cd2) vs [JuliaLang/julia@0cebddf9dd0675caf4b3f0bf59cc828c8fd448de](https://github.com/JuliaLang/julia/commit/0cebddf9dd0675caf4b3f0bf59cc828c8fd448de)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19890#issuecomment-281791383)

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
| `["problem","monte carlo","euro_option_devec"]` | 5.53 (15%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 5.16 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.76 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","fast path, k = 1","Float 32")]` | 18.20 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","no agument reduction, k = 9","Float 32")]` | 18.17 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","no agument reduction, k = 9","Float 64")]` | 9.58 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","small argument path","Float 32")]` | 35.62 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","small argument path","Float 64")]` | 25.49 (40%) :x: | 1.00 (1%)  |
| `["shootout","binary_trees"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2916
Commit 9973b8c (2017-02-22 20:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8215.0390625 MB free)
Uptime: 2.3446532e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   48263147 s          0 s    7435184 s  2284027187 s         69 s
#2  3501 MHz  160055044 s          0 s    7970823 s  2172787925 s         24 s
#3  3501 MHz   39383580 s          0 s    4665058 s  2299538505 s         38 s
#4  3501 MHz   35266532 s          0 s    4601736 s  2303937903 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2913
Commit 0cebddf (2017-02-22 20:19 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8035.31640625 MB free)
Uptime: 2.3452726e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   48344180 s          0 s    7445204 s  2284553054 s         69 s
#2  3501 MHz  160619174 s          0 s    7979153 s  2172834176 s         24 s
#3  3501 MHz   39468445 s          0 s    4673272 s  2300064024 s         38 s
#4  3501 MHz   35361925 s          0 s    4609909 s  2304453053 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
