# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b36141f4799d73113b3597ee94d5925929b2ccd5](https://github.com/JuliaLang/julia/commit/b36141f4799d73113b3597ee94d5925929b2ccd5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b36141f4799d73113b3597ee94d5925929b2ccd5#commitcomment-19235956)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-09-30 vs 2016-09-29

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
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","Array")]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","NullableArray")]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","BigInt")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Complex{Float64}")]` | 2.72 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float64")]` | 2.74 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int64")]` | 2.72 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Bool")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Complex{Float64}")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float32")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int64")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int8")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.826
Commit b36141f (2016-09-29 16:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14738.07421875 MB free)
Uptime: 1.0857877e7 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18083617 s          0 s    3754457 s  1060866338 s         34 s
#2  3501 MHz   47976857 s          0 s    2377477 s  1034726947 s          4 s
#3  3501 MHz   16621194 s          0 s    2066639 s  1066576049 s         22 s
#4  3501 MHz   14411544 s          0 s    2085084 s  1068746032 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
