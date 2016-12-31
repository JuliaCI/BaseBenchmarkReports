# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@49759ffc7f1948bfc72ffc8f48891de0ea2c9ea4](https://github.com/JuliaLang/julia/commit/49759ffc7f1948bfc72ffc8f48891de0ea2c9ea4) vs [JuliaLang/julia@6629f5124f774933c98dec881001b11f17ff53f2](https://github.com/JuliaLang/julia/commit/6629f5124f774933c98dec881001b11f17ff53f2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269876694)

*Tag Predicate:* `"io"`

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
| `["io","serialization",("deserialize","Vector{String}")]` | 0.28 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.38 (15%) :white_check_mark: | 1.11 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["io","read"]`
- `["io","serialization"]`
- `["parallel","remotecall"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1834
Commit 49759ff (2016-12-31 18:19 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3563.56640625 MB free)
Uptime: 1.8857729e7 sec
Load Avg:  1.02685546875  0.953125  0.90380859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   32022591 s          0 s    5139505 s  1844793214 s         55 s
#2  3501 MHz   96996172 s          0 s    6171331 s  1779465523 s         20 s
#3  3501 MHz   27394045 s          0 s    3457541 s  1854054652 s         32 s
#4  3501 MHz   23283494 s          0 s    3360441 s  1858421782 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1829
Commit 6629f51 (2016-12-31 17:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3551.7734375 MB free)
Uptime: 1.8861265e7 sec
Load Avg:  1.12255859375  0.95263671875  0.9140625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   32102265 s          0 s    5148083 s  1845057766 s         55 s
#2  3501 MHz   97051069 s          0 s    6178105 s  1779756626 s         20 s
#3  3501 MHz   27451945 s          0 s    3463973 s  1854343100 s         32 s
#4  3501 MHz   23412140 s          0 s    3371365 s  1858635241 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
