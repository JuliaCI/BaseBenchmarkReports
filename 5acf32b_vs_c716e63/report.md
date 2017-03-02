# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5acf32b735346dda58c6f4041d3f8c6e77dfb98d](https://github.com/JuliaLang/julia/commit/5acf32b735346dda58c6f4041d3f8c6e77dfb98d) vs [JuliaLang/julia@c716e638bba74f52114c7adedfe4a653e42c40d0](https://github.com/JuliaLang/julia/commit/c716e638bba74f52114c7adedfe4a653e42c40d0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20853#issuecomment-283512184)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.68 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.96 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.47 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.83 (45%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 1.18 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 1.21 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 1.24 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 1.17 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 1.21 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{UInt64}")]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 1.23 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 1.19 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 1.22 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 1.26 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 1.17 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 1.22 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 1.24 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 1.20 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.30 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 1.42 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.23
Commit 5acf32b (2017-03-01 22:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8902.3359375 MB free)
Uptime: 2.4064524e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   41252287 s          0 s    8612314 s  2349628292 s         69 s
#2  3501 MHz  151770312 s          0 s    5177802 s  2248107035 s          9 s
#3  3501 MHz   37035167 s          0 s    4532111 s  2363761569 s         50 s
#4  3501 MHz   34645639 s          0 s    4677681 s  2365993580 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.18
Commit c716e63 (2017-03-01 18:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8561.93359375 MB free)
Uptime: 2.4070766e7 sec
Load Avg:  1.0048828125  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   41347197 s          0 s    8622213 s  2350145307 s         69 s
#2  3501 MHz  152337516 s          0 s    5186354 s  2248154794 s          9 s
#3  3501 MHz   37115826 s          0 s    4540498 s  2364295861 s         50 s
#4  3501 MHz   34725803 s          0 s    4686136 s  2366528564 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
