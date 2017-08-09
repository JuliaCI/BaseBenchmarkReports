# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@616394f40bab7ea1b301f2acc377f83afbc97de9](https://github.com/JuliaLang/julia/commit/616394f40bab7ea1b301f2acc377f83afbc97de9) vs [JuliaLang/julia@44c53f410e52ff560727318def5466a22c83ec44](https://github.com/JuliaLang/julia/commit/44c53f410e52ff560727318def5466a22c83ec44)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23169#issuecomment-321137047)

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
| `["array","cat",("catnd",5)]` | 1.37 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 0.94 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.33 (15%) :x: | 1.21 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 1.33 (15%) :x: | 1.29 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 1.41 (15%) :x: | 1.29 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.11 (15%)  | 1.20 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.39 (15%) :x: | 1.21 (1%) :x: |
| `["array","convert",("Int","Complex{Float64}")]` | 2.54 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",8)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","index","7d"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","index","sub2ind"]` | 154899.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sum","3dsubarray")]` | 1.02 (50%)  | Inf (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 2.60 (50%) :x: | 1.08 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 1.48 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 1.49 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 2.33 (50%) :x: | 1.14 (1%) :x: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 2.33 (50%) :x: | 1.14 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.20 (50%)  | 1.10 (1%) :x: |
| `["array","index",("sumrange","Array{Float32,2}")]` | 0.97 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 1.01 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.03 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.02 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.01 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.02 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 2.63 (50%) :x: | 1.08 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.95 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.00 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.06 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.05 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.02 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.07 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumvector","100000:-1:1")]` | 1.06 (50%)  | 1.13 (1%) :x: |
| `["array","index",("sumvector","1:100000")]` | 1.05 (50%)  | 1.13 (1%) :x: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","BitArray{2}")]` | 3.29 (50%) :x: | 1.12 (1%) :x: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.03 (50%)  | 1.15 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.11 (50%)  | 1.15 (1%) :x: |
| `["array","reductions",("var","Float64")]` | 0.92 (15%)  | 0.83 (1%) :white_check_mark: |
| `["array","reductions",("var","Int64")]` | 0.99 (15%)  | 0.85 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Month")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 1.09 (45%)  | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["misc","parse","Int"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.32 (15%) :x: | 1.21 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["problem","simplex","simplex"]` | 1.00 (15%)  | 1.30 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.05 (15%)  | 1.11 (1%) :x: |
| `["random","collections",("rand!","ImplicitRNG","large String")]` | 1.00 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","ImplicitRNG","small String")]` | 1.00 (25%)  | 1.29 (1%) :x: |
| `["random","collections",("rand!","MersenneTwister","large String")]` | 1.01 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","MersenneTwister","small String")]` | 1.01 (25%)  | 1.29 (1%) :x: |
| `["random","collections",("rand!","RandomDevice","large String")]` | 1.02 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","RandomDevice","small String")]` | 1.00 (25%)  | 1.29 (1%) :x: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 1.21 (25%)  | 1.07 (1%) :x: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 1.01 (25%)  | 1.03 (1%) :x: |
| `["random","ranges",("RangeGenerator","UInt128","1:170141183460469231731687303715884105728")]` | 1.68 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt16","1:1")]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt8","1:1")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.05 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 0.93 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.06 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("rem type","Bool","Bool")]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 2.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 2.53 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 1.00 (15%)  | 0.65 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4095)]` | 0.60 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4096)]` | 0.61 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 0.98 (30%)  | 1.22 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.00 (30%)  | 1.22 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 0.98 (30%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.01 (30%)  | 1.13 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 2.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 3.63 (30%) :x: | 1.00 (1%)  |
| `["string","search","String"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(4,4),(4,4))]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.72 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1302
Commit 616394f (2017-08-09 02:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   79026138 s          0 s   12194887 s  3690429924 s        132 s
       #2  3501 MHz  313081108 s          0 s   13210802 s  3456865418 s         47 s
       #3  3501 MHz   67210729 s          0 s    7702278 s  3713373381 s         63 s
       #4  3501 MHz   62539570 s          0 s    7632776 s  3718467542 s         21 s
       
  Memory: 31.383651733398438 GB (3398.7109375 MB free)
  Uptime: 3.7899497e7 sec
  Load Avg:  0.990234375  1.013671875  1.04443359375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1300
Commit 44c53f4 (2017-08-09 02:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   79109164 s          0 s   12204261 s  3691029234 s        132 s
       #2  3501 MHz  313714910 s          0 s   13221880 s  3456914125 s         47 s
       #3  3501 MHz   67287032 s          0 s    7709702 s  3713983214 s         63 s
       #4  3501 MHz   62635051 s          0 s    7639911 s  3719058740 s         21 s
       
  Memory: 31.383651733398438 GB (2859.84765625 MB free)
  Uptime: 3.790644e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
