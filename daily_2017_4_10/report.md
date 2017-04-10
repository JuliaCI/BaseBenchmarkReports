# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7c1e5af84c8c85b35624c7462c112b075a69defa](https://github.com/JuliaLang/julia/commit/7c1e5af84c8c85b35624c7462c112b075a69defa)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/7c1e5af84c8c85b35624c7462c112b075a69defa#commitcomment-21694197)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-04-10 vs 2017-04-09

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
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.41 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.63 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 0.35 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 0.38 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 0.39 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 0.59 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",10)]` | 0.74 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",3)]` | 0.41 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",5)]` | 0.72 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 1.39 (25%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.beta.85
Commit 7c1e5af (2017-04-09 16:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2325.00390625 MB free)
Uptime: 2.7447275e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53190146 s          0 s   10387377 s  2673175808 s         74 s
#2  3501 MHz  211907266 s          0 s    6383155 s  2524838837 s         11 s
#3  3501 MHz   47135726 s          0 s    5649711 s  2690628060 s         57 s
#4  3501 MHz   44575084 s          0 s    5783237 s  2693062786 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
