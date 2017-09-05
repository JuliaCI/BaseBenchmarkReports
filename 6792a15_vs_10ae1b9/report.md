# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6792a153ec19d9e22c8a7c9bfcf04d73fa2084c1](https://github.com/JuliaLang/julia/commit/6792a153ec19d9e22c8a7c9bfcf04d73fa2084c1) vs [JuliaLang/julia@10ae1b97ede620b62b2a3a1133bd02dcdb48576b](https://github.com/JuliaLang/julia/commit/10ae1b97ede620b62b2a3a1133bd02dcdb48576b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23582#issuecomment-327068733)

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
Julia Version 0.7.0-DEV.1646
Commit 6792a15 (2017-09-05 01:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84665381 s          0 s   12954610 s  3916881733 s        158 s
       #2  3501 MHz  342348595 s          0 s   14130277 s  3659724444 s         54 s
       #3  3501 MHz   71653276 s          0 s    8194608 s  3941742092 s         74 s
       #4  3501 MHz   66941344 s          0 s    8067068 s  3946988125 s         26 s
       
  Memory: 31.383651733398438 GB (2942.16015625 MB free)
  Uptime: 4.023369e7 sec
  Load Avg:  1.01123046875  1.47607421875  1.7255859375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1644
Commit 10ae1b9 (2017-09-05 01:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84742208 s          0 s   12962051 s  3916958630 s        158 s
       #2  3501 MHz  342449268 s          0 s   14137968 s  3659777461 s         54 s
       #3  3501 MHz   71735728 s          0 s    8202160 s  3941813361 s         75 s
       #4  3501 MHz   67039150 s          0 s    8074202 s  3947044554 s         26 s
       
  Memory: 31.383651733398438 GB (2930.92578125 MB free)
  Uptime: 4.0235309e7 sec
  Load Avg:  0.9228515625  1.4287109375  1.986328125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
