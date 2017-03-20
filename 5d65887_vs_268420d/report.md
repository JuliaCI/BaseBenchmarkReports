# Benchmark Report

## Job Properties

*Commit(s):* [ajkeller34/julia@5d658872208849cf19f2b4c371a5b2489d682920](https://github.com/ajkeller34/julia/commit/5d658872208849cf19f2b4c371a5b2489d682920) vs [JuliaLang/julia@268420df5211670fd7df3e6e4d1b4fc3f15c793f](https://github.com/JuliaLang/julia/commit/268420df5211670fd7df3e6e4d1b4fc3f15c793f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21099#issuecomment-287667646)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 2.17 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem","json","parse_json"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","binary_trees"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 1.37 (20%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4096)]` | 1.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Int32",4095)]` | 1.28 (20%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Int32",4096)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Int64",4095)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.40 (20%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.189
Commit 5d65887 (2017-03-20 00:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2896.15625 MB free)
Uptime: 2.5628671e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   48150916 s          0 s    9541099 s  2497746995 s         73 s
#2  3501 MHz  183605716 s          0 s    5816365 s  2371950677 s         10 s
#3  3501 MHz   42252546 s          0 s    5103555 s  2514295183 s         53 s
#4  3501 MHz   39833953 s          0 s    5244656 s  2516569576 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.187
Commit 268420d (2017-03-19 21:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2888.2109375 MB free)
Uptime: 2.5634998e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   48231586 s          0 s    9551040 s  2498286780 s         73 s
#2  3501 MHz  184184810 s          0 s    5825118 s  2371995076 s         10 s
#3  3501 MHz   42345140 s          0 s    5112319 s  2514825857 s         53 s
#4  3501 MHz   39917024 s          0 s    5253344 s  2517109907 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
