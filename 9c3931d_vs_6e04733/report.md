# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9c3931d6f27cceb475c44ba78fe6854838cee449](https://github.com/JuliaLang/julia/commit/9c3931d6f27cceb475c44ba78fe6854838cee449) vs [JuliaLang/julia@6e0473380b2b561b373869cb50f352c3e12d0246](https://github.com/JuliaLang/julia/commit/6e0473380b2b561b373869cb50f352c3e12d0246)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/32097#issuecomment-494182435)

*Tag Predicate:* `"linalg"`

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

- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`

## Version Info

#### Primary Build

```
Julia Version 1.3.0-DEV.259
Commit 9c3931d (2019-05-20 23:15 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   90209987 s       5031 s   10241994 s  3513664670 s         24 s
       #2  3501 MHz  580592766 s        203 s    9710178 s  3029703293 s         21 s
       #3  3501 MHz   73605626 s       3237 s    6095119 s  3540376385 s         30 s
       #4  3501 MHz   69067072 s         14 s    8081688 s  3541808604 s         19 s
       
  Memory: 31.383651733398438 GB (6081.921875 MB free)
  Uptime: 3.6228311e7 sec
  Load Avg:  0.9228515625  1.0322265625  1.35302734375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.3.0-DEV.257
Commit 6e04733 (2019-05-20 21:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   90312048 s       5031 s   10246903 s  3513802427 s         24 s
       #2  3501 MHz  580770497 s        203 s    9714926 s  3029765963 s         21 s
       #3  3501 MHz   73711207 s       3237 s    6100066 s  3540510924 s         30 s
       #4  3501 MHz   69174384 s         14 s    8086390 s  3541941618 s         19 s
       
  Memory: 31.383651733398438 GB (6078.75 MB free)
  Uptime: 3.6230764e7 sec
  Load Avg:  1.0029296875  1.0498046875  1.451171875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
