# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@97f092e749697d471fc5d53854469cb568f4fc01](https://github.com/JuliaLang/julia/commit/97f092e749697d471fc5d53854469cb568f4fc01) vs [JuliaLang/julia@285ec1f0a9211161ecac50fc006d1d4051b9c80f](https://github.com/JuliaLang/julia/commit/285ec1f0a9211161ecac50fc006d1d4051b9c80f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22262#issuecomment-306688797)

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
| `["array","bool","boolarray_true_load!"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs2","Float64")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.41 (45%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.492
Commit 97f092e (2017-06-07 05:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68510895 s          0 s   12782328 s  3155634181 s         82 s
       #2  3501 MHz  285807696 s          0 s    8090360 s  2950581335 s         12 s
       #3  3501 MHz   61720512 s          0 s    7212304 s  3175881824 s         66 s
       #4  3501 MHz   58705639 s          0 s    7373508 s  3178730911 s         15 s
       
  Memory: 31.383651733398438 GB (2681.90625 MB free)
  Uptime: 3.2463888e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.490
Commit 285ec1f (2017-06-06 21:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68596836 s          0 s   12791795 s  3156064701 s         82 s
       #2  3501 MHz  286290778 s          0 s    8098975 s  2950616963 s         12 s
       #3  3501 MHz   61806098 s          0 s    7220551 s  3176315267 s         66 s
       #4  3501 MHz   58785819 s          0 s    7381928 s  3179169672 s         15 s
       
  Memory: 31.383651733398438 GB (2633.19921875 MB free)
  Uptime: 3.2469168e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
