# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@634ee7e1049f8f821af39ff6e79c6d71af34642d](https://github.com/JuliaLang/julia/commit/634ee7e1049f8f821af39ff6e79c6d71af34642d) vs [JuliaLang/julia@2ecc4994566265582f4cc7c46ca18c2ea6a95522](https://github.com/JuliaLang/julia/commit/2ecc4994566265582f4cc7c46ca18c2ea6a95522)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30830#issuecomment-461550559)

*Tag Predicate:* `"dates"`

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
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`

## Version Info

#### Primary Build

```
Julia Version 1.2.0-DEV.294
Commit 634ee7e (2019-02-07 18:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   75329586 s       5015 s    8414150 s  2649443946 s         23 s
       #2  3501 MHz  442306644 s        203 s    7310373 s  2288113230 s         19 s
       #3  3501 MHz   58480150 s       3228 s    4934021 s  2674219435 s         27 s
       #4  3501 MHz   54772393 s          2 s    6429544 s  2675743902 s         17 s
       
  Memory: 31.383651733398438 GB (5030.82421875 MB free)
  Uptime: 2.7399034e7 sec
  Load Avg:  1.0029296875  1.32421875  1.7529296875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.2.0-DEV.291
Commit 2ecc499 (2019-02-07 17:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   75451309 s       5015 s    8421625 s  2649523573 s         23 s
       #2  3501 MHz  442432824 s        203 s    7317570 s  2288188870 s         19 s
       #3  3501 MHz   58603118 s       3228 s    4941027 s  2674298356 s         27 s
       #4  3501 MHz   54893103 s          2 s    6436865 s  2675825074 s         17 s
       
  Memory: 31.383651733398438 GB (4890.96484375 MB free)
  Uptime: 2.7401131e7 sec
  Load Avg:  1.0029296875  1.32958984375  1.93505859375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
