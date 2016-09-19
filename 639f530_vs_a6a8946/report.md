# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@639f530ded87c47448db695661c2d7b106a06de2](https://github.com/JuliaLang/julia/commit/639f530ded87c47448db695661c2d7b106a06de2) vs [JuliaLang/julia@a6a8946a8f668798dbe641ac48860f9e192e58db](https://github.com/JuliaLang/julia/commit/a6a8946a8f668798dbe641ac48860f9e192e58db)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18304#issuecomment-248124570)

*Tag Predicate:* `"nullable"`

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
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(0)")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(1)")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(false)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(true)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(false)")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
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
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}()")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(0)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(1)")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Complex{Float64}")]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Float32")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Float64")]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int64")]` | 0.54 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int8")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 0.11 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Complex{Float64}")]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 0.13 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 0.11 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 0.08 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 0.11 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Float64")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","BigInt")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int8")]` | 1.26 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["nullable","basic"]`
- `["nullable","nullablearray"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.703
Commit 639f530 (2016-09-19 20:56 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18877.7265625 MB free)
Uptime: 9.967447e6 sec
Load Avg:  0.9970703125  0.9453125  0.8896484375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15651881 s          0 s    2703008 s  976277548 s         31 s
#2  3501 MHz   38389436 s          0 s    2822310 s  954169642 s          8 s
#3  3501 MHz   13521393 s          0 s    1745932 s  980993020 s         14 s
#4  3501 MHz   11179290 s          0 s    1698910 s  983465507 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.698
Commit a6a8946a (2016-09-19 19:25 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18993.2578125 MB free)
Uptime: 9.970717e6 sec
Load Avg:  0.99365234375  0.91357421875  0.900390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15772880 s          0 s    2712482 s  976473306 s         31 s
#2  3501 MHz   38468624 s          0 s    2829967 s  954409115 s          8 s
#3  3501 MHz   13566590 s          0 s    1752581 s  981267447 s         15 s
#4  3501 MHz   11230378 s          0 s    1705417 s  983734259 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
