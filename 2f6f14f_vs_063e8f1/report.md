# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@2f6f14fb807184809f024c3755ad83c0fccde178](https://github.com/JuliaLang/julia/commit/2f6f14fb807184809f024c3755ad83c0fccde178) vs [JuliaLang/julia@063e8f110bb7f0ee61bbc166ad6d0af7e2113d87](https://github.com/JuliaLang/julia/commit/063e8f110bb7f0ee61bbc166ad6d0af7e2113d87)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22202#issuecomment-305975932)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.98 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.60 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),1)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["dates","string","Date"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.41 (45%) :x: | 1.00 (1%)  |
| `["micro","parseint"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 6.89 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int8")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 3.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 3.40 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 3.36 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 3.40 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Complex{Float32}")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{Float32}")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Float32}")]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 3.40 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Int64")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{UInt64}")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 3.40 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 3.40 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 3.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{UInt64}")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Int64}")]` | 3.40 (50%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","+")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","-")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","UInt64","+")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 93.56 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 93.45 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
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
Julia Version 0.7.0-DEV.464
Commit 2f6f14f (2017-06-03 13:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2701.30859375 MB free)
Uptime: 3.2148773e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   67472879 s          0 s   12626341 s  3125407569 s         81 s
#2  3501 MHz  280123817 s          0 s    7970670 s  2924893649 s         12 s
#3  3501 MHz   60655374 s          0 s    7103585 s  3145561433 s         65 s
#4  3501 MHz   57665710 s          0 s    7260066 s  3148391839 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.460
Commit 063e8f1 (2017-06-03 11:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2681.38671875 MB free)
Uptime: 3.215405e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   67556058 s          0 s   12635895 s  3125840566 s         81 s
#2  3501 MHz  280595194 s          0 s    7979190 s  2924940875 s         12 s
#3  3501 MHz   60751850 s          0 s    7111712 s  3145983895 s         65 s
#4  3501 MHz   57749752 s          0 s    7268420 s  3148826636 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
