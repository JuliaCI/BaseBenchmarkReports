# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fce2d689222c10ae735362dc67a8f6b973be55a3](https://github.com/JuliaLang/julia/commit/fce2d689222c10ae735362dc67a8f6b973be55a3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/fce2d689222c10ae735362dc67a8f6b973be55a3#commitcomment-24835759)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-10-08 vs 2017-10-07

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
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.97 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","types",("rand","MersenneTwister","Complex{UInt32}")]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","RandomDevice","ImplicitFloat64")]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","negative argument","Float64")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","positive argument","Float64")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float32")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","sin_kernel")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Diagonal",100)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","integer",1000)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["string","readuntil","target length 1"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2068
Commit fce2d68 (2017-10-07 21:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   97345269 s          0 s   17251727 s  4181535009 s         93 s
       #2  3501 MHz  423419814 s          0 s   11214596 s  3871636779 s         20 s
       #3  3501 MHz   84715328 s          0 s    9590380 s  4212391640 s         78 s
       #4  3501 MHz   80925338 s          0 s    9788271 s  4215982377 s         19 s
       
  Memory: 31.383651733398438 GB (3003.26171875 MB free)
  Uptime: 4.3087654e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
