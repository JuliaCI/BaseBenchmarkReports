# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a969c2a96da4775aa7ef7b6ac389c40892ddcfba](https://github.com/JuliaLang/julia/commit/a969c2a96da4775aa7ef7b6ac389c40892ddcfba)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a969c2a96da4775aa7ef7b6ac389c40892ddcfba#commitcomment-23991205)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-31 vs 2017-08-30

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
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","julia",("macroexpand","evalpoly")]` | 1.07 (15%)  | 1.04 (1%) :x: |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.03 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.03 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.03 (25%)  | 1.01 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 1.00 (25%)  | 1.07 (1%) :x: |
| `["scalar","atan",("very large","negative argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan",("very small","negative argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan",("very small","positive argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 1.61 (15%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Int64")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","UInt64")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Int64")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","UInt64")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Int64")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","UInt64")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(16,))]` | 1.33 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1586
Commit a969c2a (2017-08-30 21:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   89896509 s          0 s   16001126 s  3862785726 s         90 s
       #2  3501 MHz  383651070 s          0 s   10349235 s  3584018444 s         15 s
       #3  3501 MHz   79015162 s          0 s    8981587 s  3890416111 s         75 s
       #4  3501 MHz   75516893 s          0 s    9167905 s  3893730999 s         17 s
       
  Memory: 31.383651733398438 GB (3240.86328125 MB free)
  Uptime: 3.9803378e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
