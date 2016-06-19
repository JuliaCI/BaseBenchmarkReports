# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@37a70a58f693a87e6d232702c11eb4920d9ab4fb](https://github.com/JuliaLang/julia/commit/37a70a58f693a87e6d232702c11eb4920d9ab4fb) vs [JuliaLang/julia@2ac304dfba75fad148d4070ef4f8a2e400c305bb](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16980#issuecomment-226986755)

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
| `["io","read"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","axpy!"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","dot"]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","dotc"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","dotu"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","sbmv!"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","symv!"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","symv"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","trsv!"]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Complex{UInt64}")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ones")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","ones")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.4.6-pre+87
Commit 37a70a5 (2016-06-19 08:53 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27111.8671875 MB free)
Uptime: 1.975727e6 sec
Load Avg:  1.0029296875  1.00537109375  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2067390 s          0 s     468797 s  194582203 s          6 s
#2  3501 MHz    5970024 s          0 s     401152 s  191029484 s          1 s
#3  3501 MHz    2360398 s          0 s     341901 s  194745464 s          2 s
#4  3501 MHz    1582724 s          0 s     302333 s  195595473 s          1 s

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
Memory: 31.383651733398438 GB (26978.421875 MB free)
Uptime: 1.979011e6 sec
Load Avg:  1.0029296875  1.001953125  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2115791 s          0 s     475033 s  194854729 s          6 s
#2  3501 MHz    6150749 s          0 s     407378 s  191170300 s          1 s
#3  3501 MHz    2408597 s          0 s     347994 s  195018806 s          2 s
#4  3501 MHz    1679090 s          0 s     310136 s  195819093 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
