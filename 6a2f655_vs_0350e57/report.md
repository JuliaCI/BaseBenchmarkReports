# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6a2f655449d6104b0d59189148f5c73c6e729416](https://github.com/JuliaLang/julia/commit/6a2f655449d6104b0d59189148f5c73c6e729416) vs [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18156)

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
| `["array","cat",("catnd",5)]` | 0.91 (15%)  | 0.94 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.83 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.96 (15%)  | 0.90 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.81 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumeach","100000000:-1:1")]` | 2.31 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000000")]` | 6.75 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","1:100000000")]` | 6.50 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 2.31 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000000")]` | 6.50 (40%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["problem","go","go_game"]` | 0.96 (15%)  | 0.82 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigFloat","BigFloat")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.28 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 1.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.32 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","integer",100000)]` | 0.41 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |

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
Julia Version 0.5.0-rc2+93
Commit 6a2f655 (2016-08-20 08:33 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10742.7578125 MB free)
Uptime: 7.332081e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12152482 s          0 s    2186062 s  717191466 s         23 s
#2  3501 MHz   28566372 s          0 s    1836525 s  702006310 s          6 s
#3  3501 MHz   10114702 s          0 s    1314538 s  721392286 s         12 s
#4  3501 MHz    8122778 s          0 s    1285049 s  723473879 s          2 s

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
Memory: 31.383651733398438 GB (10656.46484375 MB free)
Uptime: 7.336739e6 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12192200 s          0 s    2191932 s  717610416 s         23 s
#2  3501 MHz   28771011 s          0 s    1844272 s  702259127 s          6 s
#3  3501 MHz   10243033 s          0 s    1324708 s  721718984 s         12 s
#4  3501 MHz    8186578 s          0 s    1291411 s  723868933 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
