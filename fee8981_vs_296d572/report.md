# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fee8981d0c540209ca60ae02be45d06150a04634](https://github.com/JuliaLang/julia/commit/fee8981d0c540209ca60ae02be45d06150a04634) vs [JuliaLang/julia@296d5728a2974ac1e3efaf358288c40b05e3abee](https://github.com/JuliaLang/julia/commit/296d5728a2974ac1e3efaf358288c40b05e3abee)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25756#issuecomment-360821992)

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
| `["string", "readuntil", "backtracking"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 0.33 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 2"]` | 0.58 (15%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 50000"]` | 0.34 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3584
Commit fee8981 (2018-01-26 02:08 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  115607640 s          0 s   20358439 s  5111685076 s        101 s
       #2  3501 MHz  495573318 s          0 s   12785709 s  4751655058 s         25 s
       #3  3501 MHz   95417080 s          0 s   10899225 s  5154212188 s         85 s
       #4  3501 MHz   91279480 s          0 s   11085191 s  5158160885 s         22 s
       
  Memory: 31.383651733398438 GB (4561.6015625 MB free)
  Uptime: 5.2630127e7 sec
  Load Avg:  0.923828125  1.42578125  1.7216796875
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
       #1  3501 MHz  115717998 s          0 s   20366091 s  5111734629 s        101 s
       #2  3501 MHz  495673955 s          0 s   12793695 s  4751713961 s         25 s
       #3  3501 MHz   95502342 s          0 s   10907254 s  5154286346 s         85 s
       #4  3501 MHz   91360794 s          0 s   11093084 s  5158239263 s         22 s
       
  Memory: 31.383651733398438 GB (4504.5703125 MB free)
  Uptime: 5.2631808e7 sec
  Load Avg:  0.9228515625  1.43505859375  2.02197265625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
