# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7784d3c2cdc61717b7aa9cb1e8e08c123ce8beb7](https://github.com/JuliaLang/julia/commit/7784d3c2cdc61717b7aa9cb1e8e08c123ce8beb7) vs [JuliaLang/julia@539879956fee623feeb445d3db4a2a4aee217f73](https://github.com/JuliaLang/julia/commit/539879956fee623feeb445d3db4a2a4aee217f73)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19545#issuecomment-274498070)

*Tag Predicate:* `"dates"`

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
| `["dates","parse","Date"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.31 (15%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.31 (15%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.02 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.03 (15%) :white_check_mark: | 0.18 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.02 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 1.16 (15%) :x: | 1.50 (1%) :x: |
| `["dates","string","DateTime"]` | 0.79 (15%) :white_check_mark: | 1.11 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.2292
Commit 7784d3c (2017-01-23 14:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19941.87109375 MB free)
Uptime: 2.0830263e7 sec
Load Avg:  0.9970703125  0.94140625  0.89404296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   32914921 s          0 s    7143356 s  2037007986 s         63 s
#2  3501 MHz  113911825 s          0 s    4421198 s  1963457797 s          8 s
#3  3501 MHz   30638093 s          0 s    3843078 s  2047556383 s         45 s
#4  3501 MHz   28372629 s          0 s    3961588 s  2049698967 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2269
Commit 5398799 (2017-01-23 07:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19838.58984375 MB free)
Uptime: 2.0833885e7 sec
Load Avg:  1.02099609375  0.9677734375  0.9189453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33004688 s          0 s    7152050 s  2037270794 s         63 s
#2  3501 MHz  114030228 s          0 s    4429686 s  1963692698 s          8 s
#3  3501 MHz   30704193 s          0 s    3850588 s  2047844230 s         45 s
#4  3501 MHz   28428957 s          0 s    3968640 s  2049997165 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
