# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@2a8335d6f8c9f55231bfa28cb1507f776593dbef](https://github.com/JuliaLang/julia/commit/2a8335d6f8c9f55231bfa28cb1507f776593dbef) vs [JuliaLang/julia@91625e08e416e840d39ffac280b51a31cd7462dc](https://github.com/JuliaLang/julia/commit/91625e08e416e840d39ffac280b51a31cd7462dc)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21552#issuecomment-297173075)

*Tag Predicate:* `"serialization"`

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

- `["io","serialization"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.331
Commit 2a8335d (2017-04-25 21:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3009.34765625 MB free)
Uptime: 2.8803796e7 sec
Load Avg:  1.03466796875  1.85009765625  1.89306640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   57048438 s          0 s   11036433 s  2803908144 s         77 s
#2  3501 MHz  231895275 s          0 s    6845576 s  2639958851 s         11 s
#3  3501 MHz   51166174 s          0 s    6079932 s  2821751852 s         59 s
#4  3501 MHz   48456034 s          0 s    6224334 s  2824322906 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.329
Commit 91625e0 (2017-04-25 21:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3110.25390625 MB free)
Uptime: 2.8805247e7 sec
Load Avg:  1.0029296875  1.830078125  2.2880859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   57140363 s          0 s   11044567 s  2803952541 s         77 s
#2  3501 MHz  231988316 s          0 s    6854268 s  2640001671 s         11 s
#3  3501 MHz   51249130 s          0 s    6088204 s  2821805071 s         59 s
#4  3501 MHz   48536709 s          0 s    6232772 s  2824378387 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
