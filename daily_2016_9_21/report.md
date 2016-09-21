# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c485fc068468c4de8809715d2ba9a01c80e5398f](https://github.com/JuliaLang/julia/commit/c485fc068468c4de8809715d2ba9a01c80e5398f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/c485fc068468c4de8809715d2ba9a01c80e5398f#commitcomment-19107803)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-09-21 vs 2016-09-20

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(0)")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(1)")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(false)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(true)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(false)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(true)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(0.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(1.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(0.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(1.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(0.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(1.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(0.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(1.0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Complex{Float64}")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Float32")]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Float64")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int64")]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int8")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 0.12 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Complex{Float64}")]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 0.13 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 0.11 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 0.08 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 0.11 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Complex{Float64}")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.93 (15%)  | 0.94 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.93 (15%)  | 0.97 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.93 (15%)  | 0.93 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["sort","issorted",("forwards","ascending")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.70 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.729
Commit c485fc0 (2016-09-21 03:48 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18327.359375 MB free)
Uptime: 1.0080287e7 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15940609 s          0 s    2745971 s  987205617 s         31 s
#2  3501 MHz   39162372 s          0 s    2872119 s  964611785 s          8 s
#3  3501 MHz   13792754 s          0 s    1779637 s  991965573 s         16 s
#4  3501 MHz   11459199 s          0 s    1731982 s  994432637 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
