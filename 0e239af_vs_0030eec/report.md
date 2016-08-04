# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0e239af4039e30be3847aa374ecbe66107a852e2](https://github.com/JuliaLang/julia/commit/0e239af4039e30be3847aa374ecbe66107a852e2) vs [JuliaLang/julia@0030eec2f332f353e6890ca289ac2aca55532dde](https://github.com/JuliaLang/julia/commit/0030eec2f332f353e6890ca289ac2aca55532dde)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17804#issuecomment-237457204)

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
| `["array","cat",("catnd",5)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 0.44 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.39 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.41 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 0.51 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 0.44 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Int32,2}")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.51 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.45 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.56 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.48 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort reverse","descending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",100)]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 1.93 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc0+196
Commit 0e239af (2016-08-04 05:30 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (30971.76171875 MB free)
Uptime: 5.93929e6 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    7600272 s          0 s    1803698 s  582825569 s         19 s
#2  3501 MHz   21477759 s          0 s    1105477 s  570912693 s          2 s
#3  3501 MHz    7823126 s          0 s    1002359 s  584818726 s         10 s
#4  3501 MHz    6407876 s          0 s     977973 s  586250946 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-rc0+0
Commit 0030eec (2016-07-26 20:22 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28024.359375 MB free)
Uptime: 5.943955e6 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    7646735 s          0 s    1810678 s  583237184 s         19 s
#2  3501 MHz   21672224 s          0 s    1112206 s  571177470 s          2 s
#3  3501 MHz    7962511 s          0 s    1012181 s  585135003 s         10 s
#4  3501 MHz    6464256 s          0 s     984044 s  586654317 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
