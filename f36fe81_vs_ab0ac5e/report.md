# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f36fe81fb908f95a307c81e647903ba148804bef](https://github.com/JuliaLang/julia/commit/f36fe81fb908f95a307c81e647903ba148804bef) vs [JuliaLang/julia@ab0ac5e31d155d6bb8d987788659cb1ea50d8e62](https://github.com/JuliaLang/julia/commit/ab0ac5e31d155d6bb8d987788659cb1ea50d8e62)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22826#issuecomment-325164779)

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
| `["array","convert",("Int","Complex{Float64}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["random","collections",("rand!","RandomDevice","'a':'z'")]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand!","RandomDevice","large Vector")]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand!","RandomDevice","small String")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(4,4))]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1521
Commit f36fe81 (2017-08-26 22:18 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83091815 s          0 s   12720582 s  3839444583 s        152 s
       #2  3501 MHz  336638368 s          0 s   13904704 s  3586338432 s         52 s
       #3  3501 MHz   70657155 s          0 s    8057587 s  3863469828 s         72 s
       #4  3501 MHz   65951466 s          0 s    7963986 s  3868654436 s         24 s
       
  Memory: 31.383651733398438 GB (5130.67578125 MB free)
  Uptime: 3.9439271e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1518
Commit ab0ac5e (2017-08-26 19:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83171263 s          0 s   12729902 s  3839983521 s        152 s
       #2  3501 MHz  337203809 s          0 s   13915918 s  3586391134 s         52 s
       #3  3501 MHz   70755624 s          0 s    8065622 s  3863992676 s         72 s
       #4  3501 MHz   66030606 s          0 s    7971811 s  3869196964 s         24 s
       
  Memory: 31.383651733398438 GB (4839.23046875 MB free)
  Uptime: 3.9445572e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
