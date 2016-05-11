# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6fccad64cda477d01ac472ff24b190d5a199b54f](https://github.com/JuliaLang/julia/commit/6fccad64cda477d01ac472ff24b190d5a199b54f) vs [JuliaLang/julia@c9d405156f8c13a2b81f268529fec3ecf9ac651a](https://github.com/JuliaLang/julia/commit/c9d405156f8c13a2b81f268529fec3ecf9ac651a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16260#issuecomment-218431340)

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
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 1.23 (40.00%)  | 2.00 (1.00%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.16 (40.00%) :x: | Inf (1.00%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.10 (40.00%) :x: | Inf (1.00%) :x: |
| `["problem","imdb","centrality"]` | 1.03 (15.00%)  | 1.02 (1.00%) :x: |
| `["problem","spellcheck"]` | 0.94 (15.00%)  | 1.03 (1.00%) :x: |
| `["shootout","k_nucleotide"]` | 0.99 (15.00%)  | 1.13 (1.00%) :x: |
| `["sparse","index",("spmat","integer",100)]` | 1.18 (15.00%) :x: | 1.00 (1.00%)  |
| `["sparse","index",("spmat","splogical",10)]` | 1.23 (15.00%) :x: | 1.17 (1.00%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 1.04 (15.00%)  | 1.17 (1.00%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.01 (15.00%)  | 1.09 (1.00%) :x: |

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
- `["io"]`
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
- `["problem"]`
- `["problem","seismic"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
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
Julia Version 0.5.0-dev+4035
Commit 6fccad6 (2016-05-11 11:15 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22136.5859375 MB free)
Uptime: 498895.0 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     532113 s          0 s     113125 s   49133071 s          1 s
#2  3501 MHz    1219243 s          0 s      99954 s   48516550 s          0 s
#3  3501 MHz     516853 s          0 s      76653 s   49271565 s          0 s
#4  3501 MHz     435052 s          0 s      72135 s   49357132 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4032
Commit c9d4051 (2016-05-10 19:55 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22099.46484375 MB free)
Uptime: 503512.0 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     608445 s          0 s     121093 s   49509086 s          1 s
#2  3501 MHz    1415020 s          0 s     106466 s   48775353 s          0 s
#3  3501 MHz     610382 s          0 s      84163 s   49631442 s          0 s
#4  3501 MHz     501715 s          0 s      79393 s   49744356 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
