# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7f5e2f61882cb23fd9c0b6e8d133c7bd4252c687](https://github.com/JuliaLang/julia/commit/7f5e2f61882cb23fd9c0b6e8d133c7bd4252c687) vs [JuliaLang/julia@05fb47d83915d94912dd3dad783fac037125e07e](https://github.com/JuliaLang/julia/commit/05fb47d83915d94912dd3dad783fac037125e07e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/29879#issuecomment-435254080)

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
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "parse", "Int"]` | 1.07 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.1.0-DEV.602
Commit 7f5e2f6 (2018-11-02 02:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   37673273 s       2410 s    6116323 s  1846433234 s         10 s
       #2  3501 MHz  198877013 s         12 s    3539956 s  1691976671 s         16 s
       #3  3501 MHz   28796917 s       3135 s    3333085 s  1862084427 s         24 s
       #4  3501 MHz   27696089 s         11 s    2617830 s  1864831457 s         19 s
       
  Memory: 31.383651733398438 GB (5178.90234375 MB free)
  Uptime: 1.89601e7 sec
  Load Avg:  0.9970703125  1.2763671875  1.72119140625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.600
Commit 05fb47d (2018-11-02 01:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   37799694 s       2410 s    6123503 s  1846512672 s         10 s
       #2  3501 MHz  199017666 s         12 s    3546836 s  1692042394 s         16 s
       #3  3501 MHz   28919682 s       3135 s    3340325 s  1862167271 s         24 s
       #4  3501 MHz   27801451 s         11 s    2624888 s  1864932268 s         19 s
       
  Memory: 31.383651733398438 GB (5167.375 MB free)
  Uptime: 1.8962238e7 sec
  Load Avg:  1.0029296875  1.2763671875  1.8701171875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
