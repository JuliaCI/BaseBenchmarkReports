# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e146e0d5824d8e353780ff75af78bf94167c0505](https://github.com/JuliaLang/julia/commit/e146e0d5824d8e353780ff75af78bf94167c0505) vs [JuliaLang/julia@b7dc60f7b4e972610846a506b7405f3631bec364](https://github.com/JuliaLang/julia/commit/b7dc60f7b4e972610846a506b7405f3631bec364)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27874#issuecomment-401663456)

*Tag Predicate:* `"string" && "join"`

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

- `["string"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.117
Commit e146e0d (2018-07-02 03:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   20972708 s        259 s    3029215 s  807021408 s          6 s
       #2  3501 MHz  105103543 s          0 s    1656151 s  725913317 s          6 s
       #3  3501 MHz   15503344 s       2392 s    1734165 s  815576856 s         13 s
       #4  3501 MHz   14869934 s          4 s    1356464 s  816976741 s          4 s
       
  Memory: 31.383651733398438 GB (4242.078125 MB free)
  Uptime: 8.335763e6 sec
  Load Avg:  1.0029296875  1.28955078125  1.7431640625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.115
Commit b7dc60f (2018-07-02 03:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   21086139 s        259 s    3037347 s  807105827 s          6 s
       #2  3501 MHz  105230905 s          0 s    1664123 s  725983993 s          6 s
       #3  3501 MHz   15629905 s       2392 s    1742604 s  815647869 s         13 s
       #4  3501 MHz   14979173 s          4 s    1364519 s  817065491 s          4 s
       
  Memory: 31.383651733398438 GB (4184.16015625 MB free)
  Uptime: 8.33783e6 sec
  Load Avg:  0.9228515625  1.310546875  1.943359375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
