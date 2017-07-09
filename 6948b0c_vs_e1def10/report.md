# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6948b0c9a8ed5dd552a68d970fbaeb37280602a8](https://github.com/JuliaLang/julia/commit/6948b0c9a8ed5dd552a68d970fbaeb37280602a8) vs [JuliaLang/julia@e1def102429941705bc16009e35a74abcdb6f88e](https://github.com/JuliaLang/julia/commit/e1def102429941705bc16009e35a74abcdb6f88e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20005#issuecomment-313920484)

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
| `["array","cat",("vcat_setind",5)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("append!",8)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_single!",256)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BitArray{2}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 2.62 (50%) :x: | 1.10 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 19.74 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 15.10 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 2.63 (50%) :x: | 1.10 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 2.67 (50%) :x: | 1.08 (1%) :x: |
| `["array","index",("sumvector","BitArray{2}")]` | 4.10 (50%) :x: | 1.12 (1%) :x: |
| `["broadcast","sparse",((10000000,),2)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","readstring"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 1.25 (15%) :x: | 1.01 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 31.35 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 1.12 (15%)  | 1.07 (1%) :x: |
| `["problem","json","parse_json"]` | 1.13 (15%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 0.79 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 0.75 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 3.03 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 3.03 (50%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","UInt64","+")]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","-")]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.10 (1%) :x: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(8,))]` | 1.19 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.877
Commit 6948b0c (2017-07-09 13:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   72967740 s          0 s   11167526 s  3434214011 s        110 s
       #2  3501 MHz  287357862 s          0 s   12388296 s  3219703847 s         40 s
       #3  3501 MHz   62540906 s          0 s    7253564 s  3454509427 s         56 s
       #4  3501 MHz   58001597 s          0 s    7195643 s  3459433283 s         19 s
       
  Memory: 31.383651733398438 GB (2822.3125 MB free)
  Uptime: 3.5258857e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.874
Commit e1def10 (2017-07-09 03:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   73045281 s          0 s   11176510 s  3434666907 s        110 s
       #2  3501 MHz  287856760 s          0 s   12396186 s  3219738103 s         40 s
       #3  3501 MHz   62623372 s          0 s    7261288 s  3454960144 s         56 s
       #4  3501 MHz   58081078 s          0 s    7203042 s  3459887503 s         19 s
       
  Memory: 31.383651733398438 GB (2777.1953125 MB free)
  Uptime: 3.5264274e7 sec
  Load Avg:  0.95263671875  1.00927734375  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
