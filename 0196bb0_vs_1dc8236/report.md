# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0196bb0d620ae944d6a8b7357b1d3e922c0cbfc1](https://github.com/JuliaLang/julia/commit/0196bb0d620ae944d6a8b7357b1d3e922c0cbfc1) vs [JuliaLang/julia@1dc8236fdea998b66b60368174ed5399398611b2](https://github.com/JuliaLang/julia/commit/1dc8236fdea998b66b60368174ed5399398611b2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/31762#issuecomment-484647120)

*Tag Predicate:* `"collection" || "iteration"`

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
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate second\")"]` | 0.21 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate\")"]` | 0.14 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"iterate second\")"]` | 0.11 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"iterate\")"]` | 0.11 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate second\")"]` | 0.15 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate\")"]` | 0.14 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Set\", \"Int\", \"iterate second\")"]` | 0.11 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"iterate\")"]` | 0.13 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"String\", \"iterate second\")"]` | 0.14 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Set\", \"String\", \"iterate\")"]` | 0.15 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"false\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"true\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"new\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "comprehension"]`
- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "optimizations"]`
- `["collection", "queries & updates"]`
- `["collection", "set operations"]`
- `["scalar", "iteration"]`

## Version Info

#### Primary Build

```
Julia Version 1.3.0-DEV.68
Commit 0196bb0 (2019-04-18 17:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   85261064 s       5022 s    9649900 s  3241914848 s         24 s
       #2  3501 MHz  531250984 s        203 s    8919514 s  2802063186 s         20 s
       #3  3501 MHz   68451997 s       3234 s    5757307 s  3268027906 s         29 s
       #4  3501 MHz   64358204 s         12 s    7631757 s  3269237160 s         18 s
       
  Memory: 31.383651733398438 GB (5559.7578125 MB free)
  Uptime: 3.3448613e7 sec
  Load Avg:  1.0029296875  1.06689453125  1.38427734375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.3.0-DEV.66
Commit 1dc8236 (2019-04-18 17:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   85365550 s       5022 s    9654598 s  3242042109 s         24 s
       #2  3501 MHz  531424942 s        203 s    8924705 s  2802120782 s         20 s
       #3  3501 MHz   68552745 s       3234 s    5762315 s  3268158820 s         29 s
       #4  3501 MHz   64463632 s         12 s    7636316 s  3269363961 s         18 s
       
  Memory: 31.383651733398438 GB (5455.4296875 MB free)
  Uptime: 3.3450984e7 sec
  Load Avg:  0.9169921875  1.044921875  1.48876953125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
