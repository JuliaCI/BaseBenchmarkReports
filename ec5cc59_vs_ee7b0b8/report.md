# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ec5cc5904b9c24594d005ef2e78c4088794094e8](https://github.com/JuliaLang/julia/commit/ec5cc5904b9c24594d005ef2e78c4088794094e8) vs [JuliaLang/julia@ee7b0b8dd342e16243e52656272d00acd9236e7c](https://github.com/JuliaLang/julia/commit/ee7b0b8dd342e16243e52656272d00acd9236e7c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20621#issuecomment-331880613)

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
| `["array","index","2d"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","ImplicitFloat64")]` | 1.72 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randexp","ImplicitRNG","Float64")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["string","readuntil","backtracking"]` | 0.00 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["string","readuntil","barbarian backtrack"]` | 0.01 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["string","readuntil","no backtracking"]` | 0.01 (15%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["string","readuntil","target length 1"]` | 0.18 (15%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["string","readuntil","target length 1000"]` | 0.10 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["string","readuntil","target length 2"]` | 0.26 (15%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["string","readuntil","target length 50000"]` | 0.11 (15%) :white_check_mark: | 0.03 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.1958
Commit ec5cc59 (2017-09-25 11:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   94506494 s          0 s   16785978 s  4076352663 s         92 s
       #2  3501 MHz  402608807 s          0 s   10790763 s  3784124558 s         20 s
       #3  3501 MHz   81738071 s          0 s    9297396 s  4106900957 s         76 s
       #4  3501 MHz   78119662 s          0 s    9485570 s  4110335760 s         18 s
       
  Memory: 31.383651733398438 GB (3161.17578125 MB free)
  Uptime: 4.1999521e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1948
Commit ee7b0b8 (2017-09-25 10:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   94585885 s          0 s   16795541 s  4076977713 s         92 s
       #2  3501 MHz  403279319 s          0 s   10802117 s  3784158937 s         20 s
       #3  3501 MHz   81817492 s          0 s    9304978 s  4107530021 s         76 s
       #4  3501 MHz   78199523 s          0 s    9493060 s  4110964748 s         18 s
       
  Memory: 31.383651733398438 GB (3076.53515625 MB free)
  Uptime: 4.2006689e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
