# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c8d3875b5fe8df5cb57e0a7b9976d41199fb550a](https://github.com/JuliaLang/julia/commit/c8d3875b5fe8df5cb57e0a7b9976d41199fb550a) vs [JuliaLang/julia@06fa32c40ca838152cac38182690266eaa3af60c](https://github.com/JuliaLang/julia/commit/06fa32c40ca838152cac38182690266eaa3af60c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19545#issuecomment-274721383)

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
| `["dates","parse","Date"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.31 (15%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.31 (15%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.02 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.02 (15%) :white_check_mark: | 0.18 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.02 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
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
Julia Version 0.6.0-dev.2303
Commit c8d3875 (2017-01-24 06:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19832.203125 MB free)
Uptime: 2.0888893e7 sec
Load Avg:  0.9365234375  0.953125  0.91455078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33163816 s          0 s    7171142 s  2042580222 s         63 s
#2  3501 MHz  114113948 s          0 s    4440116 s  1969095361 s          8 s
#3  3501 MHz   30751532 s          0 s    3859676 s  2053284798 s         45 s
#4  3501 MHz   28469874 s          0 s    3978302 s  2055444040 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2279
Commit 06fa32c (2017-01-24 04:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19952.76953125 MB free)
Uptime: 2.0892519e7 sec
Load Avg:  0.99560546875  0.9521484375  0.95068359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33225961 s          0 s    7178007 s  2042872807 s         63 s
#2  3501 MHz  114172289 s          0 s    4446720 s  1969392517 s          8 s
#3  3501 MHz   30799640 s          0 s    3866548 s  2053591668 s         45 s
#4  3501 MHz   28632375 s          0 s    3989463 s  2055632511 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
