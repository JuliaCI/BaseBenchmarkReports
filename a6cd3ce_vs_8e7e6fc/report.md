# Benchmark Report

## Job Properties

*Commit(s):* [haampie/julia@a6cd3cee51be3fa1e0fba9813bdd166c142df96e](https://github.com/haampie/julia/commit/a6cd3cee51be3fa1e0fba9813bdd166c142df96e) vs [JuliaLang/julia@8e7e6fc00a9fc407a88b8a997578adcb1d967c7e](https://github.com/JuliaLang/julia/commit/8e7e6fc00a9fc407a88b8a997578adcb1d967c7e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27386#issuecomment-400821826)

*Tag Predicate:* `"collection"`

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
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"unspecified\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"in\", \"false\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"in\", \"true\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"Vector\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "optimizations"]`
- `["collection", "queries & updates"]`
- `["collection", "set operations"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.64
Commit a6cd3ce (2018-06-27 18:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   36308585 s        278 s    3787239 s  753970779 s          7 s
       #2  3501 MHz  166067082 s          0 s    2309721 s  627708211 s          4 s
       #3  3501 MHz   22629418 s       2377 s    1870189 s  771261393 s         11 s
       #4  3501 MHz   21162688 s          0 s    2154457 s  772580004 s          8 s
       
  Memory: 31.383651733398438 GB (4809.71484375 MB free)
  Uptime: 7.965651e6 sec
  Load Avg:  1.0029296875  1.080078125  1.49267578125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.58
Commit 8e7e6fc (2018-06-27 18:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   36425087 s        278 s    3796802 s  754104908 s          7 s
       #2  3501 MHz  166239039 s          0 s    2318171 s  627788245 s          4 s
       #3  3501 MHz   22764456 s       2377 s    1879297 s  771377588 s         12 s
       #4  3501 MHz   21285589 s          0 s    2162905 s  772709192 s          8 s
       
  Memory: 31.383651733398438 GB (4756.69921875 MB free)
  Uptime: 7.968262e6 sec
  Load Avg:  1.0029296875  1.076171875  1.59033203125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
