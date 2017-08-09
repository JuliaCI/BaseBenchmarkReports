# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@44c53f410e52ff560727318def5466a22c83ec44](https://github.com/JuliaLang/julia/commit/44c53f410e52ff560727318def5466a22c83ec44)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/44c53f410e52ff560727318def5466a22c83ec44#commitcomment-23549457)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-09 vs 2017-08-08

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
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.47 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.45 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.45 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Float32,2}")]` | 0.31 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Float64,3}")]` | 0.78 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Int32,2}")]` | 0.31 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.89 (50%)  | 0.70 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.43 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.42 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Float32,2}")]` | 0.32 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Float64,3}")]` | 0.79 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Int32,2}")]` | 0.31 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.53 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.51 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.53 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.51 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.90 (50%)  | 0.70 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.53 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.46 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.43 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.97 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.51 (50%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.46 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.43 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","Int128","RangeGenerator(1:1)")]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","Int128","RangeGenerator(1:4294967295)")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","Int128","RangeGenerator(1:4294967297)")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:1)")]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:4294967295)")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:4294967297)")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.46 (30%) :x: | 1.00 (1%)  |
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
Julia Version 0.7.0-DEV.1300
Commit 44c53f4 (2017-08-09 02:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84163248 s          0 s   15133574 s  3680939138 s         87 s
       #2  3501 MHz  349152665 s          0 s    9574742 s  3430380570 s         13 s
       #3  3501 MHz   73375876 s          0 s    8434148 s  3707687304 s         73 s
       #4  3501 MHz   70068215 s          0 s    8624531 s  3710791706 s         17 s
       
  Memory: 31.383651733398438 GB (3654.88671875 MB free)
  Uptime: 3.7913181e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
