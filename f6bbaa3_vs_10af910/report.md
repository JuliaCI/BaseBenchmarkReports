# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f6bbaa3db7b3bc5b7e8281d6a2a35ac3bbc37dad](https://github.com/JuliaLang/julia/commit/f6bbaa3db7b3bc5b7e8281d6a2a35ac3bbc37dad) vs [JuliaLang/julia@10af9107cf9c289b2239b2b8968826e28c76e390](https://github.com/JuliaLang/julia/commit/10af9107cf9c289b2239b2b8968826e28c76e390)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23612#issuecomment-327686675)

*Tag Predicate:* `"string"`

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
| `["dates","string","DateTime"]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 2.96 (15%) :x: | 2.28 (1%) :x: |
| `["string","replace"]` | 2.12 (15%) :x: | 13.70 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["problem","spellcheck"]`
- `["string"]`
- `["string","search"]`
- `["string","searchindex"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1683
Commit f6bbaa3 (2017-09-07 04:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   91039932 s          0 s   16213514 s  3921971277 s         92 s
       #2  3501 MHz  387037270 s          0 s   10435621 s  3641255307 s         17 s
       #3  3501 MHz   79497525 s          0 s    9041406 s  3950587423 s         75 s
       #4  3501 MHz   75995627 s          0 s    9231889 s  3953903459 s         17 s
       
  Memory: 31.383651733398438 GB (2908.51171875 MB free)
  Uptime: 4.0410715e7 sec
  Load Avg:  0.9228515625  1.4736328125  2.314453125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1681
Commit 10af910 (2017-09-07 02:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   91115797 s          0 s   16220762 s  3922044669 s         92 s
       #2  3501 MHz  387155712 s          0 s   10443057 s  3641286120 s         17 s
       #3  3501 MHz   79576095 s          0 s    9048987 s  3950657806 s         75 s
       #4  3501 MHz   76073726 s          0 s    9239022 s  3953974854 s         17 s
       
  Memory: 31.383651733398438 GB (2877.7734375 MB free)
  Uptime: 4.0412286e7 sec
  Load Avg:  1.005859375  1.49072265625  2.11865234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
