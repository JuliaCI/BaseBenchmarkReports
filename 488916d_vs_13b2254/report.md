# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@488916d26fd2e71a05bbc3065c929d979d0f4bdd](https://github.com/JuliaLang/julia/commit/488916d26fd2e71a05bbc3065c929d979d0f4bdd) vs [JuliaLang/julia@13b22540b7b85cc29e62f15bbad7c2b29a82afeb](https://github.com/JuliaLang/julia/commit/13b22540b7b85cc29e62f15bbad7c2b29a82afeb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19730#issuecomment-270123557)

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
| `["array","bool","boolarray_true_load!"]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 1.09 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.06 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.08 (15%)  | 1.06 (1%) :x: |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.00 (50%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.00 (50%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.00 (50%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","linspace(1.0,2.0,10000)")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon","BitArray{2}")]` | 1.02 (50%)  | 1.08 (1%) :x: |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 0.30 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.00 (50%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","linspace(1.0,2.0,10000)")]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 0.30 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","linspace(1.0,2.0,10000)")]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 1.16 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000:-1:1")]` | 1.26 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000")]` | 1.28 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.14 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.18 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.20 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.30 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.21 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.37 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.20 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.25 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.13 (50%)  | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.18 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.23 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000)")]` | 0.99 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 1.04 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 1.04 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.13 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.14 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.15 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.14 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.16 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.13 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 1.15 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.02 (50%)  | 0.54 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.03 (50%)  | 0.54 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 1.25 (15%) :x: | 1.40 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.19 (15%) :x: | 1.22 (1%) :x: |
| `["problem","go","go_game"]` | 1.04 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spvec","integer",10000)]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.30 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1864
Commit 488916d (2017-01-03 13:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4727.3984375 MB free)
Uptime: 1.9106189e7 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33505742 s          0 s    5327271 s  1867907918 s         56 s
#2  3501 MHz  101855802 s          0 s    6336008 s  1799252998 s         20 s
#3  3501 MHz   28815202 s          0 s    3604882 s  1877312838 s         32 s
#4  3501 MHz   24397024 s          0 s    3488050 s  1882013923 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1854
Commit 13b2254 (2017-01-03 12:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4280.2890625 MB free)
Uptime: 1.9113689e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33554412 s          0 s    5334936 s  1868599181 s         57 s
#2  3501 MHz  102317601 s          0 s    6344204 s  1799532139 s         20 s
#3  3501 MHz   28869064 s          0 s    3611298 s  1878001675 s         32 s
#4  3501 MHz   24549888 s          0 s    3499888 s  1882598768 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
