# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@583fa20b6778e74c3fcd2df13baa3830eca4ed8b](https://github.com/JuliaLang/julia/commit/583fa20b6778e74c3fcd2df13baa3830eca4ed8b) vs [JuliaLang/julia@e70de2100f466161d4140a07c62321cb49f624a0](https://github.com/JuliaLang/julia/commit/e70de2100f466161d4140a07c62321cb49f624a0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/583fa20b6778e74c3fcd2df13baa3830eca4ed8b#commitcomment-18453413)

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
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ascending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","descending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,10000))]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.19 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc0+56
Commit 583fa20 (2016-07-29 17:54 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13056.6328125 MB free)
Uptime: 5.467755e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6784880 s          0 s    1367007 s  537414398 s         18 s
#2  3501 MHz   16953775 s          0 s    1169963 s  528120026 s          4 s
#3  3501 MHz    5828291 s          0 s     855938 s  539788513 s          9 s
#4  3501 MHz    4317375 s          0 s     822468 s  541381564 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-rc0+54
Commit e70de21 (2016-07-29 14:57 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12894.26171875 MB free)
Uptime: 5.472405e6 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6845308 s          0 s    1373004 s  537811444 s         18 s
#2  3501 MHz   17139349 s          0 s    1176730 s  528392070 s          4 s
#3  3501 MHz    5881134 s          0 s     862576 s  540193221 s          9 s
#4  3501 MHz    4453150 s          0 s     833172 s  541699620 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
