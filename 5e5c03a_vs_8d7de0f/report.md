# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5e5c03a5ba0d9841ac252fc01624813ff36b8d74](https://github.com/JuliaLang/julia/commit/5e5c03a5ba0d9841ac252fc01624813ff36b8d74) vs [JuliaLang/julia@8d7de0f40a300f35516a6dc51004c0aeb3a485d8](https://github.com/JuliaLang/julia/commit/8d7de0f40a300f35516a6dc51004c0aeb3a485d8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27417#issuecomment-396856126)

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
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 1.26 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "set operations"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha.103
Commit 5e5c03a (2018-06-13 08:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   11438997 s        256 s    2067259 s  655816996 s          5 s
       #2  3501 MHz   56103658 s          0 s     931212 s  613576996 s          4 s
       #3  3501 MHz    7645014 s       2388 s    1073027 s  662029863 s         10 s
       #4  3501 MHz    7399722 s          4 s     754403 s  662922144 s          2 s
       
  Memory: 31.383651733398438 GB (4100.421875 MB free)
  Uptime: 6.713477e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.08740234375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.101
Commit 8d7de0f (2018-06-13 07:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   11551050 s        256 s    2076859 s  656128457 s          5 s
       #2  3501 MHz   56443524 s          0 s     940408 s  613662314 s          4 s
       #3  3501 MHz    7766804 s       2388 s    1081838 s  662333421 s         10 s
       #4  3501 MHz    7543428 s          4 s     763161 s  663204078 s          2 s
       
  Memory: 31.383651733398438 GB (6209.7734375 MB free)
  Uptime: 6.717827e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.095703125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
