# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5d90ab6f1407ff934825cfa234f8db378ec1161e](https://github.com/JuliaLang/julia/commit/5d90ab6f1407ff934825cfa234f8db378ec1161e) vs [JuliaLang/julia@c38a5a3044ffd62c585225a201422f95fd18f6dc](https://github.com/JuliaLang/julia/commit/c38a5a3044ffd62c585225a201422f95fd18f6dc)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/5d90ab6f1407ff934825cfa234f8db378ec1161e#commitcomment-20388297)

*Tag Predicate:* `"nullablearray"`

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

- `["nullable","nullablearray"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1960
Commit 5d90ab6 (2017-01-06 15:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4464.265625 MB free)
Uptime: 1.9367386e7 sec
Load Avg:  0.9970703125  0.95068359375  0.90478515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   34721000 s          0 s    5506084 s  1892567486 s         58 s
#2  3501 MHz  108363632 s          0 s    6488317 s  1818676284 s         20 s
#3  3501 MHz   30233855 s          0 s    3733601 s  1901868970 s         33 s
#4  3501 MHz   25636304 s          0 s    3619114 s  1906750787 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1843
Commit c38a5a3 (2017-01-01 14:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4425.09765625 MB free)
Uptime: 1.9370989e7 sec
Load Avg:  1.0078125  0.95703125  0.9482421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   34860253 s          0 s    5516177 s  1892777702 s         58 s
#2  3501 MHz  108432488 s          0 s    6496094 s  1818959303 s         20 s
#3  3501 MHz   30276037 s          0 s    3739813 s  1902179994 s         33 s
#4  3501 MHz   25713860 s          0 s    3627477 s  1907024594 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
