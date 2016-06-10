# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f0b618765f0913c8bf90dbd58a2d005019798782](https://github.com/JuliaLang/julia/commit/f0b618765f0913c8bf90dbd58a2d005019798782) vs [JuliaLang/julia@56d7d6672c7db717dacb5e34f485180c2eba83b2](https://github.com/JuliaLang/julia/commit/56d7d6672c7db717dacb5e34f485180c2eba83b2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16260#issuecomment-225212802)

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
| `["array","bool","bitarray_true_load!"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 1.07 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.13 (15%)  | 1.13 (1%) :x: |
| `["array","cat",("vcat",5)]` | 0.98 (15%)  | 1.12 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.18 (15%) :x: | 1.13 (1%) :x: |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.16 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.60 (40%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumeach","1:100000000")]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.34 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.34 (40%)  | 1.04 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.16 (40%)  | 1.05 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.62 (40%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.66 (40%) :x: | 1.33 (1%) :x: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.65 (40%) :x: | 1.33 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.07 (15%)  | 1.22 (1%) :x: |
| `["shootout","revcomp"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.03 (25%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.04 (15%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","integer",1000)]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",10)]` | 1.13 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.04 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.16 (15%) :x: | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.03 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 1.06 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 1.01 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.00 (25%)  | 1.05 (1%) :x: |

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
Julia Version 0.5.0-dev+4678
Commit f0b6187 (2016-06-10 14:57 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28051.390625 MB free)
Uptime: 1.222027e6 sec
Load Avg:  1.0029296875  1.001953125  0.95703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     422407 s          0 s     237986 s  121235848 s          4 s
#2  3501 MHz    1760533 s          0 s     138735 s  120231456 s          0 s
#3  3501 MHz     777333 s          0 s     147832 s  121210882 s          0 s
#4  3501 MHz     689456 s          0 s     131129 s  121322394 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4646
Commit 56d7d66 (2016-06-10 11:00 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27892.34375 MB free)
Uptime: 1.226633e6 sec
Load Avg:  1.11279296875  1.03125  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     457706 s          0 s     243861 s  121653854 s          4 s
#2  3501 MHz    1969091 s          0 s     145030 s  120476752 s          0 s
#3  3501 MHz     922402 s          0 s     158664 s  121514961 s          0 s
#4  3501 MHz     732064 s          0 s     137046 s  121733911 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
