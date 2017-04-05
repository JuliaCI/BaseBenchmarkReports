# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c49440a05470275d99c5e1f861c43bac68ce0969](https://github.com/JuliaLang/julia/commit/c49440a05470275d99c5e1f861c43bac68ce0969) vs [JuliaLang/julia@a5b993c43074ea45288531b1cdc74bc51f663507](https://github.com/JuliaLang/julia/commit/a5b993c43074ea45288531b1cdc74bc51f663507)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21277#issuecomment-291943258)

*Tag Predicate:* `"simd"`

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
| `["simd",("conditional_loop!","Float32",4096)]` | 0.80 (20%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","index"]`
- `["problem","seismic"]`
- `["simd"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.33
Commit c49440a (2017-04-05 06:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5785.9453125 MB free)
Uptime: 2.7063073e7 sec
Load Avg:  1.01953125  1.0537109375  1.3408203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   55259662 s          0 s    8573371 s  2636749063 s         79 s
#2  3501 MHz  204968694 s          0 s    9400860 s  2487472167 s         29 s
#3  3501 MHz   46274776 s          0 s    5417474 s  2653408026 s         43 s
#4  3501 MHz   41931731 s          0 s    5357851 s  2658061554 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.30
Commit a5b993c (2017-04-05 04:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5639.75390625 MB free)
Uptime: 2.7065468e7 sec
Load Avg:  1.0029296875  1.0419921875  1.44287109375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   55354708 s          0 s    8582374 s  2636883551 s         79 s
#2  3501 MHz  205153130 s          0 s    9409125 s  2487518491 s         29 s
#3  3501 MHz   46359678 s          0 s    5425825 s  2653553612 s         43 s
#4  3501 MHz   42013978 s          0 s    5366314 s  2658209831 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
