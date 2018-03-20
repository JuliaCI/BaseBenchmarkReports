# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@00d6f2e0b924bd4d20ab81a673e37abd93babdbe](https://github.com/JuliaLang/julia/commit/00d6f2e0b924bd4d20ab81a673e37abd93babdbe) vs [JuliaLang/julia@f0c09df61ebf3cf3d1a558693f23832b4087f8a1](https://github.com/JuliaLang/julia/commit/f0c09df61ebf3cf3d1a558693f23832b4087f8a1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26529#issuecomment-374535829)

*Tag Predicate:* `"random"`

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

- `["problem", "monte carlo"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.4644
Commit 00d6f2e (2018-03-20 09:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  112111145 s          0 s   17496901 s  5575703121 s        292 s
       #2  3501 MHz  457864943 s          0 s   18488919 s  5232659291 s         90 s
       #3  3501 MHz   88519182 s          0 s   10095646 s  5617928456 s        134 s
       #4  3501 MHz   83690689 s          0 s   10111789 s  5623127995 s         55 s
       
  Memory: 31.383651733398438 GB (4673.5859375 MB free)
  Uptime: 5.7187834e7 sec
  Load Avg:  0.9228515625  1.10205078125  1.47021484375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4642
Commit f0c09df (2018-03-20 09:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  112201032 s          0 s   17505310 s  5575829046 s        292 s
       #2  3501 MHz  458003098 s          0 s   18498681 s  5232735949 s         90 s
       #3  3501 MHz   88629478 s          0 s   10103881 s  5618034299 s        135 s
       #4  3501 MHz   83774188 s          0 s   10120099 s  5623260579 s         57 s
       
  Memory: 31.383651733398438 GB (6634.61328125 MB free)
  Uptime: 5.7190087e7 sec
  Load Avg:  0.9228515625  1.10205078125  1.6015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
