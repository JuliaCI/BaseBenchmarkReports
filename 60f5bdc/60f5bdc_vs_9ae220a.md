# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@60f5bdcdc94bfa20b48695eafa00c07154316bc1](https://github.com/JuliaLang/julia/commit/60f5bdcdc94bfa20b48695eafa00c07154316bc1) vs [JuliaLang/julia@9ae220a62c63afaf49c9222fb6695d167ba3f043](https://github.com/JuliaLang/julia/commit/9ae220a62c63afaf49c9222fb6695d167ba3f043)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16260#issuecomment-217904522)

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
| `["array","cat",("vcat",5)]` | 1.39 (15.00%) :x: | 1.00 (1.00%)  |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 2.12 (30.00%) :x: | 1.00 (1.00%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.57 (30.00%) :x: | 1.00 (1.00%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 3.13 (40.00%) :x: | 1.00 (1.00%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.93 (40.00%) :x: | 1.00 (1.00%)  |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 1.26 (40.00%)  | 2.00 (1.00%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.12 (40.00%) :x: | Inf (1.00%) :x: |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.05 (40.00%) :x: | Inf (1.00%) :x: |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.45 (40.00%) :white_check_mark: | 1.00 (1.00%)  |
| `["problem","imdb","centrality"]` | 1.03 (15.00%)  | 1.02 (1.00%) :x: |
| `["problem","spellcheck"]` | 0.93 (15.00%)  | 1.03 (1.00%) :x: |
| `["shootout","k_nucleotide"]` | 1.03 (15.00%)  | 1.13 (1.00%) :x: |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.30 (15.00%) :x: | 1.00 (1.00%)  |
| `["sparse","index",("spmat","splogical",10)]` | 1.19 (15.00%) :x: | 1.17 (1.00%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 1.03 (15.00%)  | 1.17 (1.00%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.00 (15.00%)  | 1.09 (1.00%) :x: |

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
Julia Version 0.5.0-dev+3997
Commit 60f5bdc (2016-05-09 15:48 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22126.39453125 MB free)
Uptime: 342220.0 sec
Load Avg:  1.0029296875  1.001953125  0.96337890625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     377848 s          0 s      86984 s   33672836 s          1 s
#2  3501 MHz     731806 s          0 s      55402 s   33409386 s          0 s
#3  3501 MHz     403140 s          0 s      58990 s   33740496 s          0 s
#4  3501 MHz     321931 s          0 s      51549 s   33829634 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+3995
Commit 9ae220a (2016-05-09 15:27 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22107.15625 MB free)
Uptime: 346846.0 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     467448 s          0 s      95093 s   34036422 s          1 s
#2  3501 MHz     945505 s          0 s      63173 s   33649977 s          0 s
#3  3501 MHz     476994 s          0 s      66757 s   34120897 s          0 s
#4  3501 MHz     378375 s          0 s      57140 s   34229694 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
