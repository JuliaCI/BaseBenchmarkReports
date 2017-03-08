# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1a8a77186d72c94ed1cfac11175a1354e77ab49b](https://github.com/JuliaLang/julia/commit/1a8a77186d72c94ed1cfac11175a1354e77ab49b) vs [JuliaLang/julia@34be66a82b85c980ccec8cd84c4c608a93c48784](https://github.com/JuliaLang/julia/commit/34be66a82b85c980ccec8cd84c4c608a93c48784)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20853#issuecomment-285110949)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 2.01 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 2.01 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.69 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.87 (45%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.85 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.85 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.90 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.84 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.81 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["sparse","index",("spmat","logical",100)]` | 1.47 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.94
Commit 1a8a771 (2017-03-08 17:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8777.41796875 MB free)
Uptime: 2.4646613e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44459770 s          0 s    9040385 s  2404023229 s         71 s
#2  3501 MHz  173036324 s          0 s    5569959 s  2284613087 s         10 s
#3  3501 MHz   40218200 s          0 s    4864961 s  2418413343 s         51 s
#4  3501 MHz   37788014 s          0 s    5014093 s  2420683655 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.88
Commit 34be66a (2017-03-08 17:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8553.484375 MB free)
Uptime: 2.4652184e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44540726 s          0 s    9049860 s  2404487761 s         71 s
#2  3501 MHz  173535790 s          0 s    5578631 s  2284661455 s         10 s
#3  3501 MHz   40299725 s          0 s    4873498 s  2418879742 s         51 s
#4  3501 MHz   37882393 s          0 s    5022094 s  2421137920 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
