# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fa5af2377381145c8949c2de7c2bfceaf772d83e](https://github.com/JuliaLang/julia/commit/fa5af2377381145c8949c2de7c2bfceaf772d83e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/fa5af2377381145c8949c2de7c2bfceaf772d83e#commitcomment-18142819)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-07-06 vs 2016-07-02

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
| `["array","growth",("prerend!",2048)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 3.82 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 5.27 (30%) :x: | 1.20 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 3.67 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 5.02 (30%) :x: | 1.20 (1%) :x: |
| `["scalar","iteration","in"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.00 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.00 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 0.99 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 0.99 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 1.00 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.00 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(600,400))]` | 1.03 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(600,600))]` | 1.01 (15%)  | Inf (1%) :x: |

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
Julia Version 0.5.0-dev+5179
Commit fa5af23 (2016-07-06 00:27 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22028.65625 MB free)
Uptime: 3.465251e6 sec
Load Avg:  1.0029296875  1.0146484375  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3484678 s          0 s     795568 s  341467894 s         11 s
#2  3501 MHz    9576999 s          0 s     685210 s  335951910 s          4 s
#3  3501 MHz    3642131 s          0 s     541398 s  342140695 s          3 s
#4  3501 MHz    2508008 s          0 s     509716 s  343337012 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
