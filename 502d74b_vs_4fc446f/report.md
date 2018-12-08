# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@502d74b5dcce78917f77151e53529bd5d057f199](https://github.com/JuliaLang/julia/commit/502d74b5dcce78917f77151e53529bd5d057f199) vs [JuliaLang/julia@4fc446f1790fe04e227ff96ab75a01d130e2d930](https://github.com/JuliaLang/julia/commit/4fc446f1790fe04e227ff96ab75a01d130e2d930)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30266#issuecomment-445361207)

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
Julia Version 1.1.0-DEV.842
Commit 502d74b (2018-12-07 20:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   65404083 s       5009 s    7198677 s  2126829849 s         22 s
       #2  3501 MHz  364105223 s        203 s    5905136 s  1833146025 s         18 s
       #3  3501 MHz   49372814 s       3214 s    4173303 s  2149540079 s         26 s
       #4  3501 MHz   46028080 s          0 s    5322715 s  2151277374 s         16 s
       
  Memory: 31.383651733398438 GB (5115.1328125 MB free)
  Uptime: 2.204984e7 sec
  Load Avg:  1.0029296875  1.0390625  1.37890625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.840
Commit 4fc446f (2018-12-07 20:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   65533317 s       5009 s    7206290 s  2126966109 s         22 s
       #2  3501 MHz  364307692 s        203 s    5912379 s  1833209791 s         18 s
       #3  3501 MHz   49488876 s       3214 s    4180521 s  2149690167 s         26 s
       #4  3501 MHz   46139167 s          0 s    5329884 s  2151432591 s         16 s
       
  Memory: 31.383651733398438 GB (5041.14453125 MB free)
  Uptime: 2.205258e7 sec
  Load Avg:  1.0029296875  1.04248046875  1.44873046875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
