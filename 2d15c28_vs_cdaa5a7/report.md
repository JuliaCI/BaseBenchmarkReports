# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@2d15c283b4150e19b511142d6097929bf9a87673](https://github.com/JuliaLang/julia/commit/2d15c283b4150e19b511142d6097929bf9a87673) vs [JuliaLang/julia@cdaa5a7da38949fb20182d0276b14673961e9999](https://github.com/JuliaLang/julia/commit/cdaa5a7da38949fb20182d0276b14673961e9999)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22877#issuecomment-316841867)

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
| `["array","convert",("Complex{Float64}","Int")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",1024)]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["problem","ziggurat","ziggurat"]` | 0.91 (15%)  | 0.99 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4095)]` | 0.07 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4096)]` | 0.07 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float64",4095)]` | 0.06 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float64",4096)]` | 0.06 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int32",4095)]` | 0.04 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int32",4096)]` | 0.04 (20%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int64",4095)]` | 0.06 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int64",4096)]` | 0.07 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.1064
Commit 2d15c28 (2017-07-20 19:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   74584757 s          0 s   11495880 s  3530268836 s        120 s
       #2  3501 MHz  294387856 s          0 s   12640525 s  3310560959 s         42 s
       #3  3501 MHz   63934581 s          0 s    7399932 s  3551215266 s         59 s
       #4  3501 MHz   59361046 s          0 s    7333544 s  3556193031 s         20 s
       
  Memory: 31.383651733398438 GB (17429.171875 MB free)
  Uptime: 3.6241618e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1059
Commit cdaa5a7 (2017-07-20 19:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   74680534 s          0 s   11505002 s  3530721029 s        120 s
       #2  3501 MHz  294888302 s          0 s   12648418 s  3310611078 s         42 s
       #3  3501 MHz   64014497 s          0 s    7407501 s  3551686165 s         59 s
       #4  3501 MHz   59442284 s          0 s    7340845 s  3556663096 s         20 s
       
  Memory: 31.383651733398438 GB (17197.703125 MB free)
  Uptime: 3.624721e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
