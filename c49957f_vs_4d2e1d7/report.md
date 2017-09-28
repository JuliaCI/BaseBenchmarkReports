# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c49957fae637be48180c6c898bb78e1bd4ddce06](https://github.com/JuliaLang/julia/commit/c49957fae637be48180c6c898bb78e1bd4ddce06) vs [JuliaLang/julia@4d2e1d7cdf4cbce4650cbe6b6c5ebde5b86cca10](https://github.com/JuliaLang/julia/commit/4d2e1d7cdf4cbce4650cbe6b6c5ebde5b86cca10)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23240#issuecomment-332846005)

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
| `["array","growth",("append!",8)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("prerend!",8)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.88 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.89 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.86 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.86 (50%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 1.05 (15%)  | 1.28 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.85 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.70 (45%) :x: | 1.00 (1%)  |
| `["misc","julia",("macroexpand","evalpoly")]` | 1.05 (15%)  | 1.02 (1%) :x: |
| `["problem","json","parse_json"]` | 1.08 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","spellcheck","spellcheck"]` | 1.03 (15%)  | 0.90 (1%) :white_check_mark: |
| `["random","collections",("rand!","MersenneTwister","large IntSet")]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.42 (25%) :x: | 1.02 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 1.44 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand!","MersenneTwister","Complex{Int128}")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand!","MersenneTwister","Complex{UInt128}")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Complex{UInt64}")]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","Char","Int64")]` | 1.72 (40%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) > 2.0^20*π/2","positive argument","Float64")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 1.03 (15%)  | 1.11 (1%) :x: |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","constructors",("Bidiagonal",100)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","constructors",("IV",10)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.75 (40%) :x: | 1.00 (1%)  |
| `["string","readuntil","backtracking"]` | 1.00 (15%)  | 1.46 (1%) :x: |
| `["string","readuntil","barbarian backtrack"]` | 1.02 (15%)  | 1.48 (1%) :x: |
| `["string","readuntil","no backtracking"]` | 1.02 (15%)  | 1.47 (1%) :x: |
| `["string","readuntil","target length 50000"]` | 1.14 (15%)  | 1.38 (1%) :x: |
| `["tuple","reduction",("sum",(16,16))]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
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
Julia Version 0.7.0-DEV.1987
Commit c49957f (2017-09-28 13:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87212658 s          0 s   13578714 s  4115748839 s        172 s
       #2  3501 MHz  350257594 s          0 s   14485562 s  3853862532 s         59 s
       #3  3501 MHz   72849838 s          0 s    8329174 s  4143012009 s         80 s
       #4  3501 MHz   68184898 s          0 s    8213558 s  4148190556 s         28 s
       
  Memory: 31.383651733398438 GB (3215.578125 MB free)
  Uptime: 4.2260042e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1983
Commit 4d2e1d7 (2017-09-28 07:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87293631 s          0 s   13588634 s  4116306557 s        172 s
       #2  3501 MHz  350859830 s          0 s   14496929 s  3853899325 s         60 s
       #3  3501 MHz   72935233 s          0 s    8336864 s  4143569314 s         81 s
       #4  3501 MHz   68265754 s          0 s    8221232 s  4148752598 s         28 s
       
  Memory: 31.383651733398438 GB (2905.0390625 MB free)
  Uptime: 4.2266554e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
