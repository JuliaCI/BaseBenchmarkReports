# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9a96fc288a6856247d67c1e67743c6f2a90dec0c](https://github.com/JuliaLang/julia/commit/9a96fc288a6856247d67c1e67743c6f2a90dec0c) vs [JuliaLang/julia@a132ae2747564936ea1bbd347d51be6911c6fa1b](https://github.com/JuliaLang/julia/commit/a132ae2747564936ea1bbd347d51be6911c6fa1b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20952#issuecomment-286143799)

*Tag Predicate:* `"dates"`

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
| `["dates","parse","Date"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.19 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.alpha.148
Commit 9a96fc2 (2017-03-13 15:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5732.78125 MB free)
Uptime: 2.5066606e7 sec
Load Avg:  1.0029296875  1.599609375  1.79296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   45783453 s          0 s    9230567 s  2444392023 s         72 s
#2  3501 MHz  177862854 s          0 s    5690844 s  2321638529 s         10 s
#3  3501 MHz   41198227 s          0 s    4985016 s  2459286766 s         52 s
#4  3501 MHz   38800691 s          0 s    5127646 s  2461534555 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.137
Commit a132ae2 (2017-03-13 14:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5666.56640625 MB free)
Uptime: 2.5068156e7 sec
Load Avg:  1.01220703125  1.60205078125  2.1142578125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   45879630 s          0 s    9238386 s  2444442425 s         72 s
#2  3501 MHz  177962136 s          0 s    5699018 s  2321685560 s         10 s
#3  3501 MHz   41281148 s          0 s    4993048 s  2459350103 s         52 s
#4  3501 MHz   38879181 s          0 s    5136383 s  2461601779 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
