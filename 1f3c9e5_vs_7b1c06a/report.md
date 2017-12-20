# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1f3c9e5fd3415011983d5b554d871c92c6cbf78a](https://github.com/JuliaLang/julia/commit/1f3c9e5fd3415011983d5b554d871c92c6cbf78a) vs [JuliaLang/julia@7b1c06a23fb4d337e1dccda8657fd564b39e6fc9](https://github.com/JuliaLang/julia/commit/7b1c06a23fb4d337e1dccda8657fd564b39e6fc9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25197#issuecomment-353032149)

*Tag Predicate:* `"problem"`

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
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.62 (15%) :x: | 1.76 (1%) :x: |
| `["problem", "ziggurat", "ziggurat"]` | 2.34 (15%) :x: | 2.86 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

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

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3130
Commit 1f3c9e5 (2017-12-20 10:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100716625 s          0 s   15584382 s  4814075671 s        234 s
       #2  3501 MHz  396125379 s          0 s   16638971 s  4520133175 s         80 s
       #3  3501 MHz   81362230 s          0 s    9198168 s  4848993349 s        106 s
       #4  3501 MHz   76563283 s          0 s    9120287 s  4854273394 s         43 s
       
  Memory: 31.383651733398438 GB (5565.07421875 MB free)
  Uptime: 4.9415465e7 sec
  Load Avg:  1.00927734375  1.3212890625  1.66650390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3127
Commit 7b1c06a (2017-12-20 09:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100801159 s          0 s   15592552 s  4814161858 s        234 s
       #2  3501 MHz  396238989 s          0 s   16647287 s  4520190259 s         80 s
       #3  3501 MHz   81469779 s          0 s    9206261 s  4849056647 s        106 s
       #4  3501 MHz   76649760 s          0 s    9128182 s  4854358138 s         44 s
       
  Memory: 31.383651733398438 GB (5559.89453125 MB free)
  Uptime: 4.9417262e7 sec
  Load Avg:  1.0029296875  1.30712890625  1.890625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
