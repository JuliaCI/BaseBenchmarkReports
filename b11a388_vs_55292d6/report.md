# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b11a388d7a1ca4b3b865ddf0dd67afbdf34471ef](https://github.com/JuliaLang/julia/commit/b11a388d7a1ca4b3b865ddf0dd67afbdf34471ef) vs [JuliaLang/julia@55292d6146b4676c424bbd9adb87a3966cde783a](https://github.com/JuliaLang/julia/commit/55292d6146b4676c424bbd9adb87a3966cde783a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23612#issuecomment-328200967)

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
Julia Version 0.7.0-DEV.1732
Commit b11a388 (2017-09-08 19:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   91620688 s          0 s   16276214 s  3935113989 s         92 s
       #2  3501 MHz  387943372 s          0 s   10469793 s  3654128320 s         17 s
       #3  3501 MHz   79753582 s          0 s    9067399 s  3964121553 s         76 s
       #4  3501 MHz   76227427 s          0 s    9261871 s  3967455020 s         17 s
       
  Memory: 31.383651733398438 GB (3293.9453125 MB free)
  Uptime: 4.0548939e7 sec
  Load Avg:  0.9228515625  1.39794921875  1.6591796875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1729
Commit 55292d6 (2017-09-08 18:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   91701701 s          0 s   16283496 s  3935186265 s         92 s
       #2  3501 MHz  388061054 s          0 s   10477022 s  3654164119 s         17 s
       #3  3501 MHz   79832680 s          0 s    9074759 s  3964195556 s         76 s
       #4  3501 MHz   76304743 s          0 s    9268913 s  3967531339 s         17 s
       
  Memory: 31.383651733398438 GB (3241.3359375 MB free)
  Uptime: 4.055055e7 sec
  Load Avg:  1.0029296875  1.38134765625  1.92822265625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
