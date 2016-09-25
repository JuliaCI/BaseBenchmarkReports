# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@415de414bd2082514aba74307d5c30800c0f1927](https://github.com/JuliaLang/julia/commit/415de414bd2082514aba74307d5c30800c0f1927) vs [JuliaLang/julia@11b06ed60481fd1d583cae8369634943be545f72](https://github.com/JuliaLang/julia/commit/11b06ed60481fd1d583cae8369634943be545f72)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/14763#issuecomment-249389007)

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
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(1)")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","descending")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.15 (15%) :x: | 1.00 (1%)  |

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
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
Julia Version 0.6.0-dev.766
Commit 415de41 (2016-09-24 20:17 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16440.98046875 MB free)
Uptime: 1.0403149e7 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16754733 s          0 s    2855659 s  1018502058 s         32 s
#2  3501 MHz   41152814 s          0 s    2998148 s  994730808 s          9 s
#3  3501 MHz   14362757 s          0 s    1858184 s  1023583288 s         16 s
#4  3501 MHz   12101409 s          0 s    1813214 s  1025982920 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.763
Commit 11b06ed (2016-09-24 18:25 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16747.734375 MB free)
Uptime: 1.0407883e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16793441 s          0 s    2862775 s  1018928157 s         32 s
#2  3501 MHz   41346964 s          0 s    3005332 s  995002141 s          9 s
#3  3501 MHz   14410710 s          0 s    1864722 s  1024001293 s         16 s
#4  3501 MHz   12262347 s          0 s    1824428 s  1026283595 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
