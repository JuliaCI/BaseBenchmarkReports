# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f184104ba391f49e404bba37afcd6b0bfa854950](https://github.com/JuliaLang/julia/commit/f184104ba391f49e404bba37afcd6b0bfa854950) vs [JuliaLang/julia@309657f69c1a54fedfda5764b5b106286389383c](https://github.com/JuliaLang/julia/commit/309657f69c1a54fedfda5764b5b106286389383c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19730#issuecomment-269565065)

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
| `["array","cat",("catnd",5)]` | 1.98 (15%) :x: | 1.45 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.08 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.02 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.05 (15%)  | 1.06 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","100000000:-1:1")]` | 22.76 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000000)")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 15.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 4.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 1.38 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000000:-1:1")]` | 3.08 (50%) :x: | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000000")]` | 1.52 (50%) :x: | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.29 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.32 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.38 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.34 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.35 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.35 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.36 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.35 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.14 (50%)  | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.39 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.37 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 1.21 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 2.96 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 16.14 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 3.19 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 0.92 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 0.94 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.95 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.95 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.97 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.96 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.93 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.94 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.92 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.92 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.97 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 0.94 (50%)  | 0.84 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000000:-1:1")]` | 1.26 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000000")]` | 1.07 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 0.70 (50%)  | 0.84 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 3.36 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.25 (15%) :x: | 1.40 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.16 (15%) :x: | 1.22 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.44 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.04 (15%)  | 1.11 (1%) :x: |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","sparse"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
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
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1741
Commit f184104 (2016-12-29 00:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6048.36328125 MB free)
Uptime: 1.8626732e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25228078 s          0 s    5984258 s  1826133635 s         59 s
#2  3501 MHz   79861316 s          0 s    3636753 s  1778065716 s          8 s
#3  3501 MHz   24372274 s          0 s    3141402 s  1834303617 s         38 s
#4  3501 MHz   21804248 s          0 s    3225641 s  1836766569 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1738
Commit 309657f (2016-12-28 18:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5841.66796875 MB free)
Uptime: 1.8633036e7 sec
Load Avg:  1.00732421875  1.01708984375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25273891 s          0 s    5991536 s  1826708787 s         59 s
#2  3501 MHz   80218851 s          0 s    3643959 s  1778330789 s          8 s
#3  3501 MHz   24414692 s          0 s    3147359 s  1834884746 s         38 s
#4  3501 MHz   21958305 s          0 s    3236860 s  1837231168 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
