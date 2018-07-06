# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ec080d4ecefeb0fe6791d6311c411486d6de2472](https://github.com/JuliaLang/julia/commit/ec080d4ecefeb0fe6791d6311c411486d6de2472) vs [JuliaLang/julia@feaee9ebbc22b04d1fe9a4fbe74e36c317b71046](https://github.com/JuliaLang/julia/commit/feaee9ebbc22b04d1fe9a4fbe74e36c317b71046)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27857#issuecomment-403086184)

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
Julia Version 0.7.0-beta.189
Commit ec080d4 (2018-07-06 17:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   39941221 s        278 s    4139102 s  827381868 s          8 s
       #2  3501 MHz  182256935 s          0 s    2587461 s  688767374 s          4 s
       #3  3501 MHz   25473553 s       2379 s    2095832 s  845641642 s         13 s
       #4  3501 MHz   23744601 s          0 s    2421659 s  847225121 s          8 s
       
  Memory: 31.383651733398438 GB (5168.78515625 MB free)
  Uptime: 8.741446e6 sec
  Load Avg:  1.0029296875  1.31005859375  1.85498046875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.182
Commit feaee9e (2018-07-06 12:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   40070355 s        278 s    4147476 s  827452188 s          8 s
       #2  3501 MHz  182392369 s          0 s    2595493 s  688832048 s          4 s
       #3  3501 MHz   25580084 s       2379 s    2104280 s  845734578 s         13 s
       #4  3501 MHz   23853022 s          0 s    2429664 s  847316817 s          8 s
       
  Memory: 31.383651733398438 GB (3991.65625 MB free)
  Uptime: 8.743533e6 sec
  Load Avg:  1.00439453125  1.310546875  1.93994140625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
