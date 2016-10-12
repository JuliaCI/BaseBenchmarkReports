# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@82d6438393ac90f552c3244c440132f206505993](https://github.com/mbauman/julia/commit/82d6438393ac90f552c3244c440132f206505993) vs [JuliaLang/julia@11d3c9684dfcb8338afd879fd25cd34c8585b38e](https://github.com/JuliaLang/julia/commit/11d3c9684dfcb8338afd879fd25cd34c8585b38e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15558#issuecomment-253127268)

*Tag Predicate:* `"array"`

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
| `["array","cat",("vcat",5)]` | 1.06 (15%)  | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 1.28 (50%)  | 1.56 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 1.29 (50%)  | 1.49 (1%) :x: |

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
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["problem","laplacian"]`
- `["simd"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.949
Commit 82d6438 (2016-10-12 05:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15899.8984375 MB free)
Uptime: 1.1902065e7 sec
Load Avg:  1.0498046875  1.015625  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18874622 s          0 s    4050991 s  1163890104 s         36 s
#2  3501 MHz   52081973 s          0 s    2553090 s  1134810959 s          5 s
#3  3501 MHz   17769267 s          0 s    2217550 s  1169652633 s         24 s
#4  3501 MHz   15387912 s          0 s    2235957 s  1171994490 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.947
Commit 11d3c96 (2016-10-12 03:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15919.08203125 MB free)
Uptime: 1.1906277e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18930995 s          0 s    4058810 s  1164245956 s         36 s
#2  3501 MHz   52222014 s          0 s    2559600 s  1135085010 s          5 s
#3  3501 MHz   17894672 s          0 s    2227344 s  1169937971 s         24 s
#4  3501 MHz   15455941 s          0 s    2243526 s  1172339575 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
