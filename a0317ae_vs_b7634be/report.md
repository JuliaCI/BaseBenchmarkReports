# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a0317aedebe82cc70cbf45c1dea53beb7b6a76c3](https://github.com/JuliaLang/julia/commit/a0317aedebe82cc70cbf45c1dea53beb7b6a76c3) vs [JuliaLang/julia@b7634bec45dc6ca7b4317fc862cf632c0bcea27f](https://github.com/JuliaLang/julia/commit/b7634bec45dc6ca7b4317fc862cf632c0bcea27f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17057#issuecomment-256251810)

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
| `["array","index",("sum","3darray")]` | 2.67 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.71 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumeach","BitArray{2}")]` | 0.71 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumelt","BitArray{2}")]` | 0.72 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.70 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.74 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","reductions",("mean","Float64")]` | 3.05 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("mean","Int64")]` | 3.39 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sum","Float64")]` | 3.06 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sum","Int64")]` | 3.45 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Float64")]` | 2.65 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs","Int64")]` | 2.01 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Float64")]` | 1.54 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("sumabs2","Int64")]` | 1.23 (15%) :x: | Inf (1%) :x: |
| `["array","reductions",("var","Float64")]` | 2.21 (15%) :x: | 2.13 (1%) :x: |
| `["array","reductions",("var","Int64")]` | 1.42 (15%) :x: | 2.00 (1%) :x: |
| `["broadcast","sparse",((1000,1000),2)]` | 2.75 (15%) :x: | 1.01 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.25 (15%) :x: | 1.23 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.24 (15%) :x: | 1.38 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.20 (15%) :x: | 1.11 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.23 (15%) :x: | 1.28 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.24 (15%) :x: | 1.36 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.21 (15%) :x: | 1.01 (1%) :x: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 1.16 (15%) :x: | 1.02 (1%) :x: |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 0.74 (1%) :white_check_mark: |
| `["string","replace"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",60,Float64)]` | 1.47 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 1.55 (40%) :x: | 1.00 (1%)  |

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
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1136
Commit a0317ae (2016-10-26 03:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12348.98828125 MB free)
Uptime: 1.3111507e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   21738209 s          0 s    3611879 s  1283059818 s         42 s
#2  3501 MHz   57755459 s          0 s    4044618 s  1247442000 s         13 s
#3  3501 MHz   18858770 s          0 s    2396094 s  1289265323 s         20 s
#4  3501 MHz   15685008 s          0 s    2314169 s  1292633696 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1123
Commit b7634be (2016-10-25 19:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12065.47265625 MB free)
Uptime: 1.3117228e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   21788858 s          0 s    3619474 s  1283572081 s         42 s
#2  3501 MHz   58069619 s          0 s    4052472 s  1247691422 s         13 s
#3  3501 MHz   18981110 s          0 s    2406178 s  1289704326 s         20 s
#4  3501 MHz   15738840 s          0 s    2320429 s  1293145107 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
