# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e331737463141abcdb427c8f801fbe1d18851af9](https://github.com/JuliaLang/julia/commit/e331737463141abcdb427c8f801fbe1d18851af9) vs [JuliaLang/julia@ffb66cd507b7fc7c66d9069858caa5404366276e](https://github.com/JuliaLang/julia/commit/ffb66cd507b7fc7c66d9069858caa5404366276e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23912#issuecomment-334054885)

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
| `["dates","parse",("Date","DateFormat")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 0.57 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.33 (15%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.39 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 2.39 (45%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.96 (15%)  | 0.90 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.93 (15%)  | 0.84 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.93 (15%)  | 0.95 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.95 (15%)  | 0.89 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.95 (15%)  | 0.85 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 0.43 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.99 (25%)  | 1.01 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.99 (25%)  | 1.01 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.86 (25%)  | 1.07 (1%) :x: |
| `["random","types",("randexp!","RandomDevice","Float64")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= abs(x) < 1","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","UInt64")]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float32")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float64")]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","tan",("medium","positive argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 0.68 (15%) :white_check_mark: | 0.49 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 1.01 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.84 (15%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["sparse","constructors",("Bidiagonal",1000)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","replace"]` | 0.43 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["tuple","reduction",("sum",(2,2))]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2051
Commit e331737 (2017-10-04 04:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88422172 s          0 s   13729790 s  4163114535 s        178 s
       #2  3501 MHz  356908776 s          0 s   14725714 s  3895688859 s         63 s
       #3  3501 MHz   74085334 s          0 s    8455354 s  4190455461 s         84 s
       #4  3501 MHz   69359614 s          0 s    8328584 s  4195710572 s         30 s
       
  Memory: 31.383651733398438 GB (2955.2109375 MB free)
  Uptime: 4.2748295e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2045
Commit ffb66cd (2017-10-04 02:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88503423 s          0 s   13739759 s  4163761938 s        178 s
       #2  3501 MHz  357583112 s          0 s   14737579 s  3895743534 s         63 s
       #3  3501 MHz   74185356 s          0 s    8462923 s  4191088564 s         84 s
       #4  3501 MHz   69442355 s          0 s    8336259 s  4196361025 s         30 s
       
  Memory: 31.383651733398438 GB (3142.32421875 MB free)
  Uptime: 4.2755711e7 sec
  Load Avg:  1.00439453125  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
