# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@404da70efb63e018a82cc29ab090341dd55ba921](https://github.com/JuliaLang/julia/commit/404da70efb63e018a82cc29ab090341dd55ba921) vs [JuliaLang/julia@9a2c1445862f69a70d074e9df2bf7469c64b0959](https://github.com/JuliaLang/julia/commit/9a2c1445862f69a70d074e9df2bf7469c64b0959)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/404da70efb63e018a82cc29ab090341dd55ba921#commitcomment-17867166)

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

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["shootout"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4764
Commit 404da70 (2016-06-14 16:49 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27688.53125 MB free)
Uptime: 1.581878e6 sec
Load Avg:  0.99609375  0.92919921875  0.88427734375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     757687 s          0 s     284614 s  156787529 s          4 s
#2  3501 MHz    2106830 s          0 s     229376 s  155718999 s          1 s
#3  3501 MHz     988563 s          0 s     187116 s  156920141 s          1 s
#4  3501 MHz     606910 s          0 s     163096 s  157350839 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4763
Commit 9a2c144 (2016-06-14 16:48 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27680.11328125 MB free)
Uptime: 1.585063e6 sec
Load Avg:  0.9970703125  0.9287109375  0.90673828125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     791823 s          0 s     290242 s  157065380 s          4 s
#2  3501 MHz    2156133 s          0 s     235619 s  155981468 s          1 s
#3  3501 MHz    1124985 s          0 s     196575 s  157092106 s          1 s
#4  3501 MHz     677182 s          0 s     169905 s  157591785 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
