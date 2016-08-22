# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b3b8ce2a5e80b63b9f76a17ae02f8813fc13b819](https://github.com/JuliaLang/julia/commit/b3b8ce2a5e80b63b9f76a17ae02f8813fc13b819) vs [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18156#issuecomment-241539747)

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
| `["array","cat",("catnd",5)]` | 0.89 (15%)  | 0.94 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.79 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.92 (15%)  | 0.90 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.81 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BitArray{2}")]` | 1.40 (40%)  | 2.00 (1%) :x: |
| `["array","index",("sumeach","BitArray{2}")]` | 1.50 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumelt","BitArray{2}")]` | 1.51 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 1.43 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumlinear","BitArray{2}")]` | 1.49 (40%) :x: | 2.00 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["problem","go","go_game"]` | 0.94 (15%)  | 0.82 (1%) :white_check_mark: |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 1.35 (1%) :x: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.31 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.36 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","integer",100000)]` | 0.44 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",10000)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",1000)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
Julia Version 0.5.0-rc2+117
Commit b3b8ce2 (2016-08-22 16:35 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13634.0703125 MB free)
Uptime: 7.547865e6 sec
Load Avg:  1.0029296875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13053107 s          0 s    2291531 s  737722254 s         24 s
#2  3501 MHz   30401698 s          0 s    1945214 s  721603841 s          6 s
#3  3501 MHz   11009563 s          0 s    1405516 s  741970961 s         12 s
#4  3501 MHz    8757524 s          0 s    1368704 s  744322416 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-rc2+0
Commit 0350e57 (2016-08-12 11:25 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13699.3359375 MB free)
Uptime: 7.552539e6 sec
Load Avg:  1.00732421875  1.01708984375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13095021 s          0 s    2297652 s  738140239 s         24 s
#2  3501 MHz   30612799 s          0 s    1952857 s  721851702 s          6 s
#3  3501 MHz   11122274 s          0 s    1414413 s  742315989 s         12 s
#4  3501 MHz    8829528 s          0 s    1376090 s  744709917 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
