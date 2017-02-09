# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@12f2f10a72d32f69bf275b1eb2850812428ec921](https://github.com/JuliaLang/julia/commit/12f2f10a72d32f69bf275b1eb2850812428ec921) vs [JuliaLang/julia@e24faa565ec581d055195c34a73266aabd2f4975](https://github.com/JuliaLang/julia/commit/e24faa565ec581d055195c34a73266aabd2f4975)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20485#issuecomment-278512563)

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
| `["array","convert",("Int","Complex{Float64}")]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",2048)]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.90 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.25 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.70 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.03 (15%)  | 1.03 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.03 (15%)  | 1.03 (1%) :x: |
| `["shootout","k_nucleotide"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ones")]` | 1.95 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ones")]` | 1.78 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.96 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 2.05 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.77 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.92 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","random")]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","random")]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.92 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","random")]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","random")]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 2.03 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 2.06 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ones")]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","random")]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ones")]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","random")]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 2.13 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 2.13 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 2.13 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 2.10 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","random")]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 1.30 (30%) :x: | 1.02 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 2.41 (30%) :x: | 1.01 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 2.72 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 1.58 (30%) :x: | 1.04 (1%) :x: |
| `["sparse","index",("spmat","logical",100)]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",10)]` | 0.93 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 0.98 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.12 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.50 (30%) :x: | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 2.20 (30%) :x: | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",1000)]` | 2.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",10)]` | 0.94 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 1.00 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.00 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spvec","array",1000)]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",10000)]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",100000)]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",1000)]` | 3.15 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",10000)]` | 2.07 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",100000)]` | 2.04 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",100000)]` | 1.44 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2676
Commit 12f2f10 (2017-02-09 00:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5562.6484375 MB free)
Uptime: 2.2255427e7 sec
Load Avg:  1.0830078125  1.03125  1.046875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   35688857 s          0 s    7766170 s  2175648735 s         64 s
#2  3501 MHz  117338966 s          0 s    4546078 s  2102378726 s          8 s
#3  3501 MHz   31628378 s          0 s    3953736 s  2188938276 s         46 s
#4  3501 MHz   29494062 s          0 s    4095853 s  2190920747 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2673
Commit e24faa5 (2017-02-08 21:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5182.875 MB free)
Uptime: 2.2263307e7 sec
Load Avg:  1.0029296875  1.01806640625  0.98681640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   35733070 s          0 s    7775298 s  2176380730 s         64 s
#2  3501 MHz  117820422 s          0 s    4552535 s  2102678188 s          8 s
#3  3501 MHz   31799797 s          0 s    3964477 s  2189543315 s         46 s
#4  3501 MHz   29553667 s          0 s    4102307 s  2191641998 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
