# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@09d3b2600506f30356d27e47f0efb7349c0389f5](https://github.com/JuliaLang/julia/commit/09d3b2600506f30356d27e47f0efb7349c0389f5) vs [JuliaLang/julia@6bdb3950bdf64152](https://github.com/JuliaLang/julia/commit/6bdb3950bdf64152)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/09d3b2600506f30356d27e47f0efb7349c0389f5#commitcomment-22176655)

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

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-rc1.78
Commit 09d3b26 (2017-05-17 06:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8295.1015625 MB free)
Uptime: 3.067998e7 sec
Load Avg:  0.9248046875  1.62451171875  1.84423828125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63566720 s          0 s    9833542 s  2988016888 s         89 s
#2  3501 MHz  247524351 s          0 s   10830745 s  2804018879 s         36 s
#3  3501 MHz   54491780 s          0 s    6348119 s  3005773653 s         46 s
#4  3501 MHz   50065975 s          0 s    6297025 s  3010532586 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-rc1.0
Commit 6bdb395 (2017-05-07 00:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8278.41015625 MB free)
Uptime: 3.0681567e7 sec
Load Avg:  0.94140625  1.6572265625  2.1884765625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63662633 s          0 s    9842346 s  2988070319 s         89 s
#2  3501 MHz  247625516 s          0 s   10839234 s  2804067447 s         36 s
#3  3501 MHz   54578835 s          0 s    6356696 s  3005836186 s         46 s
#4  3501 MHz   50152723 s          0 s    6305391 s  3010595678 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
