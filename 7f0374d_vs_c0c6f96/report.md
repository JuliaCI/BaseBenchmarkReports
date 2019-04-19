# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7f0374dc5f0f80a71f2d91213777098133f795b1](https://github.com/JuliaLang/julia/commit/7f0374dc5f0f80a71f2d91213777098133f795b1) vs [JuliaLang/julia@c0c6f96b78b057a0c7e8360a1f6df9c4be2a900b](https://github.com/JuliaLang/julia/commit/c0c6f96b78b057a0c7e8360a1f6df9c4be2a900b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/29879#issuecomment-484818800)

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
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "DateTime"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "parseint"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["misc", "parse", "Int"]` | 1.14 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.3.0-DEV.80
Commit 7f0374d (2019-04-19 09:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   47339248 s       2433 s   10445541 s  3281546864 s         12 s
       #2  3501 MHz  275857428 s         14 s    4958139 s  3066463293 s         19 s
       #3  3501 MHz   38335567 s       3165 s    4612332 s  3304198266 s         29 s
       #4  3501 MHz   36963659 s         15 s    3470564 s  3308144709 s         25 s
       
  Memory: 31.383651733398438 GB (6232.6953125 MB free)
  Uptime: 3.3498023e7 sec
  Load Avg:  0.9169921875  1.2646484375  1.63671875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.3.0-DEV.78
Commit c0c6f96 (2019-04-19 07:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   47443004 s       2433 s   10450277 s  3281627251 s         12 s
       #2  3501 MHz  275981868 s         14 s    4962751 s  3066523232 s         19 s
       #3  3501 MHz   38448401 s       3165 s    4616951 s  3304269767 s         29 s
       #4  3501 MHz   37057138 s         15 s    3475032 s  3308235753 s         25 s
       
  Memory: 31.383651733398438 GB (6155.0625 MB free)
  Uptime: 3.3499916e7 sec
  Load Avg:  1.01220703125  1.31103515625  1.85107421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
