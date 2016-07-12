# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@019ba505a7d32c4709ab227a3f1dbc46fa65af21](https://github.com/JuliaLang/julia/commit/019ba505a7d32c4709ab227a3f1dbc46fa65af21) vs [JuliaLang/julia@f881efb5e8ee4b3c04d90895a92c03c075805147](https://github.com/JuliaLang/julia/commit/f881efb5e8ee4b3c04d90895a92c03c075805147)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17355#issuecomment-232087923)

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
| `["array","cat",("hcat",5)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 8.74 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 9.95 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 8.74 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 10.10 (40%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{UInt64}")]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5357
Commit 019ba50 (2016-07-12 14:51 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13382.828125 MB free)
Uptime: 3.987727e6 sec
Load Avg:  1.0029296875  1.0146484375  0.99462890625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5008070 s          0 s    1023445 s  391837241 s         14 s
#2  3501 MHz   11537756 s          0 s     799569 s  386075856 s          4 s
#3  3501 MHz    4342810 s          0 s     628191 s  393575059 s          4 s
#4  3501 MHz    2992194 s          0 s     586742 s  395006719 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5351
Commit f881efb (2016-07-12 14:50 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13242.4296875 MB free)
Uptime: 3.992255e6 sec
Load Avg:  1.0029296875  1.00634765625  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    5087762 s          0 s    1030897 s  392201628 s         14 s
#2  3501 MHz   11739517 s          0 s     806184 s  386319729 s          4 s
#3  3501 MHz    4390016 s          0 s     634073 s  393974029 s          4 s
#4  3501 MHz    3087422 s          0 s     595847 s  395354806 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
