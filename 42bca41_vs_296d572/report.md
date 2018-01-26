# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@42bca41f20465aeded9016aa3672fde8b248cb5a](https://github.com/JuliaLang/julia/commit/42bca41f20465aeded9016aa3672fde8b248cb5a) vs [JuliaLang/julia@296d5728a2974ac1e3efaf358288c40b05e3abee](https://github.com/JuliaLang/julia/commit/296d5728a2974ac1e3efaf358288c40b05e3abee)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25713#issuecomment-360646734)

*Tag Predicate:* `"string" && "readuntil"`

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

- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3582
Commit 42bca41 (2018-01-26 00:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  106131352 s          0 s   16339699 s  5123129999 s        263 s
       #2  3501 MHz  414538570 s          0 s   17478150 s  4816222627 s         84 s
       #3  3501 MHz   83829982 s          0 s    9509581 s  5162031492 s        113 s
       #4  3501 MHz   79023359 s          0 s    9417033 s  5167367239 s         47 s
       
  Memory: 31.383651733398438 GB (3760.80859375 MB free)
  Uptime: 5.2574585e7 sec
  Load Avg:  1.00537109375  1.43310546875  1.74267578125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3580
Commit 296d572 (2018-01-26 00:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  106221466 s          0 s   16347910 s  5123202729 s        263 s
       #2  3501 MHz  414641380 s          0 s   17486506 s  4816282595 s         84 s
       #3  3501 MHz   83918826 s          0 s    9518074 s  5162105218 s        114 s
       #4  3501 MHz   79127196 s          0 s    9425247 s  5167426384 s         47 s
       
  Memory: 31.383651733398438 GB (3751.06640625 MB free)
  Uptime: 5.2576303e7 sec
  Load Avg:  0.98486328125  1.396484375  1.9755859375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
