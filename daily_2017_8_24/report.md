# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@98c7a06f1a90cd7ee17d280ccb0d871c497aa025](https://github.com/JuliaLang/julia/commit/98c7a06f1a90cd7ee17d280ccb0d871c497aa025)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/98c7a06f1a90cd7ee17d280ccb0d871c497aa025#commitcomment-23837189)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-24 vs 2017-08-23

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
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",256)]` | 0.97 (15%)  | 0.93 (1%) :white_check_mark: |
| `["array","growth",("prerend!",2048)]` | 1.12 (15%)  | 1.11 (1%) :x: |
| `["array","growth",("prerend!",256)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["io","read","readstring"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 1.73 (45%) :x: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["random","collections",("rand","RandomDevice","small IntSet")]` | 3.51 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.01 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.00 (25%)  | 0.97 (1%) :white_check_mark: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.98 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","acos",("0.5 <= abs(x) < 1","negative argument","Float32")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= abs(x) < 1","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= abs(x) < 1","positive argument","Float32")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= abs(x) < 1","positive argument","Float64")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","negative argument","Float32")]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","negative argument","Float64")]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","positive argument","Float32")]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","positive argument","Float64")]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","negative argument","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","positive argument","Float32")]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","positive argument","Float64")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","negative argument","Float64")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","positive argument","Float64")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","negative argument","Float32")]` | 0.21 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","negative argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","positive argument","Float32")]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","positive argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.51 (30%) :x: | 1.00 (1%)  |
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
Julia Version 0.7.0-DEV.1470
Commit 98c7a06 (2017-08-24 00:59 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87330120 s          0 s   15670935 s  3805464942 s         90 s
       #2  3501 MHz  368743501 s          0 s   10042304 s  3538871575 s         15 s
       #3  3501 MHz   76654436 s          0 s    8759480 s  3832640824 s         75 s
       #4  3501 MHz   73284344 s          0 s    8952323 s  3835811484 s         17 s
       
  Memory: 31.383651733398438 GB (3346.703125 MB free)
  Uptime: 3.9199392e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
