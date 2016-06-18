# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@76083b434aff8198a20fde2afd45aacebf9835d7](https://github.com/JuliaLang/julia/commit/76083b434aff8198a20fde2afd45aacebf9835d7) vs [JuliaLang/julia@2ac304dfba75fad148d4070ef4f8a2e400c305bb](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/76083b434aff8198a20fde2afd45aacebf9835d7#commitcomment-17923253)

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
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["linalg","blas","dotc"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dotu"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",1024)]` | 2.52 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 2.65 (25%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ones")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.29 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.4.6-pre+60
Commit 76083b4 (2016-06-17 07:56 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27136.71484375 MB free)
Uptime: 1.903141e6 sec
Load Avg:  0.9228515625  0.9853515625  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2374804 s          0 s     557088 s  186889054 s          5 s
#2  3501 MHz    7854501 s          0 s     408068 s  181931521 s          1 s
#3  3501 MHz    3199712 s          0 s     400000 s  186600982 s          1 s
#4  3501 MHz    2627270 s          0 s     369548 s  187213313 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

#### Comparison Build

```
Julia Version 0.4.5
Commit 2ac304d (2016-03-18 00:58 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (26988.02734375 MB free)
Uptime: 1.906802e6 sec
Load Avg:  1.0029296875  0.99365234375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2444750 s          0 s     563959 s  187177013 s          5 s
#2  3501 MHz    8092038 s          0 s     414669 s  182052796 s          1 s
#3  3501 MHz    3255622 s          0 s     406360 s  186903891 s          1 s
#4  3501 MHz    2676688 s          0 s     375765 s  187523091 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
