# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@19b4012521e971837bbb6fcefd308d0019f3d20d](https://github.com/JuliaLang/julia/commit/19b4012521e971837bbb6fcefd308d0019f3d20d) vs [JuliaLang/julia@1093977c989a3f7bef4e791d58055c30ee2fee10](https://github.com/JuliaLang/julia/commit/1093977c989a3f7bef4e791d58055c30ee2fee10)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21514#issuecomment-297618495)

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
Julia Version 0.6.0-pre.beta.363
Commit 19b4012 (2017-04-27 05:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2771.30859375 MB free)
Uptime: 2.8919701e7 sec
Load Avg:  1.00390625  1.82080078125  1.89453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   57386898 s          0 s   11087456 s  2815078176 s         77 s
#2  3501 MHz  233108036 s          0 s    6888022 s  2650285195 s         11 s
#3  3501 MHz   51524042 s          0 s    6117298 s  2832941354 s         59 s
#4  3501 MHz   48785368 s          0 s    6264564 s  2835535639 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.361
Commit 1093977 (2017-04-27 05:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2680.95703125 MB free)
Uptime: 2.8921152e7 sec
Load Avg:  1.0361328125  1.85302734375  2.27001953125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   57479719 s          0 s   11095525 s  2815121776 s         77 s
#2  3501 MHz  233202546 s          0 s    6896430 s  2650326842 s         11 s
#3  3501 MHz   51605577 s          0 s    6125584 s  2832995934 s         59 s
#4  3501 MHz   48864609 s          0 s    6272995 s  2835592534 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
