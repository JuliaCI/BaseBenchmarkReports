# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ce35ee32b252ea232fba3c7f1ade02dd0014e20c](https://github.com/JuliaLang/julia/commit/ce35ee32b252ea232fba3c7f1ade02dd0014e20c) vs [JuliaLang/julia@6445c82d0060dbe82b88436f0f4371a4ee64d918](https://github.com/JuliaLang/julia/commit/6445c82d0060dbe82b88436f0f4371a4ee64d918)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21684#issuecomment-299234947)

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
| `["array","cat",("hcat",5)]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 0.45 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",2048)]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 2.27 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 2.51 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 2.12 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 2.14 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 2.12 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",1024)]` | 0.39 (45%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",256)]` | 0.37 (45%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Diagonal",256)]` | 1.77 (45%) :x: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 2.76 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 2.80 (15%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 2.72 (15%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","meteor_contest"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 2.60 (15%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 2.16 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.48 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.2-pre+60
Commit ce35ee3 (2017-05-04 16:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8902.3984375 MB free)
Uptime: 2.9568135e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61234136 s          0 s    9439870 s  2879815123 s         86 s
#2  3501 MHz  232906864 s          0 s   10429497 s  2707994823 s         35 s
#3  3501 MHz   52115404 s          0 s    6065623 s  2897305098 s         45 s
#4  3501 MHz   47654726 s          0 s    6006715 s  2902102925 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.1
Commit 6445c82 (2017-03-05 13:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9407.51171875 MB free)
Uptime: 2.9577004e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61306307 s          0 s    9451436 s  2880615023 s         86 s
#2  3501 MHz  233732912 s          0 s   10447920 s  2708036576 s         35 s
#3  3501 MHz   52207098 s          0 s    6074064 s  2898091262 s         45 s
#4  3501 MHz   47732618 s          0 s    6015178 s  2902902947 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
