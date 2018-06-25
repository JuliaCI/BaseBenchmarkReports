# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@67a284a07147b9e58f460a18c21b15c2209d3296](https://github.com/JuliaLang/julia/commit/67a284a07147b9e58f460a18c21b15c2209d3296) vs [JuliaLang/julia@0978251ac5223ffc650c0e8a3c20fb0af83e9d4a](https://github.com/JuliaLang/julia/commit/0978251ac5223ffc650c0e8a3c20fb0af83e9d4a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27764)

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
| `["micro", "fib"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["misc", "parse", "Float64"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta.9
Commit 67a284a (2018-06-25 08:15 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   33974446 s        278 s    3583108 s  734972490 s          6 s
       #2  3501 MHz  151585861 s          0 s    2112664 s  620795802 s          4 s
       #3  3501 MHz   20397748 s       2377 s    1705702 s  752065044 s         11 s
       #4  3501 MHz   19050066 s          0 s    1983363 s  753276688 s          7 s
       
  Memory: 31.383651733398438 GB (4080.0234375 MB free)
  Uptime: 7.749544e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.10888671875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.7
Commit 0978251 (2018-06-25 01:11 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   34080192 s        278 s    3592782 s  735261659 s          6 s
       #2  3501 MHz  151924098 s          0 s    2121596 s  620854175 s          4 s
       #3  3501 MHz   20522132 s       2377 s    1714622 s  752336984 s         11 s
       #4  3501 MHz   19172140 s          0 s    1992308 s  753551051 s          7 s
       
  Memory: 31.383651733398438 GB (3973.0234375 MB free)
  Uptime: 7.753605e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.1240234375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
