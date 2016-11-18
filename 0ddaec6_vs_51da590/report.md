# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0ddaec6a7f105c4bd5154b913835c03039a395a1](https://github.com/JuliaLang/julia/commit/0ddaec6a7f105c4bd5154b913835c03039a395a1) vs [JuliaLang/julia@51da5900574ee0149bd00f51d0324d8528062002](https://github.com/JuliaLang/julia/commit/51da5900574ee0149bd00f51d0324d8528062002)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19212#issuecomment-261571746)

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
| `["dates","query",("dayofweek","Date")]` | 7842.58 (25%) :x: | Inf (1%) :x: |
| `["dates","query",("dayofweek","DateTime")]` | 6996.81 (25%) :x: | Inf (1%) :x: |
| `["dates","query",("firstdayofweek","DateTime")]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 1.43 (25%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1275
Commit 0ddaec6 (2016-11-18 16:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10628.40625 MB free)
Uptime: 1.5134577e7 sec
Load Avg:  0.9794921875  0.923828125  0.89306640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   24129388 s          0 s    4007774 s  1482212928 s         46 s
#2  3501 MHz   66688220 s          0 s    4688594 s  1439789378 s         16 s
#3  3501 MHz   21035834 s          0 s    2688226 s  1489020876 s         25 s
#4  3501 MHz   17691427 s          0 s    2612163 s  1492567378 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1272
Commit 51da590 (2016-11-18 16:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10532.08984375 MB free)
Uptime: 1.5137859e7 sec
Load Avg:  1.0283203125  0.96044921875  0.91357421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   24255894 s          0 s    4017568 s  1482404161 s         46 s
#2  3501 MHz   66765462 s          0 s    4695979 s  1440032367 s         16 s
#3  3501 MHz   21078696 s          0 s    2695241 s  1489298378 s         25 s
#4  3501 MHz   17742322 s          0 s    2618363 s  1492837896 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
