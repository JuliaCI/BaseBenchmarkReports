# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6fccad64cda477d01ac472ff24b190d5a199b54f](https://github.com/JuliaLang/julia/commit/6fccad64cda477d01ac472ff24b190d5a199b54f) vs [JuliaLang/julia@c9d405156f8c13a2b81f268529fec3ecf9ac651a](https://github.com/JuliaLang/julia/commit/c9d405156f8c13a2b81f268529fec3ecf9ac651a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16260#issuecomment-218490299)

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
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.11 (40.00%) :x: | Inf (1.00%) :x: |
| `["problem","imdb","centrality"]` | 1.03 (15.00%)  | 1.02 (1.00%) :x: |
| `["problem","spellcheck"]` | 0.94 (15.00%)  | 1.03 (1.00%) :x: |
| `["shootout","k_nucleotide"]` | 0.99 (15.00%)  | 1.13 (1.00%) :x: |
| `["sparse","index",("spmat","integer",100)]` | 1.18 (15.00%) :x: | 1.00 (1.00%)  |
| `["sparse","index",("spmat","splogical",10)]` | 1.22 (15.00%) :x: | 1.17 (1.00%) :x: |
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
Memory: 31.383651733398438 GB (22178.6484375 MB free)
Uptime: 512210.0 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     293018 s          0 s     137326 s   50651383 s          0 s
#2  3501 MHz     931022 s          0 s      47712 s   50231219 s          0 s
#3  3501 MHz     314194 s          0 s      96690 s   50756554 s          0 s
#4  3501 MHz     289122 s          0 s      42960 s   50874080 s          1 s

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
Memory: 31.383651733398438 GB (22142.921875 MB free)
Uptime: 516826.0 sec
Load Avg:  1.03076171875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     354271 s          0 s     145396 s   51042283 s          0 s
#2  3501 MHz    1149772 s          0 s      54747 s   50466616 s          0 s
#3  3501 MHz     415951 s          0 s     104623 s   51107777 s          0 s
#4  3501 MHz     339897 s          0 s      49067 s   51278386 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
