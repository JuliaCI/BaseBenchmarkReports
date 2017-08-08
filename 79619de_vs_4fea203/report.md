# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@79619de41e186e6495ac6ae9e32e51c202451cdd](https://github.com/JuliaLang/julia/commit/79619de41e186e6495ac6ae9e32e51c202451cdd) vs [JuliaLang/julia@4fea2033758793c6ba980695fe252eeb69fa5761](https://github.com/JuliaLang/julia/commit/4fea2033758793c6ba980695fe252eeb69fa5761)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23117#issuecomment-320810757)

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
| `["array","bool","bitarray_true_fill!"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("append!",8)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 1.23 (15%) :x: | 1.01 (1%)  |
| `["parallel","remotecall",("identity",4096)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",512)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",64)]` | 1.19 (15%) :x: | 1.01 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.00 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.02 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","negative argument","Float32")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float32")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float32","cos_kernel")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32","cos_kernel")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32","cos_kernel")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32","cos_kernel")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32","cos_kernel")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32","sin_kernel")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32","sin_kernel")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32","cos_kernel")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32","sin_kernel")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32","sin_kernel")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32","sin_kernel")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32","sin_kernel")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32","sin_kernel")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32","cos_kernel")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","cos_kernel")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","cos_kernel")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32","sin_kernel")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32","sin_kernel")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1284
Commit 79619de (2017-08-07 22:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78546864 s          0 s   12135427 s  3681232798 s        132 s
       #2  3501 MHz  309440903 s          0 s   13131331 s  3450842971 s         47 s
       #3  3501 MHz   66683925 s          0 s    7656862 s  3704190329 s         62 s
       #4  3501 MHz   62030422 s          0 s    7586203 s  3709267781 s         21 s
       
  Memory: 31.383651733398438 GB (4669.015625 MB free)
  Uptime: 3.780189e7 sec
  Load Avg:  1.08349609375  1.04248046875  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1283
Commit 4fea203 (2017-08-07 22:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78623201 s          0 s   12144955 s  3681839976 s        132 s
       #2  3501 MHz  310076574 s          0 s   13142328 s  3450891315 s         47 s
       #3  3501 MHz   66779423 s          0 s    7664382 s  3704782269 s         62 s
       #4  3501 MHz   62112652 s          0 s    7593215 s  3709873726 s         21 s
       
  Memory: 31.383651733398438 GB (4152.515625 MB free)
  Uptime: 3.7808848e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
