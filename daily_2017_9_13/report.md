# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@518c0663ff9a2c43c3b83f7ee695a31bbcda9996](https://github.com/JuliaLang/julia/commit/518c0663ff9a2c43c3b83f7ee695a31bbcda9996)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/518c0663ff9a2c43c3b83f7ee695a31bbcda9996#commitcomment-24266743)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-09-13 vs 2017-09-11

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("append!",256)]` | 0.98 (15%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 0.44 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.25 (15%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.90 (15%)  | 0.90 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.91 (15%)  | 0.86 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.90 (15%)  | 0.96 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.90 (15%)  | 0.90 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.89 (15%)  | 0.86 (1%) :white_check_mark: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 0.54 (25%) :white_check_mark: | 0.99 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Int32")]` | 1.08 (25%)  | 0.94 (1%) :white_check_mark: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 1.25 (25%) :x: | 1.07 (1%) :x: |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","positive argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","negative argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","positive argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","sin_kernel")]` | 1.77 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 0.37 (15%) :white_check_mark: | 0.49 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.77 (15%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["sparse","transpose",("adjoint!",(20000,10000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 0.45 (40%) :white_check_mark: | 0.99 (1%)  |
| `["string","replace"]` | 0.26 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.1769
Commit 518c066 (2017-09-13 01:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92382386 s          0 s   16389143 s  3971913748 s         92 s
       #2  3501 MHz  390489093 s          0 s   10543559 s  3689253960 s         18 s
       #3  3501 MHz   80157116 s          0 s    9121656 s  4001414822 s         76 s
       #4  3501 MHz   76611609 s          0 s    9317770 s  4004763874 s         17 s
       
  Memory: 31.383651733398438 GB (6844.31640625 MB free)
  Uptime: 4.0926638e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
