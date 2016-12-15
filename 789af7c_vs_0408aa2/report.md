# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@789af7c56acf56601b510250fdec69950df4f7fa](https://github.com/stevengj/julia/commit/789af7c56acf56601b510250fdec69950df4f7fa) vs [JuliaLang/julia@0408aa206330fd2bd149efb58c0772740a0580aa](https://github.com/JuliaLang/julia/commit/0408aa206330fd2bd149efb58c0772740a0580aa)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17623#issuecomment-267230423)

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
| `["array","index","5d"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.28 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.11 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.13 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.56 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 1.10 (15%)  | 1.04 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.07 (15%)  | 1.03 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 0.77 (45%)  | 0.84 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 0.61 (45%)  | 0.60 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.80 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 2.01 (15%) :x: | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 0.68 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.71 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.70 (30%)  | 0.54 (1%) :white_check_mark: |

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
Julia Version 0.6.0-dev.1612
Commit 789af7c (2016-12-15 03:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10364.34375 MB free)
Uptime: 1.7429891e7 sec
Load Avg:  1.02880859375  1.0244140625  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26941456 s          0 s    4488613 s  1708028169 s         53 s
#2  3501 MHz   77942306 s          0 s    5470115 s  1656693458 s         20 s
#3  3501 MHz   23808847 s          0 s    3026297 s  1715361975 s         29 s
#4  3501 MHz   19631240 s          0 s    2926421 s  1719778062 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1565
Commit 0408aa2 (2016-12-15 03:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9948.59375 MB free)
Uptime: 1.7435813e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27006286 s          0 s    4497480 s  1708544784 s         53 s
#2  3501 MHz   78260014 s          0 s    5477308 s  1656959924 s         20 s
#3  3501 MHz   23918408 s          0 s    3035572 s  1715834601 s         29 s
#4  3501 MHz   19699554 s          0 s    2933606 s  1720294078 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
