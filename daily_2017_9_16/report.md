# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c23d6bc0db0bddcc9d83a1d3609975a5dcc8fff8](https://github.com/JuliaLang/julia/commit/c23d6bc0db0bddcc9d83a1d3609975a5dcc8fff8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/c23d6bc0db0bddcc9d83a1d3609975a5dcc8fff8#commitcomment-24337036)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-09-16 vs 2017-09-15

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
| `["array","index","sub2ind"]` | 208189.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.88 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.77 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.78 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.97 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.81 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.84 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.96 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.97 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.76 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.81 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.91 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.97 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.79 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.82 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000:-1:1")]` | 1.10 (50%)  | 1.13 (1%) :x: |
| `["array","index",("sumvector","1:100000")]` | 1.11 (50%)  | 1.13 (1%) :x: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.25 (50%)  | 1.15 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["array","reductions",("var","Float64")]` | 0.92 (15%)  | 0.83 (1%) :white_check_mark: |
| `["array","reductions",("var","Int64")]` | 1.00 (15%)  | 0.85 (1%) :white_check_mark: |
| `["array","setindex!",("setindex!",5)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 1.01 (15%)  | 1.10 (1%) :x: |
| `["random","collections",("rand!","ImplicitRNG","large String")]` | 1.00 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","ImplicitRNG","small String")]` | 1.01 (25%)  | 1.29 (1%) :x: |
| `["random","collections",("rand!","MersenneTwister","large String")]` | 1.00 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","MersenneTwister","small String")]` | 1.01 (25%)  | 1.29 (1%) :x: |
| `["random","collections",("rand!","RandomDevice","large String")]` | 1.02 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","RandomDevice","small String")]` | 1.02 (25%)  | 1.29 (1%) :x: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 1.05 (25%)  | 1.08 (1%) :x: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 0.98 (25%)  | 1.03 (1%) :x: |
| `["random","types",("randn","ImplicitRNG","Float64")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 2.69 (25%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 2.85 (25%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 1.00 (15%)  | 0.65 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.01 (30%)  | 1.22 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.02 (30%)  | 1.22 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 0.96 (30%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.00 (30%)  | 1.13 (1%) :x: |
| `["sparse","constructors",("Diagonal",10)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Diagonal",100)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("SymTridiagonal",10)]` | 1.05 (15%)  | 1.07 (1%) :x: |
| `["sparse","constructors",("Tridiagonal",10)]` | 1.11 (15%)  | 1.07 (1%) :x: |
| `["sparse","index",("spmat","integer",10)]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",100)]` | 2.17 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 2.98 (30%) :x: | 1.00 (1%)  |
| `["string","search","String"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 2.18 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 1.42 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1799
Commit c23d6bc (2017-09-15 20:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92617311 s          0 s   16448330 s  3997545727 s         92 s
       #2  3501 MHz  392284964 s          0 s   10589462 s  3713386290 s         19 s
       #3  3501 MHz   80396389 s          0 s    9163106 s  4027107997 s         76 s
       #4  3501 MHz   76864273 s          0 s    9351796 s  4030455134 s         18 s
       
  Memory: 31.383651733398438 GB (5585.625 MB free)
  Uptime: 4.1186544e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
