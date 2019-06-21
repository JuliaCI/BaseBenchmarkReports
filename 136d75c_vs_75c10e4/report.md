# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@136d75cc92afd331077732bbc47076333094e400](https://github.com/JuliaLang/julia/commit/136d75cc92afd331077732bbc47076333094e400) vs [JuliaLang/julia@75c10e435b2b9c947422ad38fa0b020595d3f747](https://github.com/JuliaLang/julia/commit/75c10e435b2b9c947422ad38fa0b020595d3f747)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/32381#issuecomment-504524722)

*Tag Predicate:* `"parse_json" || ("regex_dna" || "regex_dna")`

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

- `["problem", "json"]`
- `["shootout"]`

## Version Info

#### Primary Build

```
Julia Version 1.3.0-DEV.437
Commit 136d75c (2019-06-21 17:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   49454151 s       2436 s   12093906 s  3823567326 s         13 s
       #2  3501 MHz  294607233 s         26 s    5327020 s  3594649627 s         19 s
       #3  3501 MHz   40483576 s       3174 s    4854436 s  3849317667 s         31 s
       #4  3501 MHz   39049612 s         16 s    3666047 s  3853445996 s         28 s
       
  Memory: 31.383651733398438 GB (5269.828125 MB free)
  Uptime: 3.8974814e7 sec
  Load Avg:  0.98974609375  1.33251953125  1.6552734375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.3.0-DEV.435
Commit 75c10e4 (2019-06-21 17:18 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   49562796 s       2436 s   12098386 s  3823637048 s         13 s
       #2  3501 MHz  294722741 s         26 s    5331644 s  3594712434 s         19 s
       #3  3501 MHz   40589775 s       3174 s    4858994 s  3849389780 s         31 s
       #4  3501 MHz   39149656 s         16 s    3670658 s  3853524365 s         28 s
       
  Memory: 31.383651733398438 GB (5222.41796875 MB free)
  Uptime: 3.8976647e7 sec
  Load Avg:  0.9140625  1.3310546875  1.9169921875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
