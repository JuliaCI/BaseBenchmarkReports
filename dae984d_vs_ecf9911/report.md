# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@dae984d4f0d1c96f60d77b8fdbe3148f59b58157](https://github.com/JuliaLang/julia/commit/dae984d4f0d1c96f60d77b8fdbe3148f59b58157) vs [JuliaLang/julia@ecf9911d92cecf50c339eddea20fe525c5697cec](https://github.com/JuliaLang/julia/commit/ecf9911d92cecf50c339eddea20fe525c5697cec)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30607#issuecomment-452829815)

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

- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-rc1.11
Commit dae984d (2019-01-09 14:04 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   42244687 s       2424 s    7951689 s  2431765482 s         12 s
       #2  3501 MHz  235564544 s         14 s    4230513 s  2247868704 s         18 s
       #3  3501 MHz   33312978 s       3143 s    3840735 s  2450416005 s         26 s
       #4  3501 MHz   32033253 s         11 s    3008104 s  2453601963 s         22 s
       
  Memory: 31.383651733398438 GB (9848.26171875 MB free)
  Uptime: 2.4896807e7 sec
  Load Avg:  1.2431640625  1.08935546875  1.38232421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-rc1.1
Commit ecf9911 (2019-01-02 23:18 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   42365622 s       2424 s    7959175 s  2431907354 s         12 s
       #2  3501 MHz  235765589 s         14 s    4237188 s  2247931806 s         18 s
       #3  3501 MHz   33434920 s       3143 s    3847731 s  2450557672 s         26 s
       #4  3501 MHz   32141057 s         11 s    3014992 s  2453758112 s         22 s
       
  Memory: 31.383651733398438 GB (9818.18359375 MB free)
  Uptime: 2.489952e7 sec
  Load Avg:  0.9970703125  1.04052734375  1.4599609375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
