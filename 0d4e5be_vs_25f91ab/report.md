# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0d4e5be47a423835b0ca7739412e4fcd11dfb2e4](https://github.com/JuliaLang/julia/commit/0d4e5be47a423835b0ca7739412e4fcd11dfb2e4) vs [JuliaLang/julia@25f91ab3068b92ef28ac462b545908c2d4687c83](https://github.com/JuliaLang/julia/commit/25f91ab3068b92ef28ac462b545908c2d4687c83)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28035)

*Tag Predicate:* `"union"`

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
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 6.56 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int8, true)"]` | 3.72 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "set operations"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.232
Commit 0d4e5be* (2018-07-10 15:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   41308364 s        279 s    4269896 s  858606896 s          9 s
       #2  3501 MHz  189055489 s          0 s    2710757 s  714659288 s          5 s
       #3  3501 MHz   26821320 s       2381 s    2205680 s  876988502 s         14 s
       #4  3501 MHz   25019867 s          0 s    2561273 s  878591133 s          9 s
       
  Memory: 31.383651733398438 GB (2059.27734375 MB free)
  Uptime: 9.069751e6 sec
  Load Avg:  0.9228515625  1.07275390625  1.52587890625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.230
Commit 25f91ab* (2018-07-10 14:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   41416135 s        279 s    4278672 s  858744344 s          9 s
       #2  3501 MHz  189252975 s          0 s    2719541 s  714707564 s          5 s
       #3  3501 MHz   26941268 s       2381 s    2214522 s  877114012 s         14 s
       #4  3501 MHz   25133509 s          0 s    2569658 s  878723703 s          9 s
       
  Memory: 31.383651733398438 GB (3882.31640625 MB free)
  Uptime: 9.072303e6 sec
  Load Avg:  0.84375  1.044921875  1.58544921875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
