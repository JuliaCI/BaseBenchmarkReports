# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3d980ca2db5a984cc093f0d628d96c8cec3bdf08](https://github.com/JuliaLang/julia/commit/3d980ca2db5a984cc093f0d628d96c8cec3bdf08) vs [JuliaLang/julia@0030eec2f332f353e6890ca289ac2aca55532dde](https://github.com/JuliaLang/julia/commit/0030eec2f332f353e6890ca289ac2aca55532dde)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3d980ca2db5a984cc093f0d628d96c8cec3bdf08#commitcomment-18609900)

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
| `["array","index",("sumcolon","100000000:-1:1")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Int32,2}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.45 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 2.00 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.99 (15%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.46 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.47 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",100)]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc1+13
Commit 3d980ca (2016-08-11 04:22 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19062.15234375 MB free)
Uptime: 6.585908e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9890624 s          0 s    2156436 s  644643332 s         22 s
#2  3501 MHz   24413410 s          0 s    1234144 s  632483556 s          3 s
#3  3501 MHz    8794030 s          0 s    1113977 s  648374937 s         12 s
#4  3501 MHz    7266182 s          0 s    1095562 s  649911599 s          2 s

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
Memory: 31.383651733398438 GB (18865.37109375 MB free)
Uptime: 6.59058e6 sec
Load Avg:  1.0029296875  1.0146484375  0.97021484375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9933126 s          0 s    2162294 s  645060628 s         22 s
#2  3501 MHz   24610782 s          0 s    1241588 s  632745279 s          3 s
#3  3501 MHz    8913210 s          0 s    1123110 s  648713057 s         12 s
#4  3501 MHz    7344721 s          0 s    1103256 s  650291991 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
