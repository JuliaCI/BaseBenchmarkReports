# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@7457905cc4c19670588c40a961814b861db0308f](https://github.com/musm/julia/commit/7457905cc4c19670588c40a961814b861db0308f) vs [JuliaLang/julia@ab0ac5e31d155d6bb8d987788659cb1ea50d8e62](https://github.com/JuliaLang/julia/commit/ab0ac5e31d155d6bb8d987788659cb1ea50d8e62)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23449#issuecomment-325159944)

*Tag Predicate:* `"linalg"`

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

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1522
Commit 7457905 (2017-08-26 19:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87965530 s          0 s   15763323 s  3827478812 s         90 s
       #2  3501 MHz  371544307 s          0 s   10117737 s  3558789716 s         15 s
       #3  3501 MHz   77318317 s          0 s    8824347 s  3854702832 s         75 s
       #4  3501 MHz   73886372 s          0 s    9011265 s  3857947241 s         17 s
       
  Memory: 31.383651733398438 GB (5126.9921875 MB free)
  Uptime: 3.9427469e7 sec
  Load Avg:  0.9228515625  1.078125  1.39990234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1518
Commit ab0ac5e (2017-08-26 19:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88046262 s          0 s   15770858 s  3827592632 s         90 s
       #2  3501 MHz  371690319 s          0 s   10124985 s  3558838892 s         15 s
       #3  3501 MHz   77393553 s          0 s    8831914 s  3854822214 s         75 s
       #4  3501 MHz   73981295 s          0 s    9018892 s  3858047161 s         17 s
       
  Memory: 31.383651733398438 GB (5073.484375 MB free)
  Uptime: 3.9429498e7 sec
  Load Avg:  1.00439453125  1.10693359375  1.58740234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
