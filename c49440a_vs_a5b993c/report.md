# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c49440a05470275d99c5e1f861c43bac68ce0969](https://github.com/JuliaLang/julia/commit/c49440a05470275d99c5e1f861c43bac68ce0969) vs [JuliaLang/julia@a5b993c43074ea45288531b1cdc74bc51f663507](https://github.com/JuliaLang/julia/commit/a5b993c43074ea45288531b1cdc74bc51f663507)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21277#issuecomment-291769914)

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
| `["array","cat",("catnd",5)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 1.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.beta.33
Commit c49440a (2017-04-05 06:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5739.25 MB free)
Uptime: 2.7026098e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   55094153 s          0 s    8552456 s  2633246233 s         79 s
#2  3501 MHz  204284138 s          0 s    9377444 s  2484489058 s         29 s
#3  3501 MHz   46101776 s          0 s    5400155 s  2649903074 s         43 s
#4  3501 MHz   41765098 s          0 s    5339739 s  2654551069 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.30
Commit a5b993c (2017-04-05 04:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5570.82421875 MB free)
Uptime: 2.7031451e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   55175465 s          0 s    8562437 s  2633688279 s         79 s
#2  3501 MHz  204773391 s          0 s    9386062 s  2484525974 s         29 s
#3  3501 MHz   46188703 s          0 s    5408587 s  2650342295 s         43 s
#4  3501 MHz   41849475 s          0 s    5348024 s  2654993186 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
