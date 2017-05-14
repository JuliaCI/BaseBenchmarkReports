# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e30ab0ed3ed50c4403f5a3f593f8a136eeb471c5](https://github.com/JuliaLang/julia/commit/e30ab0ed3ed50c4403f5a3f593f8a136eeb471c5) vs [JuliaLang/julia@6bdb3950bdf64152](https://github.com/JuliaLang/julia/commit/6bdb3950bdf64152)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21878)

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
| `["array","bool","boolarray_true_load!"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","BigInt","+")]` | 0.36 (40%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["scalar","intfuncs",("nextpow2","BigInt","-")]` | 0.22 (40%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","BigInt","+")]` | 0.76 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","BigInt","-")]` | 0.40 (40%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.80 (20%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.20 (15%) :x: | 1.00 (1%)  |

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
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
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
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
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
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-rc1.59
Commit e30ab0e (2017-05-14 18:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4877.59375 MB free)
Uptime: 3.043934e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63217837 s          0 s   11905140 s  2959944026 s         80 s
#2  3501 MHz  257805905 s          0 s    7469025 s  2776873075 s         12 s
#3  3501 MHz   56330288 s          0 s    6632845 s  2979501808 s         64 s
#4  3501 MHz   53386442 s          0 s    6789684 s  2982286761 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-rc1.0
Commit 6bdb395 (2017-05-07 00:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4671.515625 MB free)
Uptime: 3.0444764e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63299937 s          0 s   11914690 s  2960392704 s         80 s
#2  3501 MHz  258294772 s          0 s    7477454 s  2776917600 s         12 s
#3  3501 MHz   56424284 s          0 s    6641003 s  2979941348 s         64 s
#4  3501 MHz   53470992 s          0 s    6797884 s  2982735860 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
