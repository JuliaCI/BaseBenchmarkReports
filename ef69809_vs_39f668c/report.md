# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@ef6980915106e105db12967d89ad29ef1c290e03](https://github.com/pkofod/julia/commit/ef6980915106e105db12967d89ad29ef1c290e03) vs [JuliaLang/julia@39f668cc67bfa95782b27c78b1a5ab4d1d3c1d54](https://github.com/JuliaLang/julia/commit/39f668cc67bfa95782b27c78b1a5ab4d1d3c1d54)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24117#issuecomment-336382185)

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
| `["array","cat",("catnd_setind",5)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.41 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 2.40 (45%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Complex{Float64}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["problem","chaosgame","chaosgame"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.99 (25%)  | 1.02 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.93 (25%)  | 1.07 (1%) :x: |
| `["scalar","cos",("no reduction","zero","Float32")]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float64")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float32")]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float64")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","negative argument","Float32")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","negative argument","Float64")]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","positive argument","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","positive argument","Float64")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","zero","Float32")]` | 2.26 (15%) :x: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","zero","Float64")]` | 2.26 (15%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Diagonal",1000)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("A_mul_B","dense 5x500, sparse 500x500 -> dense 5x500")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B","dense 500x5, sparse 500x50 -> dense 5x50")]` | 1.05 (30%)  | 1.92 (1%) :x: |
| `["string","search","String"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","sincos"]`
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
- `["sparse","matmul"]`
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
Julia Version 0.7.0-DEV.2138
Commit ef69809 (2017-10-13 08:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   89772758 s          0 s   13948370 s  4240220013 s        183 s
       #2  3501 MHz  363909548 s          0 s   14997763 s  3967106840 s         66 s
       #3  3501 MHz   75199709 s          0 s    8555933 s  4268070945 s         86 s
       #4  3501 MHz   70378812 s          0 s    8445406 s  4273398221 s         32 s
       
  Memory: 31.383651733398438 GB (3188.5703125 MB free)
  Uptime: 4.3536766e7 sec
  Load Avg:  1.0419921875  1.02734375  1.046875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2136
Commit 39f668c (2017-10-13 07:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   89853433 s          0 s   13958664 s  4240946000 s        183 s
       #2  3501 MHz  364668211 s          0 s   15009610 s  3967155690 s         66 s
       #3  3501 MHz   75282423 s          0 s    8564125 s  4268799333 s         87 s
       #4  3501 MHz   70474157 s          0 s    8453182 s  4274114617 s         32 s
       
  Memory: 31.383651733398438 GB (3188.25390625 MB free)
  Uptime: 4.3544968e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
