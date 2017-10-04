# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@285c67aa1c7d9263badb62f07b90f8d65f7b13bc](https://github.com/pkofod/julia/commit/285c67aa1c7d9263badb62f07b90f8d65f7b13bc) vs [JuliaLang/julia@16139d054e29ea63b797537927beee84da1b229d](https://github.com/JuliaLang/julia/commit/16139d054e29ea63b797537927beee84da1b229d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23383#issuecomment-334278083)

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
| `["scalar","atan",("0 <= abs(x) < 7/16","negative argument","Float32")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan",("0 <= abs(x) < 7/16","positive argument","Float32")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan",("11/16 <= abs(x) < 19/16","negative argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("11/16 <= abs(x) < 19/16","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("19/16 <= abs(x) < 39/16","negative argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("19/16 <= abs(x) < 39/16","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("39/16 <= abs(x) < 2^66","negative argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("39/16 <= abs(x) < 2^66","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("7/16 <= abs(x) < 11/16","negative argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("7/16 <= abs(x) < 11/16","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y negative","x negative","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y negative","x positive","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (large)","y positive","x positive","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (small)","y negative","x positive","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("abs(y/x) safe (small)","y positive","x positive","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float32")]` | 1.70 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float64")]` | 1.59 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2053
Commit 285c67a (2017-10-04 18:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96274435 s          0 s   17090236 s  4153890101 s         93 s
       #2  3501 MHz  415355897 s          0 s   11063441 s  3850895579 s         20 s
       #3  3501 MHz   83539661 s          0 s    9483618 s  4184716413 s         77 s
       #4  3501 MHz   79840557 s          0 s    9681668 s  4188215227 s         19 s
       
  Memory: 31.383651733398438 GB (4455.75 MB free)
  Uptime: 4.2797926e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.1767578125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2046
Commit 16139d0 (2017-10-04 06:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96352544 s          0 s   17098234 s  4154094111 s         93 s
       #2  3501 MHz  415584993 s          0 s   11070756 s  3850950085 s         20 s
       #3  3501 MHz   83636314 s          0 s    9491161 s  4184903003 s         77 s
       #4  3501 MHz   79922463 s          0 s    9689246 s  4188416634 s         19 s
       
  Memory: 31.383651733398438 GB (4282.8828125 MB free)
  Uptime: 4.280084e7 sec
  Load Avg:  0.9228515625  0.998046875  1.2333984375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
