# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@086eca171b3f238996da5e4a51f237e4b670eec4](https://github.com/JuliaLang/julia/commit/086eca171b3f238996da5e4a51f237e4b670eec4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/086eca171b3f238996da5e4a51f237e4b670eec4#commitcomment-23810362)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-23 vs 2017-08-22

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.40 (45%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.10 (25%)  | 1.01 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 1.06 (25%)  | 1.07 (1%) :x: |
| `["scalar","acos",("0.5 <= abs(x) < 1","positive argument","Float32")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","positive argument","Float32")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.01 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 0.99 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 0.98 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 1.01 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 1.00 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 0.98 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.00 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.99 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 0.96 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.98 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 0.96 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.98 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.00 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.99 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.00 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.00 (50%)  | 1.07 (1%) :x: |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","positive argument","Float32")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","negative argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","positive argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","negative argument","Float32")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","negative argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","positive argument","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","negative argument","Float32")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","negative argument","Float64")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float64")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","negative argument","Float32")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","positive argument","Float64")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float32")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float64")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1454
Commit 086eca1 (2017-08-23 00:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   86902800 s          0 s   15621037 s  3798289340 s         90 s
       #2  3501 MHz  366591367 s          0 s    9990930 s  3533406120 s         15 s
       #3  3501 MHz   76259208 s          0 s    8722019 s  3825403758 s         75 s
       #4  3501 MHz   72852824 s          0 s    8912000 s  3828614126 s         17 s
       
  Memory: 31.383651733398438 GB (3134.96484375 MB free)
  Uptime: 3.9122644e7 sec
  Load Avg:  1.064453125  1.02978515625  1.04931640625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
