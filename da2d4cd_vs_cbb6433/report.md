# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@da2d4cd78d62fb5cda4510aa2778678644292afe](https://github.com/JuliaLang/julia/commit/da2d4cd78d62fb5cda4510aa2778678644292afe) vs [JuliaLang/julia@cbb643366937a85579cb5291c7b835a8e22ce7cb](https://github.com/JuliaLang/julia/commit/cbb643366937a85579cb5291c7b835a8e22ce7cb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28259)

*Tag Predicate:* `"shootout" || ("string" || "problem")`

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
| `["shootout", "regex_dna"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["problem", "chaosgame"]`
- `["problem", "fem"]`
- `["problem", "go"]`
- `["problem", "grigoriadis khachiyan"]`
- `["problem", "imdb"]`
- `["problem", "json"]`
- `["problem", "laplacian"]`
- `["problem", "monte carlo"]`
- `["problem", "raytrace"]`
- `["problem", "seismic"]`
- `["problem", "simplex"]`
- `["problem", "spellcheck"]`
- `["problem", "stockcorr"]`
- `["problem", "ziggurat"]`
- `["shootout"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta2.93
Commit da2d4cd* (2018-07-24 12:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   45456141 s        284 s    4710239 s  973798608 s         12 s
       #2  3501 MHz  214778230 s          0 s    3125299 s  808444270 s          8 s
       #3  3501 MHz   31130315 s       2381 s    2552420 s  992285428 s         17 s
       #4  3501 MHz   28932404 s          0 s    2990156 s  994133038 s         10 s
       
  Memory: 31.383651733398438 GB (4367.49609375 MB free)
  Uptime: 1.027019e7 sec
  Load Avg:  0.93310546875  1.22412109375  1.70458984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta2.91
Commit cbb6433* (2018-07-24 04:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   45572268 s        284 s    4719441 s  973900284 s         12 s
       #2  3501 MHz  214930755 s          0 s    3133932 s  808510257 s          8 s
       #3  3501 MHz   31253182 s       2381 s    2561404 s  992380615 s         17 s
       #4  3501 MHz   29052854 s          0 s    2998983 s  994231074 s         10 s
       
  Memory: 31.383651733398438 GB (4278.6015625 MB free)
  Uptime: 1.0272468e7 sec
  Load Avg:  0.9970703125  1.1953125  1.81494140625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
