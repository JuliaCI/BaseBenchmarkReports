# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@ad87f5e5974787741460b50310fa199c014c377b](https://github.com/pkofod/julia/commit/ad87f5e5974787741460b50310fa199c014c377b) vs [JuliaLang/julia@cd8f33ea9989a0364d01f7b55249379eec1643f0](https://github.com/JuliaLang/julia/commit/cd8f33ea9989a0364d01f7b55249379eec1643f0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22603#issuecomment-317902881)

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
| `["scalar","mod2pi",("argument reduction (easy) |x| > 2.0^20*π/2","negative argument","Float64")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) |x| > 2.0^20*π/2","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 2.0^20π/4","negative argument","Float64")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 2.0^20π/4","positive argument","Float64")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 2π/4","negative argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 2π/4","positive argument","Float64")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 3π/4","negative argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 3π/4","positive argument","Float64")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 4π/4","negative argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 4π/4","positive argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 5π/4","negative argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 5π/4","positive argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 6π/4","negative argument","Float64")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 6π/4","positive argument","Float64")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 7π/4","negative argument","Float64")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 7π/4","positive argument","Float64")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 8π/4","negative argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 8π/4","positive argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 9π/4","negative argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) |x| < 9π/4","positive argument","Float64")]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 2π/4","negative argument","Float64")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 2π/4","positive argument","Float64")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 4π/4","negative argument","Float64")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 4π/4","positive argument","Float64")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 6π/4","negative argument","Float64")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 6π/4","positive argument","Float64")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 8π/4","negative argument","Float64")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) |x| < 8π/4","positive argument","Float64")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) |x| > 2.0^20*π/2","negative argument","Float64")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) |x| > 2.0^20*π/2","positive argument","Float64")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["scalar","arithmetic"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1157
Commit ad87f5e (2017-07-25 22:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78797992 s          0 s   14432763 s  3563525098 s         85 s
       #2  3501 MHz  321054598 s          0 s    8937171 s  3335324933 s         13 s
       #3  3501 MHz   68628962 s          0 s    7981802 s  3589091661 s         70 s
       #4  3501 MHz   65437843 s          0 s    8176178 s  3592066186 s         16 s
       
  Memory: 31.383651733398438 GB (2707.65234375 MB free)
  Uptime: 3.6674537e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.16796875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1107
Commit cd8f33e (2017-07-24 20:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78877100 s          0 s   14440022 s  3563699738 s         85 s
       #2  3501 MHz  321259059 s          0 s    8944580 s  3335374538 s         13 s
       #3  3501 MHz   68708858 s          0 s    7988960 s  3589265877 s         70 s
       #4  3501 MHz   65529046 s          0 s    8183408 s  3592229314 s         16 s
       
  Memory: 31.383651733398438 GB (2600.62109375 MB free)
  Uptime: 3.6677157e7 sec
  Load Avg:  0.9970703125  1.0146484375  1.29638671875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
