# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c9132d2af2cb28888e8e74c3d8406978b8be461e](https://github.com/JuliaLang/julia/commit/c9132d2af2cb28888e8e74c3d8406978b8be461e) vs [JuliaLang/julia@7ab6428050466fa20cde4e06869d9a926919ff2c](https://github.com/JuliaLang/julia/commit/7ab6428050466fa20cde4e06869d9a926919ff2c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20593#issuecomment-280410062)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.54 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","Array{Int32,2}")]` | 4.34 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 4.34 (50%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.41 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.40 (45%) :x: | 1.00 (1%)  |
| `["micro","pisum"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.89 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigInt}(1)")]` | 1.90 (60%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.97 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.96 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.96 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.97 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 1.13 (15%)  | 1.02 (1%) :x: |
| `["scalar","iteration","in"]` | 14553.04 (25%) :x: | 1.00 (1%)  |
| `["shootout","fasta"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 1.38 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.90 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.53 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 1.33 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 1.42 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 1.45 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 1.48 (20%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort forwards","ones")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort reverse","descending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! forwards","ones")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","descending")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sort! reverse","ones")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","random")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","random")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","random")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","random")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",3,Float32)]` | 1.66 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",3,Float64)]` | 1.66 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 1.58 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",8,Float32)]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",8,Float64)]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",3,Float64)]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 1.58 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 1.58 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float32)]` | 1.67 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float64)]` | 1.72 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2839
Commit c9132d2 (2017-02-16 16:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2308.10546875 MB free)
Uptime: 2.2919924e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   38249526 s          0 s    8120910 s  2238992395 s         66 s
#2  3501 MHz  131745572 s          0 s    4798610 s  2154125361 s          8 s
#3  3501 MHz   34000441 s          0 s    4200326 s  2252728899 s         48 s
#4  3501 MHz   31709761 s          0 s    4337450 s  2254874113 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2833
Commit 7ab6428 (2017-02-16 16:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2248.9453125 MB free)
Uptime: 2.2925646e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   38327978 s          0 s    8130530 s  2239474436 s         66 s
#2  3501 MHz  132265115 s          0 s    4807203 s  2154168924 s          8 s
#3  3501 MHz   34095861 s          0 s    4208729 s  2253196707 s         48 s
#4  3501 MHz   31792762 s          0 s    4345473 s  2255354825 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
