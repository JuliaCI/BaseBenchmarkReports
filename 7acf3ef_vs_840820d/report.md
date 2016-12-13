# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@7acf3efa6bb408422bf423f7239367bb6bdb5974](https://github.com/stevengj/julia/commit/7acf3efa6bb408422bf423f7239367bb6bdb5974) vs [JuliaLang/julia@840820d60005d0554ce48fac4b86ece8aacd8777](https://github.com/JuliaLang/julia/commit/840820d60005d0554ce48fac4b86ece8aacd8777)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17623#issuecomment-266637383)

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
| `["array","index","2d"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.29 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.10 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.14 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.61 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 1.24 (15%) :x: | 1.07 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.20 (15%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 1.37 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.94 (45%) :x: | 1.04 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.67 (45%) :x: | 1.04 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.13 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.35 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.13 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.36 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 1.34 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 1.12 (45%)  | 1.01 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 0.79 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","norm","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","norm","Float64")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 1.97 (15%) :x: | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 5.01 (30%) :x: | 1.40 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 4.96 (30%) :x: | 1.32 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 3.89 (30%) :x: | 1.11 (1%) :x: |

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
Julia Version 0.6.0-dev.1582
Commit 7acf3ef (2016-12-13 04:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11085.234375 MB free)
Uptime: 1.7254587e7 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26367745 s          0 s    4412153 s  1691183906 s         52 s
#2  3501 MHz   75648685 s          0 s    5376578 s  1641580102 s         19 s
#3  3501 MHz   23225181 s          0 s    2959953 s  1698490911 s         28 s
#4  3501 MHz   19147846 s          0 s    2861190 s  1702806334 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1553
Commit 840820d (2016-12-13 04:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10798.98046875 MB free)
Uptime: 1.7260487e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26419436 s          0 s    4419409 s  1691713127 s         52 s
#2  3501 MHz   75988917 s          0 s    5385178 s  1641820664 s         19 s
#3  3501 MHz   23266649 s          0 s    2966066 s  1699032589 s         28 s
#4  3501 MHz   19272786 s          0 s    2871392 s  1703260732 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
