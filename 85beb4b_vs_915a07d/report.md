# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@85beb4b0b4f302ef9d1c519ac1a8979f2e881c59](https://github.com/JuliaLang/julia/commit/85beb4b0b4f302ef9d1c519ac1a8979f2e881c59) vs [JuliaLang/julia@915a07d994c06ac37dd96c26abffe3be4ee07d95](https://github.com/JuliaLang/julia/commit/915a07d994c06ac37dd96c26abffe3be4ee07d95)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19730)

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
| `["array","cat",("catnd",5)]` | 2.07 (15%) :x: | 1.47 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.13 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.02 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.08 (15%)  | 1.06 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","100000000:-1:1")]` | 22.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000000)")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 15.19 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BitArray{2}")]` | 1.04 (50%)  | 1.08 (1%) :x: |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 1.91 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 1.62 (50%) :x: | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000000:-1:1")]` | 3.29 (50%) :x: | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000000")]` | 1.80 (50%) :x: | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.79 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.80 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 2.02 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 2.06 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.97 (50%) :x: | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.95 (50%) :x: | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 2.00 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 2.07 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.38 (50%)  | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.01 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.00 (50%) :x: | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 1.52 (50%) :x: | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 15.11 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 3.14 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 3.36 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),1)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.21 (15%) :x: | 1.40 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.15 (15%) :x: | 1.22 (1%) :x: |
| `["dates","string","Date"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.07 (15%)  | 1.11 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 2.25 (15%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.77 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",1000)]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.85 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1713
Commit 85beb4b (2016-12-27 20:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9715.42578125 MB free)
Uptime: 1.8522414e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   29299426 s          0 s    4835587 s  1814360868 s         55 s
#2  3501 MHz   88880684 s          0 s    5918532 s  1754359691 s         20 s
#3  3501 MHz   25580639 s          0 s    3269022 s  1822549727 s         29 s
#4  3501 MHz   21795438 s          0 s    3189537 s  1826565298 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1711
Commit 915a07d (2016-12-27 19:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9602.41796875 MB free)
Uptime: 1.8529843e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   29431140 s          0 s    4847748 s  1814957699 s         55 s
#2  3501 MHz   89361737 s          0 s    5930570 s  1754608764 s         20 s
#3  3501 MHz   25622392 s          0 s    3274806 s  1823244169 s         29 s
#4  3501 MHz   21847913 s          0 s    3196708 s  1827247967 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
