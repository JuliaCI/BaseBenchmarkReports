# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@278d064b84ba08e0c6ab1c340cb0baede902bb60](https://github.com/JuliaLang/julia/commit/278d064b84ba08e0c6ab1c340cb0baede902bb60) vs [JuliaLang/julia@e0c497b22289487aff417380cdbdefa77255dd3b](https://github.com/JuliaLang/julia/commit/e0c497b22289487aff417380cdbdefa77255dd3b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21514)

*Tag Predicate:* `"serialization"`

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
| `["io","serialization",("deserialize","Vector{String}")]` | 0.62 (15%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.73 (15%) :white_check_mark: | 0.81 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["io","serialization"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.295
Commit 278d064 (2017-04-24 01:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3470.6171875 MB free)
Uptime: 2.8645259e7 sec
Load Avg:  0.99951171875  1.8017578125  1.88134765625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   58454520 s          0 s    9057312 s  2790884800 s         85 s
#2  3501 MHz  220285923 s          0 s    9965261 s  2628964817 s         33 s
#3  3501 MHz   49282632 s          0 s    5751722 s  2808212611 s         44 s
#4  3501 MHz   44835585 s          0 s    5705992 s  2812967669 s         15 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.293
Commit e0c497b (2017-04-23 19:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3547.18359375 MB free)
Uptime: 2.8646737e7 sec
Load Avg:  1.03125  1.8330078125  2.26953125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   58547568 s          0 s    9065974 s  2790930241 s         85 s
#2  3501 MHz  220382612 s          0 s    9973585 s  2629007147 s         33 s
#3  3501 MHz   49366158 s          0 s    5760496 s  2808267444 s         44 s
#4  3501 MHz   44917666 s          0 s    5714102 s  2813024730 s         15 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
