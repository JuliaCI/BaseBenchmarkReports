# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a9d418eba943162e13046b4eddb09bf0dd6c0da9](https://github.com/JuliaLang/julia/commit/a9d418eba943162e13046b4eddb09bf0dd6c0da9) vs [JuliaLang/julia@6bdb3950bdf64152](https://github.com/JuliaLang/julia/commit/6bdb3950bdf64152)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a9d418eba943162e13046b4eddb09bf0dd6c0da9#commitcomment-22177931)

*Tag Predicate:* `"parse"`

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

- `["dates","parse"]`
- `["micro"]`
- `["misc","parse"]`
- `["problem","json"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-rc1.79
Commit a9d418e (2017-05-17 06:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8287.7578125 MB free)
Uptime: 3.0684053e7 sec
Load Avg:  1.0029296875  1.673828125  1.9853515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63748058 s          0 s    9851035 s  2988223792 s         89 s
#2  3501 MHz  247725384 s          0 s   10847909 s  2804206872 s         36 s
#3  3501 MHz   54677350 s          0 s    6365336 s  3005976866 s         46 s
#4  3501 MHz   50236689 s          0 s    6314142 s  3010750886 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-rc1.0
Commit 6bdb395 (2017-05-07 00:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8278.15234375 MB free)
Uptime: 3.0685612e7 sec
Load Avg:  0.99169921875  1.71826171875  2.23779296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63836452 s          0 s    9859352 s  2988282437 s         89 s
#2  3501 MHz  247828735 s          0 s   10856555 s  2804250288 s         36 s
#3  3501 MHz   54766038 s          0 s    6374147 s  3006034663 s         46 s
#4  3501 MHz   50324642 s          0 s    6322593 s  3010809871 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
