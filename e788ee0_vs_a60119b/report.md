# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e788ee0fe403a4268eb3e3226338179f328ac691](https://github.com/JuliaLang/julia/commit/e788ee0fe403a4268eb3e3226338179f328ac691) vs [JuliaLang/julia@a60119b57f1e193e387cb44578a461bf96ac501b](https://github.com/JuliaLang/julia/commit/a60119b57f1e193e387cb44578a461bf96ac501b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27974)

*Tag Predicate:* `"string"`

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

- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["problem", "spellcheck"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.190
Commit e788ee0 (2018-07-06 21:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   40177195 s        278 s    4155660 s  827646118 s          8 s
       #2  3501 MHz  182529959 s          0 s    2603787 s  688995856 s          4 s
       #3  3501 MHz   25698096 s       2379 s    2113026 s  845917317 s         13 s
       #4  3501 MHz   23975400 s          0 s    2437804 s  847495813 s          8 s
       
  Memory: 31.383651733398438 GB (3960.85546875 MB free)
  Uptime: 8.746635e6 sec
  Load Avg:  0.923828125  1.24951171875  1.76416015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.188
Commit a60119b (2018-07-06 20:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   40298718 s        278 s    4163877 s  827730482 s          8 s
       #2  3501 MHz  182660789 s          0 s    2612040 s  689071110 s          4 s
       #3  3501 MHz   25809107 s       2379 s    2120924 s  846012679 s         14 s
       #4  3501 MHz   24099637 s          0 s    2446191 s  847577497 s          8 s
       
  Memory: 31.383651733398438 GB (3929.3046875 MB free)
  Uptime: 8.748784e6 sec
  Load Avg:  0.9228515625  1.23779296875  1.869140625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
