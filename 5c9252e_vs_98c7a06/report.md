# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@5c9252eff16dc0e33ac2067cc2b18315c0b0db94](https://github.com/musm/julia/commit/5c9252eff16dc0e33ac2067cc2b18315c0b0db94) vs [JuliaLang/julia@98c7a06f1a90cd7ee17d280ccb0d871c497aa025](https://github.com/JuliaLang/julia/commit/98c7a06f1a90cd7ee17d280ccb0d871c497aa025)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23322#issuecomment-324514326)

*Tag Predicate:* `"BigFloat"`

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

- `["nullable","nullablearray"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","predicate"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1473
Commit 5c9252e (2017-08-24 01:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87172703 s          0 s   15654419 s  3804642005 s         90 s
       #2  3501 MHz  367985577 s          0 s   10023808 s  3538648686 s         15 s
       #3  3501 MHz   76498302 s          0 s    8745082 s  3831812194 s         75 s
       #4  3501 MHz   73096854 s          0 s    8937702 s  3835014112 s         17 s
       
  Memory: 31.383651733398438 GB (3395.6484375 MB free)
  Uptime: 3.9189388e7 sec
  Load Avg:  1.0029296875  1.28173828125  1.60791015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1470
Commit 98c7a06 (2017-08-24 00:59 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87252977 s          0 s   15661570 s  3804726086 s         90 s
       #2  3501 MHz  368101324 s          0 s   10031239 s  3538697231 s         15 s
       #3  3501 MHz   76573897 s          0 s    8752344 s  3831900960 s         75 s
       #4  3501 MHz   73191558 s          0 s    8945005 s  3835083823 s         17 s
       
  Memory: 31.383651733398438 GB (3362.51953125 MB free)
  Uptime: 3.9191109e7 sec
  Load Avg:  0.9970703125  1.27490234375  1.8310546875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
