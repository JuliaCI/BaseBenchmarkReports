# Benchmark Report

## Job Properties

*Commit(s):* [TotalVerb/julia@0cb81b86dbf78d3ba19270f7154186f56130616e](https://github.com/TotalVerb/julia/commit/0cb81b86dbf78d3ba19270f7154186f56130616e) vs [JuliaLang/julia@9ed7d828ff8b8bf5c609012acae5279aab3a565a](https://github.com/JuliaLang/julia/commit/9ed7d828ff8b8bf5c609012acae5279aab3a565a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21290#issuecomment-292168646)

*Tag Predicate:* `"nullable"`

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

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["nullable","basic"]`
- `["nullable","nullablearray"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.36
Commit 0cb81b8 (2017-04-05 22:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2766.55859375 MB free)
Uptime: 2.713164e7 sec
Load Avg:  1.0029296875  1.47705078125  1.75341796875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52007205 s          0 s   10226920 s  2643047064 s         74 s
#2  3501 MHz  207381444 s          0 s    6284715 s  2497918235 s         11 s
#3  3501 MHz   46257455 s          0 s    5550965 s  2660062086 s         56 s
#4  3501 MHz   43744823 s          0 s    5689437 s  2662438447 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.33
Commit 9ed7d82 (2017-04-05 21:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2705.03515625 MB free)
Uptime: 2.713327e7 sec
Load Avg:  0.9228515625  1.43798828125  2.01220703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52104304 s          0 s   10235101 s  2643104230 s         74 s
#2  3501 MHz  207487932 s          0 s    6293215 s  2497965867 s         11 s
#3  3501 MHz   46340999 s          0 s    5559363 s  2660132555 s         56 s
#4  3501 MHz   43823657 s          0 s    5698041 s  2662513417 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
