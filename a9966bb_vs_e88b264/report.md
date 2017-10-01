# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@a9966bbfd79e036507f11defecce5909e3d53ea3](https://github.com/pkofod/julia/commit/a9966bbfd79e036507f11defecce5909e3d53ea3) vs [JuliaLang/julia@e88b26408c025c50aabdc91a0859400b016bf4ff](https://github.com/JuliaLang/julia/commit/e88b26408c025c50aabdc91a0859400b016bf4ff)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23468#issuecomment-333392962)

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
| `["scalar","acos",("one","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y negative","x negative","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y negative","x positive","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y positive","x negative","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y positive","x positive","Float32")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (small)","y negative","x negative","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (small)","y negative","x positive","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (small)","y positive","x negative","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("y zero","y negative","x negative","Float32")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("y zero","y positive","x negative","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
- `["scalar","tan"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2028
Commit a9966bb (2017-10-01 16:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87566703 s          0 s   13624008 s  4142154352 s        173 s
       #2  3501 MHz  352361546 s          0 s   14596185 s  3878429029 s         60 s
       #3  3501 MHz   73187064 s          0 s    8370408 s  4169475381 s         81 s
       #4  3501 MHz   68530805 s          0 s    8245131 s  4174658654 s         30 s
       
  Memory: 31.383651733398438 GB (4929.95703125 MB free)
  Uptime: 4.2528539e7 sec
  Load Avg:  0.9970703125  1.0146484375  1.1689453125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2024
Commit e88b264 (2017-10-01 16:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87663712 s          0 s   13632472 s  4142374868 s        174 s
       #2  3501 MHz  352628340 s          0 s   14603810 s  3878481304 s         60 s
       #3  3501 MHz   73270065 s          0 s    8378409 s  4169710974 s         82 s
       #4  3501 MHz   68614710 s          0 s    8253033 s  4174893605 s         30 s
       
  Memory: 31.383651733398438 GB (4579.5703125 MB free)
  Uptime: 4.2531813e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.1611328125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
