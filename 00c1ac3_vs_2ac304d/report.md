# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@00c1ac387d1eea9c20163537df2ef414c9aef391](https://github.com/JuliaLang/julia/commit/00c1ac387d1eea9c20163537df2ef414c9aef391) vs [JuliaLang/julia@2ac304dfba75fad148d4070ef4f8a2e400c305bb](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/00c1ac387d1eea9c20163537df2ef414c9aef391#commitcomment-17910757)

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
| `["array","index",("sumcartesian","1:100000000")]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["linalg","blas","axpy!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dot"]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Diagonal",256)]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","ones")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ones")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","ones")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 1.46 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.4.6-pre+44
Commit 00c1ac3 (2016-06-17 01:59 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27348.59375 MB free)
Uptime: 1.810527e6 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1902631 s          0 s     483108 s  178204244 s          5 s
#2  3501 MHz    5816369 s          0 s     332868 s  174792703 s          1 s
#3  3501 MHz    2498192 s          0 s     331508 s  178119478 s          1 s
#4  3501 MHz    2106045 s          0 s     305394 s  178546768 s          0 s

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
Memory: 31.383651733398438 GB (27215.38671875 MB free)
Uptime: 1.813975e6 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1961975 s          0 s     489326 s  178482112 s          5 s
#2  3501 MHz    6038026 s          0 s     340862 s  174907158 s          1 s
#3  3501 MHz    2558465 s          0 s     337922 s  178396653 s          1 s
#4  3501 MHz    2153868 s          0 s     311050 s  178837387 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
