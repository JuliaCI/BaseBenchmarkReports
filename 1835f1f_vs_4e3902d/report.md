# Benchmark Report

## Job Properties

*Commit(s):* [oxinabox/julia@1835f1f14ddc7109cc1fbbed25c72a226f337fa3](https://github.com/oxinabox/julia/commit/1835f1f14ddc7109cc1fbbed25c72a226f337fa3) vs [JuliaLang/julia@4e3902d6240d08bbd07032ccf99d2992239a6f8f](https://github.com/JuliaLang/julia/commit/4e3902d6240d08bbd07032ccf99d2992239a6f8f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27790#issuecomment-400238046)

*Tag Predicate:* `"string" || ("shootout" || "problem")`

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
Julia Version 0.7.0-beta.20
Commit 1835f1f (2018-06-26 09:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   17695150 s        259 s    2732700 s  761084626 s          5 s
       #2  3501 MHz   90430986 s          0 s    1429020 s  691257012 s          5 s
       #3  3501 MHz   13057634 s       2389 s    1532411 s  768634773 s         11 s
       #4  3501 MHz   12622556 s          4 s    1170156 s  769803085 s          4 s
       
  Memory: 31.383651733398438 GB (4256.65625 MB free)
  Uptime: 7.839372e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.1015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.18
Commit 4e3902d (2018-06-26 06:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   17808151 s        259 s    2742873 s  761379548 s          5 s
       #2  3501 MHz   90783425 s          0 s    1437658 s  691315124 s          5 s
       #3  3501 MHz   13192160 s       2389 s    1540998 s  768910753 s         11 s
       #4  3501 MHz   12728437 s          4 s    1178607 s  770107866 s          4 s
       
  Memory: 31.383651733398438 GB (4218.18359375 MB free)
  Uptime: 7.843571e6 sec
  Load Avg:  0.93798828125  1.005859375  1.109375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
