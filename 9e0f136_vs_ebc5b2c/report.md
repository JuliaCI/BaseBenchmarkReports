# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9e0f136319ddc445a700bf5c18b12622f091f781](https://github.com/JuliaLang/julia/commit/9e0f136319ddc445a700bf5c18b12622f091f781) vs [JuliaLang/julia@ebc5b2c51e227942d3a8894df500f8f270db006b](https://github.com/JuliaLang/julia/commit/ebc5b2c51e227942d3a8894df500f8f270db006b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25713#issuecomment-360622805)

*Tag Predicate:* `"string" && "readuntil"`

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
| `["string", "readuntil", "backtracking"]` | 18.59 (15%) :x: | 48.33 (1%) :x: |
| `["string", "readuntil", "barbarian backtrack"]` | 11.76 (15%) :x: | 43.41 (1%) :x: |
| `["string", "readuntil", "no backtracking"]` | 8.67 (15%) :x: | 11.56 (1%) :x: |
| `["string", "readuntil", "target length 1000"]` | 6.50 (15%) :x: | 10.51 (1%) :x: |
| `["string", "readuntil", "target length 2"]` | 2.65 (15%) :x: | 1.22 (1%) :x: |
| `["string", "readuntil", "target length 50000"]` | 7.08 (15%) :x: | 24.34 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3580
Commit 9e0f136 (2018-01-25 22:04 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  105940359 s          0 s   16322956 s  5122638007 s        263 s
       #2  3501 MHz  414305036 s          0 s   17460938 s  4815773535 s         84 s
       #3  3501 MHz   83653864 s          0 s    9492905 s  5161524021 s        113 s
       #4  3501 MHz   78851900 s          0 s    9400152 s  5166855089 s         47 s
       
  Memory: 31.383651733398438 GB (3792.32421875 MB free)
  Uptime: 5.2567566e7 sec
  Load Avg:  1.0048828125  1.42236328125  1.90966796875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3578
Commit ebc5b2c (2018-01-25 22:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  106027130 s          0 s   16331247 s  5122713786 s        263 s
       #2  3501 MHz  414428166 s          0 s   17469067 s  4815813318 s         84 s
       #3  3501 MHz   83745043 s          0 s    9501131 s  5161595546 s        113 s
       #4  3501 MHz   78937018 s          0 s    9408504 s  5166932638 s         47 s
       
  Memory: 31.383651733398438 GB (3776.5625 MB free)
  Uptime: 5.2569283e7 sec
  Load Avg:  1.00830078125  1.4443359375  2.05224609375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
