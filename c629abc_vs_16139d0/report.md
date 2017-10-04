# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c629abc414744ecee4810f352b60557f7d122b48](https://github.com/JuliaLang/julia/commit/c629abc414744ecee4810f352b60557f7d122b48) vs [JuliaLang/julia@16139d054e29ea63b797537927beee84da1b229d](https://github.com/JuliaLang/julia/commit/16139d054e29ea63b797537927beee84da1b229d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23986)

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
| `["array","bool","bitarray_true_fill!"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("prerend!",2048)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","DateFormat")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","NPDUpperTriangular",1024)]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.08 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.95 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","acos",("one","positive argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Int64}")]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","negative argument","Float32")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int64",4095)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("IV",1000)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",100)]` | 0.47 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 0.34 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["string","search","Char"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","search","String"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","searchindex","Char"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","searchindex","String"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(4,4))]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2049
Commit c629abc (2017-10-04 09:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88585629 s          0 s   13749530 s  4164413843 s        178 s
       #2  3501 MHz  358273566 s          0 s   14749215 s  3895787272 s         63 s
       #3  3501 MHz   74272570 s          0 s    8470742 s  4191739504 s         84 s
       #4  3501 MHz   69521867 s          0 s    8344098 s  4197019672 s         30 s
       
  Memory: 31.383651733398438 GB (3384.30859375 MB free)
  Uptime: 4.2763178e7 sec
  Load Avg:  1.0830078125  1.03125  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2046
Commit 16139d0 (2017-10-04 06:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88666555 s          0 s   13759206 s  4165061826 s        178 s
       #2  3501 MHz  358947220 s          0 s   14760938 s  3895842644 s         63 s
       #3  3501 MHz   74353804 s          0 s    8478512 s  4192391156 s         84 s
       #4  3501 MHz   69621526 s          0 s    8351933 s  4197653078 s         30 s
       
  Memory: 31.383651733398438 GB (2942.39453125 MB free)
  Uptime: 4.2770593e7 sec
  Load Avg:  1.03857421875  1.02685546875  1.04638671875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
