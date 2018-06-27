# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8e5731d0508eba3717655f5cce5a0593a7384f34](https://github.com/JuliaLang/julia/commit/8e5731d0508eba3717655f5cce5a0593a7384f34) vs [JuliaLang/julia@d0e0e2341987b5b7955632c02a99af12a16c7f1e](https://github.com/JuliaLang/julia/commit/d0e0e2341987b5b7955632c02a99af12a16c7f1e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27789#issuecomment-400574941)

*Tag Predicate:* `"sort" || "union"`

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
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigFloat, true)"]` | 1.01 (15%)  | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", BigInt, true)"]` | 0.86 (15%)  | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Bool, true)"]` | 0.63 (15%) :white_check_mark: | 0.65 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float32, true)"]` | 0.85 (15%)  | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float64, true)"]` | 0.84 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int64, true)"]` | 0.68 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int8, true)"]` | 0.66 (15%) :white_check_mark: | 0.65 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "set operations"]`
- `["micro"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.46
Commit 8e5731d (2018-06-27 04:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   36075895 s        278 s    3767847 s  749580739 s          7 s
       #2  3501 MHz  165712196 s          0 s    2290558 s  623441279 s          4 s
       #3  3501 MHz   22371652 s       2377 s    1850471 s  766892420 s         11 s
       #4  3501 MHz   20898746 s          0 s    2127536 s  768231931 s          8 s
       
  Memory: 31.383651733398438 GB (3593.9453125 MB free)
  Uptime: 7.919159e6 sec
  Load Avg:  0.9970703125  1.04052734375  1.4208984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.44
Commit d0e0e23 (2018-06-27 03:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   36188958 s        278 s    3777136 s  749736722 s          7 s
       #2  3501 MHz  165898350 s          0 s    2299420 s  623524801 s          4 s
       #3  3501 MHz   22505127 s       2377 s    1859504 s  767028343 s         11 s
       #4  3501 MHz   21028842 s          0 s    2136451 s  768371556 s          8 s
       
  Memory: 31.383651733398438 GB (5680.7890625 MB free)
  Uptime: 7.921952e6 sec
  Load Avg:  0.9970703125  1.0390625  1.47265625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
