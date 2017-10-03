# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@fee69fc10356dd407041e564597f5f45b14a25b2](https://github.com/pkofod/julia/commit/fee69fc10356dd407041e564597f5f45b14a25b2) vs [JuliaLang/julia@6159bcb45161304e4c5fd915991d82e8ee56797b](https://github.com/JuliaLang/julia/commit/6159bcb45161304e4c5fd915991d82e8ee56797b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22824#issuecomment-333750332)

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
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","cos_kernel")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","cos_kernel")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","cos_kernel")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32","sin_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float32","cos_kernel")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float32")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float64")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","sin_kernel")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","cos_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","sin_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float64","sin_kernel")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float64","sin_kernel")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float32")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float64")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2049
Commit fee69fc (2017-10-03 06:15 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87926553 s          0 s   13668492 s  4154958395 s        175 s
       #2  3501 MHz  354264839 s          0 s   14656978 s  3889677380 s         62 s
       #3  3501 MHz   73519162 s          0 s    8406071 s  4182338517 s         83 s
       #4  3501 MHz   68856691 s          0 s    8281450 s  4187526615 s         30 s
       
  Memory: 31.383651733398438 GB (3767.14453125 MB free)
  Uptime: 4.2660908e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.1337890625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2038
Commit 6159bcb (2017-10-03 03:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88009823 s          0 s   13676792 s  4155193414 s        175 s
       #2  3501 MHz  354530948 s          0 s   14664609 s  3889730792 s         62 s
       #3  3501 MHz   73617587 s          0 s    8413871 s  4182559422 s         84 s
       #4  3501 MHz   68937964 s          0 s    8289235 s  4187764788 s         30 s
       
  Memory: 31.383651733398438 GB (3703.98828125 MB free)
  Uptime: 4.2664188e7 sec
  Load Avg:  0.9970703125  1.0146484375  1.15380859375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
