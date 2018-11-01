# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f109bb75bba19ffb6f74a87063aea33cf06ab53e](https://github.com/JuliaLang/julia/commit/f109bb75bba19ffb6f74a87063aea33cf06ab53e) vs [JuliaLang/julia@13694f4210f42a8e7a0d282296422b1d0a07b0f4](https://github.com/JuliaLang/julia/commit/13694f4210f42a8e7a0d282296422b1d0a07b0f4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/29892#issuecomment-435130019)

*Tag Predicate:* `"parse"`

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
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["micro", "parseint"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "parse", "Int"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates", "parse"]`
- `["micro"]`
- `["misc", "julia"]`
- `["misc", "parse"]`
- `["problem", "json"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-DEV.599
Commit f109bb7 (2018-11-01 20:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   59851008 s       5004 s    6540119 s  1822591863 s         21 s
       #2  3501 MHz  322002750 s        203 s    5136070 s  1565157035 s         15 s
       #3  3501 MHz   44292390 s       3209 s    3752894 s  1844237472 s         25 s
       #4  3501 MHz   41108808 s          0 s    4662112 s  1846181454 s         14 s
       
  Memory: 31.383651733398438 GB (6192.109375 MB free)
  Uptime: 1.8939163e7 sec
  Load Avg:  1.0029296875  1.31494140625  1.861328125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.589
Commit 13694f4 (2018-11-01 00:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   59982634 s       5004 s    6547362 s  1822666003 s         21 s
       #2  3501 MHz  322142259 s        203 s    5142791 s  1565224075 s         15 s
       #3  3501 MHz   44404787 s       3209 s    3760110 s  1844330705 s         25 s
       #4  3501 MHz   41221378 s          0 s    4669267 s  1846274840 s         14 s
       
  Memory: 31.383651733398438 GB (6145.98828125 MB free)
  Uptime: 1.8941301e7 sec
  Load Avg:  1.0029296875  1.26806640625  1.873046875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
