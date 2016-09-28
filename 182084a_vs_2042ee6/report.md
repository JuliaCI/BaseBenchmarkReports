# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@182084a6c72a93085feea143d2a76d7479dd5d12](https://github.com/pabloferz/julia/commit/182084a6c72a93085feea143d2a76d7479dd5d12) vs [JuliaLang/julia@2042ee6458bd93f50e0e569ae109c53d06638f13](https://github.com/JuliaLang/julia/commit/2042ee6458bd93f50e0e569ae109c53d06638f13)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18642#issuecomment-250062824)

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
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 1.32 (30%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.84 (30%) :x: | 1.04 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.52 (30%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 2.09 (30%) :x: | 1.04 (1%) :x: |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(1)")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","BigInt")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Float64")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",100)]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.54 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.815
Commit 182084a (2016-09-28 01:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15341.2265625 MB free)
Uptime: 1.0683896e7 sec
Load Avg:  1.0029296875  1.0078125  0.9580078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17703753 s          0 s    3688038 s  1043963960 s         34 s
#2  3501 MHz   47108730 s          0 s    2334024 s  1018250526 s          4 s
#3  3501 MHz   16447389 s          0 s    2037128 s  1049388684 s         22 s
#4  3501 MHz   14062439 s          0 s    2043541 s  1051748397 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.811
Commit 2042ee6 (2016-09-27 23:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14846.40625 MB free)
Uptime: 1.0688873e7 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17763047 s          0 s    3695880 s  1044392921 s         34 s
#2  3501 MHz   47327786 s          0 s    2344585 s  1018518158 s          4 s
#3  3501 MHz   16485463 s          0 s    2043488 s  1049841128 s         22 s
#4  3501 MHz   14208789 s          0 s    2054207 s  1052088539 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
