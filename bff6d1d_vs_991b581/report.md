# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@bff6d1d2a95aae5fa0fe1d4168979d70a8683d3d](https://github.com/musm/julia/commit/bff6d1d2a95aae5fa0fe1d4168979d70a8683d3d) vs [JuliaLang/julia@991b581c2723c57fc0d5005c1c7b61a1b0458308](https://github.com/JuliaLang/julia/commit/991b581c2723c57fc0d5005c1c7b61a1b0458308)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21445#issuecomment-297966296)

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
| `["array","bool","boolarray_true_load!"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 2.20 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","agument reduction, k = 2","Float64")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","agument reduction, k = 83","Float32")]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","agument reduction, k = 83","Float64")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","direct approx, k = 0","Float32")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","direct approx, k = 0","Float64")]` | 0.14 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","no agument reduction, k = 1","Float32")]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","no agument reduction, k = 1","Float64")]` | 0.18 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","normal path -> small, k = -150","Float32")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","overflow","Float32")]` | 0.09 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","overflow","Float64")]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","taylor expansion","Float32")]` | 0.06 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","underflow","Float32")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp10","underflow","Float64")]` | 0.05 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.beta.401
Commit bff6d1d (2017-04-28 08:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2822.859375 MB free)
Uptime: 2.9027194e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   59130488 s          0 s    9170032 s  2828208754 s         85 s
#2  3501 MHz  223453256 s          0 s   10096183 s  2663793888 s         33 s
#3  3501 MHz   49979440 s          0 s    5837334 s  2845605179 s         45 s
#4  3501 MHz   45538704 s          0 s    5781829 s  2850371654 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.397
Commit 991b581 (2017-04-28 08:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2609.97265625 MB free)
Uptime: 2.9032689e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   59214240 s          0 s    9179750 s  2828662800 s         85 s
#2  3501 MHz  223959988 s          0 s   10105152 s  2663827238 s         33 s
#3  3501 MHz   50058694 s          0 s    5846102 s  2846065973 s         45 s
#4  3501 MHz   45625203 s          0 s    5790130 s  2850825877 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
