# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@44fe78ceef725270f02b6fea1a81e91cf4fc027f](https://github.com/JuliaLang/julia/commit/44fe78ceef725270f02b6fea1a81e91cf4fc027f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/44fe78ceef725270f02b6fea1a81e91cf4fc027f#commitcomment-24016245)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-09-01 vs 2017-08-31

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
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",256)]` | 1.05 (45%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 1.01 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",256)]` | 1.06 (45%)  | 1.02 (1%) :x: |
| `["problem","stockcorr","stockcorr"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","Int16","1:1")]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","Int8","1:1")]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Int32")]` | 1.04 (25%)  | 1.07 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 1.00 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","atan",("zero","Float32")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["shootout","regex_dna"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,10000))]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(16,))]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1599
Commit 44fe78c (2017-08-31 22:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   89971808 s          0 s   16028107 s  3871372348 s         90 s
       #2  3501 MHz  384304422 s          0 s   10362872 s  3592066288 s         16 s
       #3  3501 MHz   79096807 s          0 s    8992655 s  3899037353 s         75 s
       #4  3501 MHz   75596299 s          0 s    9176604 s  3902358867 s         17 s
       
  Memory: 31.383651733398438 GB (3214.19140625 MB free)
  Uptime: 3.9890555e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
