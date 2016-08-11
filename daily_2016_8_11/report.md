# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@eb515f39848eaaafd3fdeea154f830ecce592409](https://github.com/JuliaLang/julia/commit/eb515f39848eaaafd3fdeea154f830ecce592409)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/eb515f39848eaaafd3fdeea154f830ecce592409#commitcomment-18600509)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-11 vs 2016-08-10

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
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 1.86 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 2.15 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 1.86 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 1.80 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.88 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.88 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.03 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.34 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.74 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 2.17 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.94 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.05 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 1.86 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 2.15 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 1.81 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Int32,2}")]` | 1.89 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.69 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 2.08 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.04 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.37 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.94 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.89 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.90 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.38 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 1.61 (40%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 2.18 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 2.02 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.97 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.96 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["shootout","fannkuch"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",100)]` | 1.53 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 1.71 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.154
Commit eb515f3 (2016-08-11 01:14 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19768.2890625 MB free)
Uptime: 6.53792e6 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9163412 s          0 s    2088914 s  640652090 s         22 s
#2  3501 MHz   22798684 s          0 s    1177218 s  629360667 s          3 s
#3  3501 MHz    8461661 s          0 s    1069698 s  643959290 s         11 s
#4  3501 MHz    6877724 s          0 s    1046620 s  645554486 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
