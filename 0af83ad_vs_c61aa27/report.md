# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@0af83ad2d609b2288a03b112d451d0d7483bf6a7](https://github.com/pkofod/julia/commit/0af83ad2d609b2288a03b112d451d0d7483bf6a7) vs [JuliaLang/julia@c61aa276a3e89f4cb0ccbe797ed48f49c4e5ae20](https://github.com/JuliaLang/julia/commit/c61aa276a3e89f4cb0ccbe797ed48f49c4e5ae20)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23383#issuecomment-335383077)

*Tag Predicate:* `"scalar"`

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
| `["scalar","asin",("small","negative argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan",("11/16 <= abs(x) < 19/16","negative argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("11/16 <= abs(x) < 19/16","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("19/16 <= abs(x) < 39/16","negative argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("19/16 <= abs(x) < 39/16","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("39/16 <= abs(x) < 2^66","negative argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("39/16 <= abs(x) < 2^66","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("7/16 <= abs(x) < 11/16","negative argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("7/16 <= abs(x) < 11/16","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("very large","positive argument","Float32")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y negative","x positive","Float64")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y positive","x negative","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y positive","x positive","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (small)","y negative","x positive","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (small)","y positive","x positive","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float64")]` | 1.62 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["scalar","tan",("small","negative argument","Float64")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","tan",("small","positive argument","Float64")]` | 1.15 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","atan2"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","sincos"]`
- `["scalar","tan"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2104
Commit 0af83ad (2017-10-10 05:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   98094969 s          0 s   17340921 s  4199046726 s         93 s
       #2  3501 MHz  424874063 s          0 s   11235882 s  3888561536 s         20 s
       #3  3501 MHz   84812640 s          0 s    9602629 s  4230682910 s         78 s
       #4  3501 MHz   81005061 s          0 s    9800764 s  4234291557 s         19 s
       
  Memory: 31.383651733398438 GB (2609.91015625 MB free)
  Uptime: 4.3271723e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.2158203125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2097
Commit c61aa27 (2017-10-10 05:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   98194052 s          0 s   17349030 s  4199248601 s         93 s
       #2  3501 MHz  425123255 s          0 s   11243575 s  3888614261 s         20 s
       #3  3501 MHz   84889904 s          0 s    9610008 s  4230907641 s         78 s
       #4  3501 MHz   81086227 s          0 s    9808201 s  4234512687 s         19 s
       
  Memory: 31.383651733398438 GB (2453.0 MB free)
  Uptime: 4.3274825e7 sec
  Load Avg:  0.9228515625  0.99951171875  1.189453125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
