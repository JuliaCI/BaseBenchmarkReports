# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@2d8f5bfc05b1894b160b9fa3597f0e1fe54d1b93](https://github.com/JuliaLang/julia/commit/2d8f5bfc05b1894b160b9fa3597f0e1fe54d1b93)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/2d8f5bfc05b1894b160b9fa3597f0e1fe54d1b93#commitcomment-20209978)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-12-16 vs 2016-12-15

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
| `["array","growth",("append!",256)]` | 1.00 (15%)  | 0.96 (1%) :white_check_mark: |
| `["array","growth",("prerend!",256)]` | 1.02 (15%)  | 1.03 (1%) :x: |
| `["array","index","5d"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_devec"]` | 0.92 (15%)  | 0.02 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.84 (15%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["shootout","nbody_vec"]` | 1.35 (15%) :x: | 1.01 (1%) :x: |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 1.46 (40%) :x: | 1.00 (1%)  |

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
- `["broadcast","sparse"]`
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
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1583
Commit 2d8f5bf (2016-12-16 01:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9961.08203125 MB free)
Uptime: 1.7515448e7 sec
Load Avg:  1.01806640625  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27120528 s          0 s    4517133 s  1716359835 s         53 s
#2  3501 MHz   78906890 s          0 s    5508842 s  1664229269 s         20 s
#3  3501 MHz   24007914 s          0 s    3050155 s  1723690359 s         29 s
#4  3501 MHz   19969731 s          0 s    2956652 s  1727962093 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
