# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4ba21aa57f57b9e42eeba5886d9dec772281e9f2](https://github.com/JuliaLang/julia/commit/4ba21aa57f57b9e42eeba5886d9dec772281e9f2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/4ba21aa57f57b9e42eeba5886d9dec772281e9f2#commitcomment-19422829)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-10-14 vs 2016-10-13

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
| `["array","cat",("hcat",5)]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 1.85 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 1.91 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 2.03 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.00 (15%)  | 0.96 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 1.02 (15%)  | 0.94 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 1.02 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 1.00 (15%)  | 0.95 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.01 (15%)  | 0.94 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.970
Commit 4ba21aa (2016-10-13 23:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15790.9296875 MB free)
Uptime: 1.2069444e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18989105 s          0 s    4088850 s  1180434258 s         36 s
#2  3501 MHz   52616400 s          0 s    2580824 s  1150976035 s          5 s
#3  3501 MHz   17947230 s          0 s    2246678 s  1186172453 s         24 s
#4  3501 MHz   15577785 s          0 s    2261991 s  1188508387 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
