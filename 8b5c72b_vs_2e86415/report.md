# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8b5c72b2ad9ca5354139ccde2609598d6949ec91](https://github.com/JuliaLang/julia/commit/8b5c72b2ad9ca5354139ccde2609598d6949ec91) vs [JuliaLang/julia@2e864155d0498e73c35f92c91efb4b4799affea1](https://github.com/JuliaLang/julia/commit/2e864155d0498e73c35f92c91efb4b4799affea1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23240#issuecomment-331684673)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("prerend!",8)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.88 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.90 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.88 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.90 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 1.05 (15%)  | 1.28 (1%) :x: |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.63 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.89 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.74 (45%) :x: | 1.00 (1%)  |
| `["misc","julia",("macroexpand","evalpoly")]` | 1.07 (15%)  | 1.02 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem","json","parse_json"]` | 1.06 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 1.03 (15%)  | 0.90 (1%) :white_check_mark: |
| `["problem","stockcorr","stockcorr"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand!","MersenneTwister","Complex{Int128}")]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand!","MersenneTwister","Complex{UInt128}")]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Int32")]` | 0.88 (25%)  | 0.94 (1%) :white_check_mark: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.90 (25%)  | 1.07 (1%) :x: |
| `["scalar","predicate",("isfinite","Float64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 0.96 (15%)  | 1.11 (1%) :x: |
| `["shootout","pidigits"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,10000))]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint",(20000,10000))]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint",(20000,20000))]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["string","readuntil","backtracking"]` | 0.99 (15%)  | 1.46 (1%) :x: |
| `["string","readuntil","barbarian backtrack"]` | 1.00 (15%)  | 1.48 (1%) :x: |
| `["string","readuntil","no backtracking"]` | 0.99 (15%)  | 1.47 (1%) :x: |
| `["string","readuntil","target length 50000"]` | 0.98 (15%)  | 1.38 (1%) :x: |
| `["tuple","linear algebra",("matmat",(16,16),(16,16))]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(8,8))]` | 1.37 (15%) :x: | 1.00 (1%)  |

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
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1941
Commit 8b5c72b (2017-09-24 03:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   94189380 s          0 s   16736112 s  4064574740 s         92 s
       #2  3501 MHz  400170994 s          0 s   10738898 s  3774445442 s         20 s
       #3  3501 MHz   81396014 s          0 s    9259828 s  4095111580 s         76 s
       #4  3501 MHz   77752636 s          0 s    9450559 s  4098567613 s         18 s
       
  Memory: 31.383651733398438 GB (3697.30078125 MB free)
  Uptime: 4.1877747e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1937
Commit 2e86415 (2017-09-23 21:19 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   94271700 s          0 s   16745615 s  4065121009 s         92 s
       #2  3501 MHz  400743184 s          0 s   10750742 s  3774501397 s         20 s
       #3  3501 MHz   81475645 s          0 s    9267441 s  4095664176 s         76 s
       #4  3501 MHz   77850969 s          0 s    9457782 s  4099102140 s         18 s
       
  Memory: 31.383651733398438 GB (3437.6796875 MB free)
  Uptime: 4.1884153e7 sec
  Load Avg:  1.0830078125  1.03125  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
