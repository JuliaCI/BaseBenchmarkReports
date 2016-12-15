# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@12e4e7c51f6cfcec242753a1bdd90ed93833624b](https://github.com/stevengj/julia/commit/12e4e7c51f6cfcec242753a1bdd90ed93833624b) vs [JuliaLang/julia@38ff38c3328858df042b7e0fcb72385d7f4c4a7a](https://github.com/JuliaLang/julia/commit/38ff38c3328858df042b7e0fcb72385d7f4c4a7a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17623#issuecomment-267419289)

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
| `["array","index","5d"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.29 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.11 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.14 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.59 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.91 (15%)  | 0.55 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.90 (15%)  | 0.68 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 0.76 (45%)  | 0.84 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 0.61 (45%)  | 0.60 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_devec"]` | 0.99 (15%)  | 0.50 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.69 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","norm","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.35 (15%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 0.67 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.72 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.75 (30%)  | 0.54 (1%) :white_check_mark: |

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
Julia Version 0.6.0-dev.1625
Commit 12e4e7c (2016-12-15 18:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13422.14453125 MB free)
Uptime: 1.7481704e7 sec
Load Avg:  0.9228515625  0.998046875  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   23504667 s          0 s    5595920 s  1714065279 s         54 s
#2  3501 MHz   72945569 s          0 s    3397722 s  1670782129 s          8 s
#3  3501 MHz   22940482 s          0 s    2954761 s  1721465900 s         34 s
#4  3501 MHz   20133778 s          0 s    2994137 s  1724225001 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1576
Commit 38ff38c (2016-12-15 18:04 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13175.23828125 MB free)
Uptime: 1.7487599e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   23543304 s          0 s    5602970 s  1714607047 s         54 s
#2  3501 MHz   73355897 s          0 s    3409047 s  1670949662 s          8 s
#3  3501 MHz   23011426 s          0 s    2962741 s  1721975810 s         34 s
#4  3501 MHz   20171580 s          0 s    2999990 s  1724770263 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
