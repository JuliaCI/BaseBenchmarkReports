# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e181e2c1ddd8ed13f4a0d9b889b8ca3727d36af3](https://github.com/JuliaLang/julia/commit/e181e2c1ddd8ed13f4a0d9b889b8ca3727d36af3) vs [JuliaLang/julia@83007fb8c4c748fb23d38759daafd77fa1d56c2b](https://github.com/JuliaLang/julia/commit/83007fb8c4c748fb23d38759daafd77fa1d56c2b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23138#issuecomment-320467990)

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
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["random","collections",("rand!","ImplicitRNG","small IntSet")]` | 0.27 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand!","MersenneTwister","small IntSet")]` | 0.26 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand!","RandomDevice","small IntSet")]` | 0.02 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","large IntSet")]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","small IntSet")]` | 0.25 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","small IntSet")]` | 0.28 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","RandomDevice","small IntSet")]` | 0.37 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.01 (25%)  | 0.99 (1%) :white_check_mark: |
| `["tuple","reduction",("sum",(2,2))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
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
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1250
Commit e181e2c (2017-08-05 18:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82779268 s          0 s   14947285 s  3653005145 s         86 s
       #2  3501 MHz  340010084 s          0 s    9387958 s  3410129148 s         13 s
       #3  3501 MHz   71943715 s          0 s    8302697 s  3679670946 s         73 s
       #4  3501 MHz   68647739 s          0 s    8494024 s  3682758797 s         17 s
       
  Memory: 31.383651733398438 GB (6187.79296875 MB free)
  Uptime: 3.7617194e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1248
Commit 83007fb (2017-08-05 18:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82858409 s          0 s   14956069 s  3653515179 s         86 s
       #2  3501 MHz  340548102 s          0 s    9398746 s  3410180089 s         13 s
       #3  3501 MHz   72021166 s          0 s    8309932 s  3680185896 s         73 s
       #4  3501 MHz   68742932 s          0 s    8501166 s  3683256252 s         17 s
       
  Memory: 31.383651733398438 GB (5586.703125 MB free)
  Uptime: 3.7623197e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
