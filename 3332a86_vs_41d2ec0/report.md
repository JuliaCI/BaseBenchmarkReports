# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3332a86acce2a5261e63bfb8cf5730b6ac317d20](https://github.com/JuliaLang/julia/commit/3332a86acce2a5261e63bfb8cf5730b6ac317d20) vs [JuliaLang/julia@41d2ec05d05e201a42fa1e015846f637aa5a8953](https://github.com/JuliaLang/julia/commit/41d2ec05d05e201a42fa1e015846f637aa5a8953)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16260#issuecomment-225497921)

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
| `["array","cat",("catnd_setind",5)]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.15 (15%) :x: | 1.13 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.04 (15%)  | 1.12 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.18 (15%) :x: | 1.13 (1%) :x: |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.75 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.98 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.57 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.56 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.51 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.50 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.66 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.65 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.56 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.63 (30%) :white_check_mark: | 0.99 (1%)  |
| `["problem","go","go_game"]` | 1.08 (15%)  | 1.22 (1%) :x: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.07 (25%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.08 (15%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",10)]` | 1.10 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.00 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.98 (15%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.07 (15%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.03 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 1.07 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 1.05 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.00 (25%)  | 1.05 (1%) :x: |
| `["string","replace"]` | 1.64 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4738
Commit 3332a86 (2016-06-13 06:20 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27628.6640625 MB free)
Uptime: 1.44884e6 sec
Load Avg:  1.0029296875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1004140 s          0 s     339036 s  143174095 s          4 s
#2  3501 MHz    3428386 s          0 s     220236 s  141148017 s          0 s
#3  3501 MHz    1674543 s          0 s     234957 s  142893127 s          0 s
#4  3501 MHz    1438450 s          0 s     211306 s  143160729 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4694
Commit 41d2ec0 (2016-06-12 22:18 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27500.1796875 MB free)
Uptime: 1.453461e6 sec
Load Avg:  1.0029296875  0.99560546875  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1053687 s          0 s     345528 s  143578623 s          4 s
#2  3501 MHz    3626442 s          0 s     227403 s  141404367 s          0 s
#3  3501 MHz    1798642 s          0 s     244053 s  143221342 s          0 s
#4  3501 MHz    1499656 s          0 s     217659 s  143554711 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
