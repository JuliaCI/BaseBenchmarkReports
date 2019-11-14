# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a8f87f3c275c0023305f8acc400d32f94f1748f1](https://github.com/JuliaLang/julia/commit/a8f87f3c275c0023305f8acc400d32f94f1748f1) vs [JuliaLang/julia@77a4d06bf2283848e7a471731fef47f8e6275c8c](https://github.com/JuliaLang/julia/commit/77a4d06bf2283848e7a471731fef47f8e6275c8c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33717#issuecomment-554046003)

*Tag Predicate:* `"shootout"`

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
| `["shootout", "binary_trees"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["shootout"]`

## Version Info

#### Primary Build

```
Julia Version 1.4.0-DEV.465
Commit a8f87f3 (2019-11-14 19:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   53377676 s       2445 s   15794477 s  5073532773 s         16 s
       #2  3501 MHz  327271875 s         44 s    6354728 s  4822334097 s         25 s
       #3  3501 MHz   44469020 s       3198 s    5261805 s  5106023943 s         36 s
       #4  3501 MHz   42848598 s         16 s    4081865 s  5110873644 s         32 s
       
  Memory: 31.383651733398438 GB (14433.203125 MB free)
  Uptime: 5.1594078e7 sec
  Load Avg:  1.00732421875  1.30322265625  1.64208984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.461
Commit 77a4d06 (2019-11-14 15:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   53479401 s       2445 s   15798741 s  5073615464 s         16 s
       #2  3501 MHz  327391756 s         44 s    6359584 s  4822398238 s         25 s
       #3  3501 MHz   44570996 s       3198 s    5266216 s  5106106324 s         36 s
       #4  3501 MHz   42963131 s         16 s    4086568 s  5110943286 s         32 s
       
  Memory: 31.383651733398438 GB (14452.48046875 MB free)
  Uptime: 5.159597e7 sec
  Load Avg:  0.927734375  1.28173828125  1.8388671875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
