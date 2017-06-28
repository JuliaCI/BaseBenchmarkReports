# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@047a67ba7553795e04bef835d8980e9a88ff660b](https://github.com/JuliaLang/julia/commit/047a67ba7553795e04bef835d8980e9a88ff660b) vs [JuliaLang/julia@f4501ffcfade1877648b69c3d866c02df5a118d3](https://github.com/JuliaLang/julia/commit/f4501ffcfade1877648b69c3d866c02df5a118d3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22481#issuecomment-311572195)

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
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.15 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.33 (50%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BitArray{2}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.72 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumelt","BitArray{2}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.15 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.72 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","BitArray{2}")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.28 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.28 (45%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 0.90 (15%)  | 0.74 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 0.22 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.30 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.775
Commit 047a67b (2017-06-28 05:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71648032 s          0 s   13402477 s  3333360151 s         83 s
       #2  3501 MHz  301715981 s          0 s    8506947 s  3116134769 s         12 s
       #3  3501 MHz   64975942 s          0 s    7590967 s  3354150869 s         68 s
       #4  3501 MHz   61873833 s          0 s    7767855 s  3357061786 s         15 s
       
  Memory: 31.383651733398438 GB (2503.91796875 MB free)
  Uptime: 3.4283785e7 sec
  Load Avg:  1.05419921875  1.02880859375  1.04833984375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.772
Commit f4501ff (2017-06-28 05:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71725970 s          0 s   13411021 s  3333786586 s         83 s
       #2  3501 MHz  302174511 s          0 s    8514911 s  3116182608 s         12 s
       #3  3501 MHz   65067309 s          0 s    7598480 s  3354566369 s         68 s
       #4  3501 MHz   61952108 s          0 s    7775101 s  3357490638 s         15 s
       
  Memory: 31.383651733398438 GB (2486.8828125 MB free)
  Uptime: 3.4288934e7 sec
  Load Avg:  0.9248046875  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
