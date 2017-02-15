# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e2cceb619d100d57ccdd06aa1fdc6b4ec6d650a5](https://github.com/JuliaLang/julia/commit/e2cceb619d100d57ccdd06aa1fdc6b4ec6d650a5) vs [JuliaLang/julia@78448fa8cbba354ea7786bfb5ff19f8e17630430](https://github.com/JuliaLang/julia/commit/78448fa8cbba354ea7786bfb5ff19f8e17630430)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/e2cceb619d100d57ccdd06aa1fdc6b4ec6d650a5#commitcomment-20893760)

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
| `["array","growth",("append!",8)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.98 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.98 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.79 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.83 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.96 (15%)  | 0.98 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.94 (15%)  | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",1024)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.02 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",256)]` | 0.02 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 0.99 (45%)  | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 0.99 (45%)  | 0.53 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 0.99 (45%)  | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 0.99 (45%)  | 0.53 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigFloat}")]` | 4.81 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2661
Commit e2cceb6 (2017-02-08 04:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13179.17578125 MB free)
Uptime: 2.2815525e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   46572978 s          0 s    7237823 s  2222927376 s         68 s
#2  3501 MHz  151278977 s          0 s    7680109 s  2118901630 s         22 s
#3  3501 MHz   38000881 s          0 s    4529137 s  2237976136 s         38 s
#4  3501 MHz   33885012 s          0 s    4463724 s  2242371069 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2430
Commit 78448fa (2017-01-28 02:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13009.86328125 MB free)
Uptime: 2.2821042e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   46656897 s          0 s    7247368 s  2223383546 s         68 s
#2  3501 MHz  151784845 s          0 s    7688803 s  2118938119 s         22 s
#3  3501 MHz   38085523 s          0 s    4537400 s  2238434090 s         38 s
#4  3501 MHz   33967162 s          0 s    4471717 s  2242832045 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
