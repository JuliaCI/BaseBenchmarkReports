# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@31216d9e0e3bd67060fc48a51c1a310bd52e5929](https://github.com/stevengj/julia/commit/31216d9e0e3bd67060fc48a51c1a310bd52e5929) vs [JuliaLang/julia@bfc72b6fe913236ccb2bdd1ef254bceccb0cc31a](https://github.com/JuliaLang/julia/commit/bfc72b6fe913236ccb2bdd1ef254bceccb0cc31a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17623#issuecomment-267039428)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.29 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.10 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.14 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.61 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 1.16 (15%) :x: | 1.04 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.15 (15%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 1.27 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.47 (45%) :x: | 1.04 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.39 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.11 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.31 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.10 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.31 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 1.31 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 1.15 (45%)  | 1.01 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 1.55 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.55 (45%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 0.83 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","norm","Float64")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("significand","subnorm","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 2.01 (15%) :x: | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 5.18 (30%) :x: | 1.40 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 4.65 (30%) :x: | 1.32 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 3.75 (30%) :x: | 1.11 (1%) :x: |
| `["string","join"]` | 1.71 (40%) :x: | 1.00 (1%)  |

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
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1600
Commit 31216d9 (2016-12-14 13:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13924.88671875 MB free)
Uptime: 1.7375342e7 sec
Load Avg:  1.0166015625  1.02197265625  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   23038766 s          0 s    5527042 s  1703997248 s         54 s
#2  3501 MHz   70768578 s          0 s    3337773 s  1662388708 s          8 s
#3  3501 MHz   22680783 s          0 s    2916096 s  1711134655 s         33 s
#4  3501 MHz   19612425 s          0 s    2941436 s  1714168249 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1563
Commit bfc72b6 (2016-12-14 10:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13677.8984375 MB free)
Uptime: 1.7381961e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   23092694 s          0 s    5534861 s  1704595264 s         54 s
#2  3501 MHz   71253953 s          0 s    3352883 s  1662549671 s          8 s
#3  3501 MHz   22723186 s          0 s    2922149 s  1711747257 s         34 s
#4  3501 MHz   19657681 s          0 s    2948320 s  1714777437 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
