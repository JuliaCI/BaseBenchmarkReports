# Benchmark Report

## Job Properties

*Commit(s):* [simeonschaub/julia@c1d05129c4fc0c49401bbb371119287f1bec773e](https://github.com/simeonschaub/julia/commit/c1d05129c4fc0c49401bbb371119287f1bec773e) vs [JuliaLang/julia@f1d10e71aba769f10e6ef340494cac47daaba93a](https://github.com/JuliaLang/julia/commit/f1d10e71aba769f10e6ef340494cac47daaba93a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/35706#issuecomment-623518378)

*Tag Predicate:* `"broadcast"`

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
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"tup_tup\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["broadcast"]`
- `["broadcast", "dotop"]`
- `["broadcast", "fusion"]`
- `["broadcast", "mix_scalar_tuple"]`
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.5.0-DEV.819
Commit c1d0512 (2020-05-04 12:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  137504214 s       5056 s   15679602 s  6475802862 s         35 s
       #2  3501 MHz  1035316599 s        217 s   20349528 s  5583397488 s         26 s
       #3  3501 MHz  122331508 s       3297 s    9293365 s  6506715943 s         38 s
       #4  3501 MHz  114904532 s         43 s   13351168 s  6508383775 s         27 s
       
  Memory: 31.383651733398438 GB (19100.453125 MB free)
  Uptime: 6.6439816e7 sec
  Load Avg:  1.0029296875  1.1513671875  1.6455078125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.5.0-DEV.814
Commit f1d10e7 (2020-05-04 11:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  137660760 s       5056 s   15685822 s  6475909941 s         35 s
       #2  3501 MHz  1035497642 s        217 s   20356468 s  5583479358 s         26 s
       #3  3501 MHz  122475988 s       3297 s    9299314 s  6506835478 s         38 s
       #4  3501 MHz  115055896 s         43 s   13357344 s  6508496205 s         27 s
       
  Memory: 31.383651733398438 GB (19990.20703125 MB free)
  Uptime: 6.644252e7 sec
  Load Avg:  0.9970703125  1.13330078125  1.712890625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
