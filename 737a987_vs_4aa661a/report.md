# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@737a98705e984b90a3efeb220de41672bd733eea](https://github.com/JuliaLang/julia/commit/737a98705e984b90a3efeb220de41672bd733eea) vs [JuliaLang/julia@4aa661a0c1b6361bb254cbf974a79cdec0c08d2e](https://github.com/JuliaLang/julia/commit/4aa661a0c1b6361bb254cbf974a79cdec0c08d2e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23670#issuecomment-330964549)

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
| `["array","bool","boolarray_true_fill!"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 0.83 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_single!",8)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.85 (15%)  | 0.95 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.96 (15%)  | 0.98 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.97 (15%)  | 1.03 (1%) :x: |
| `["io","serialization",("serialize","Vector{String}")]` | 1.07 (15%)  | 1.06 (1%) :x: |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc","repeat",(200,24,1)]` | 6.54 (15%) :x: | 2.65 (1%) :x: |
| `["parallel","remotecall",("identity",1024)]` | 1.00 (15%)  | 0.91 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.92 (15%)  | 0.82 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.98 (15%)  | 0.96 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.96 (15%)  | 0.88 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.98 (15%)  | 0.84 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.00 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:2^10000)")]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.85 (25%)  | 1.07 (1%) :x: |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Bidiagonal",100)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Tridiagonal",100)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.20 (15%) :x: | 1.00 (1%)  |

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
- `["sparse","constructors"]`
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
Julia Version 0.6.1-pre.88
Commit 737a987 (2017-09-18 23:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2200.49609375 MB free)
Uptime: 4.1593105e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   85999631 s          0 s   13393941 s  4050608695 s        164 s
#2  3501 MHz  343435487 s          0 s   14267126 s  3794316194 s         55 s
#3  3501 MHz   71995440 s          0 s    8232873 s  4077288713 s         77 s
#4  3501 MHz   67304542 s          0 s    8108136 s  4082511546 s         26 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.1-pre.3
Commit 4aa661a (2017-09-14 17:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2559.171875 MB free)
Uptime: 4.1600429e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   86084892 s          0 s   13404792 s  4051241994 s        164 s
#2  3501 MHz  344109942 s          0 s   14278142 s  3794362116 s         55 s
#3  3501 MHz   72079900 s          0 s    8241345 s  4077927130 s         77 s
#4  3501 MHz   67403212 s          0 s    8116780 s  4083135934 s         26 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
