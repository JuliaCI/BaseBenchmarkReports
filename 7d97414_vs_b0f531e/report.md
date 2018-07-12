# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7d97414a9fe938b33ef10540fc246b37e6c99344](https://github.com/JuliaLang/julia/commit/7d97414a9fe938b33ef10540fc246b37e6c99344) vs [JuliaLang/julia@b0f531e5f0b626f1ee91bb7cac2a0bb660f435f3](https://github.com/JuliaLang/julia/commit/b0f531e5f0b626f1ee91bb7cac2a0bb660f435f3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28035#issuecomment-404628293)

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
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 1.28 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "set operations"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.281
Commit 7d97414* (2018-07-12 19:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   42182681 s        279 s    4358633 s  876440483 s          9 s
       #2  3501 MHz  193830476 s          0 s    2793620 s  728629389 s          6 s
       #3  3501 MHz   27706924 s       2381 s    2273626 s  894864043 s         14 s
       #4  3501 MHz   25823556 s          0 s    2635348 s  896539066 s          9 s
       
  Memory: 31.383651733398438 GB (4619.45703125 MB free)
  Uptime: 9.258208e6 sec
  Load Avg:  0.9228515625  1.0693359375  1.52294921875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.279
Commit b0f531e* (2018-07-12 15:33 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   42313199 s        279 s    4367341 s  876555979 s          9 s
       #2  3501 MHz  194006980 s          0 s    2802597 s  728698857 s          6 s
       #3  3501 MHz   27828804 s       2381 s    2282368 s  894988207 s         15 s
       #4  3501 MHz   25934825 s          0 s    2644197 s  896673841 s          9 s
       
  Memory: 31.383651733398438 GB (6378.8984375 MB free)
  Uptime: 9.260763e6 sec
  Load Avg:  0.9970703125  1.08349609375  1.6083984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
