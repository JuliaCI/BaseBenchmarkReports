# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@725a14bc86db564bbb0945b00568d0740bc301f8](https://github.com/JuliaLang/julia/commit/725a14bc86db564bbb0945b00568d0740bc301f8) vs [JuliaLang/julia@379c248bb02690651a6f5cc2bbdb4f991ad3af9b](https://github.com/JuliaLang/julia/commit/379c248bb02690651a6f5cc2bbdb4f991ad3af9b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18259#issuecomment-242905569)

*Tag Predicate:* `"string" && "problem"`

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

- `["problem","spellcheck"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.421
Commit 725a14b (2016-08-27 08:06 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20496.04296875 MB free)
Uptime: 7.936704e6 sec
Load Avg:  1.01318359375  0.94091796875  0.88671875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13603740 s          0 s    2754516 s  775043819 s         28 s
#2  3501 MHz   34663597 s          0 s    1718175 s  756745837 s          4 s
#3  3501 MHz   11992596 s          0 s    1495768 s  779798816 s         17 s
#4  3501 MHz   10406366 s          0 s    1508965 s  781358719 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.419
Commit 379c248 (2016-08-27 08:05 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20493.953125 MB free)
Uptime: 7.939943e6 sec
Load Avg:  1.01025390625  0.92138671875  0.912109375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13635218 s          0 s    2760267 s  775329529 s         28 s
#2  3501 MHz   34721410 s          0 s    1725440 s  757004144 s          4 s
#3  3501 MHz   12142356 s          0 s    1506877 s  779961281 s         17 s
#4  3501 MHz   10460802 s          0 s    1515146 s  781621334 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
