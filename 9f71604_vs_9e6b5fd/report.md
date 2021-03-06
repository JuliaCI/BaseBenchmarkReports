# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9f716040e59299d8d835504b712eb0358f6f6558](https://github.com/JuliaLang/julia/commit/9f716040e59299d8d835504b712eb0358f6f6558) vs [JuliaLang/julia@9e6b5fd48e978d70518194733e4fc38f293b6655](https://github.com/JuliaLang/julia/commit/9e6b5fd48e978d70518194733e4fc38f293b6655)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20853#issuecomment-285540745)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","readstring"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.80 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Float32}")]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.81 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.80 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.91 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.84 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.81 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.91 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.80 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 1.45 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.107
Commit 9f71604 (2017-03-10 01:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6072.17578125 MB free)
Uptime: 2.4761468e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   45279050 s          0 s    9133145 s  2414562027 s         72 s
#2  3501 MHz  175253568 s          0 s    5624726 s  2293818796 s         10 s
#3  3501 MHz   40692996 s          0 s    4916353 s  2429366279 s         52 s
#4  3501 MHz   38274614 s          0 s    5066292 s  2431623070 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.100
Commit 9e6b5fd (2017-03-09 02:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5815.3125 MB free)
Uptime: 2.4767025e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   45362159 s          0 s    9142704 s  2415022815 s         72 s
#2  3501 MHz  175766861 s          0 s    5633177 s  2293852160 s         10 s
#3  3501 MHz   40775873 s          0 s    4924715 s  2429829873 s         52 s
#4  3501 MHz   38353528 s          0 s    5074300 s  2432091189 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
