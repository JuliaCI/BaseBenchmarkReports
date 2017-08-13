# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4c5cc04156ba074a8baa028c2a8a41b9e70d56ee](https://github.com/JuliaLang/julia/commit/4c5cc04156ba074a8baa028c2a8a41b9e70d56ee)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/4c5cc04156ba074a8baa028c2a8a41b9e70d56ee#commitcomment-23619603)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-13 vs 2017-08-12

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
| `["array","index",("sumvector_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","'a':'z'")]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","large Vector")]` | 0.36 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","small Vector")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","'a':'z'")]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","large Vector")]` | 0.37 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","small Vector")]` | 0.43 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","ImplicitRNG","Int","1:1000")]` | 0.31 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","Int","1:1000")]` | 0.28 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","negative argument","Float64")]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","positive argument","Float64")]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.20 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","OneTo",10)]` | 0.99 (30%)  | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","OneTo",100)]` | 1.11 (30%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","col","OneTo",1000)]` | 0.95 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",1000)]` | 0.99 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","logical",10)]` | 1.06 (30%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 1.09 (30%)  | 1.05 (1%) :x: |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.38 (30%) :x: | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 1.07 (30%)  | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 1.11 (30%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.92 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","OneTo",100)]` | 1.07 (30%)  | 1.64 (1%) :x: |
| `["sparse","index",("spmat","row","OneTo",1000)]` | 0.98 (30%)  | 1.77 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.93 (30%)  | 1.77 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.12 (30%)  | 1.19 (1%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.03 (30%)  | 1.14 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.07 (30%)  | 1.64 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 0.97 (30%)  | 1.77 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.48 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1333
Commit 4c5cc04 (2017-08-12 13:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84814102 s          0 s   15256428 s  3713624392 s         88 s
       #2  3501 MHz  352112005 s          0 s    9672478 s  3460867056 s         13 s
       #3  3501 MHz   74074159 s          0 s    8508296 s  3740458007 s         74 s
       #4  3501 MHz   70720300 s          0 s    8692718 s  3743620343 s         17 s
       
  Memory: 31.383651733398438 GB (2985.9765625 MB free)
  Uptime: 3.824879e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
