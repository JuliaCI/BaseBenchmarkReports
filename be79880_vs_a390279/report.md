# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@be79880cd93dfcf1a8b28afae010b11e687c9215](https://github.com/JuliaLang/julia/commit/be79880cd93dfcf1a8b28afae010b11e687c9215) vs [JuliaLang/julia@a390279cfb8434be0a5cfcd90ceb69cb178a4884](https://github.com/JuliaLang/julia/commit/a390279cfb8434be0a5cfcd90ceb69cb178a4884)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30010#issuecomment-446461079)

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
Julia Version 1.0.3-pre.71
Commit be79880 (2018-12-07 21:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   66151694 s       5009 s    7292403 s  2163365929 s         22 s
       #2  3501 MHz  369252242 s        203 s    6010141 s  1865320044 s         18 s
       #3  3501 MHz   50099970 s       3216 s    4236672 s  2186177002 s         26 s
       #4  3501 MHz   46768748 s          0 s    5398352 s  2187887996 s         16 s
       
  Memory: 31.383651733398438 GB (5002.51953125 MB free)
  Uptime: 2.2424434e7 sec
  Load Avg:  1.0068359375  1.05859375  1.4365234375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.0.3-pre.2
Commit a390279 (2018-12-05 22:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   66276716 s       5009 s    7299451 s  2163496996 s         22 s
       #2  3501 MHz  369441051 s        203 s    6016878 s  1865388096 s         18 s
       #3  3501 MHz   50211923 s       3216 s    4243667 s  2186321328 s         26 s
       #4  3501 MHz   46877044 s          0 s    5405014 s  2188036543 s         16 s
       
  Memory: 31.383651733398438 GB (4932.484375 MB free)
  Uptime: 2.2427074e7 sec
  Load Avg:  1.0029296875  1.04443359375  1.46337890625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
