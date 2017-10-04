# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7f252d5f85728776573264c2b28513d60348e38d](https://github.com/JuliaLang/julia/commit/7f252d5f85728776573264c2b28513d60348e38d) vs [JuliaLang/julia@16139d054e29ea63b797537927beee84da1b229d](https://github.com/JuliaLang/julia/commit/16139d054e29ea63b797537927beee84da1b229d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23939#issuecomment-334086602)

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
| `["array","growth",("append!",8)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.97 (15%)  | 3.00 (1%) :x: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 1.60 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","Int64","1:1")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","Int64","1:4294967295")]` | 1.65 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","Int64","1:4294967297")]` | 1.62 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt64","1:1")]` | 1.59 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt64","1:18446744073709551615")]` | 1.57 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt64","1:4294967295")]` | 1.65 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt64","1:4294967297")]` | 1.66 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.04 (25%)  | 1.02 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.03 (25%)  | 1.03 (1%) :x: |
| `["random","types",("rand","MersenneTwister","Int32")]` | 0.94 (25%)  | 1.07 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 1.03 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","negative argument","Float32")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float32")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(8,8))]` | 1.15 (15%) :x: | 1.00 (1%)  |

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
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
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
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","atan2"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2050
Commit 7f252d5 (2017-10-04 08:33 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96109617 s          0 s   17064200 s  4150194996 s         93 s
       #2  3501 MHz  414429163 s          0 s   11044488 s  3847942126 s         20 s
       #3  3501 MHz   83377876 s          0 s    9468423 s  4180994350 s         77 s
       #4  3501 MHz   79679852 s          0 s    9666672 s  4184491609 s         19 s
       
  Memory: 31.383651733398438 GB (4400.46484375 MB free)
  Uptime: 4.2758918e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2046
Commit 16139d0 (2017-10-04 06:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96190706 s          0 s   17073798 s  4150832695 s         93 s
       #2  3501 MHz  415106360 s          0 s   11055802 s  3847984218 s         20 s
       #3  3501 MHz   83459453 s          0 s    9475817 s  4181635828 s         77 s
       #4  3501 MHz   79760854 s          0 s    9674014 s  4185133917 s         19 s
       
  Memory: 31.383651733398438 GB (4127.26953125 MB free)
  Uptime: 4.276623e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
