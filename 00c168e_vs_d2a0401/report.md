# Benchmark Report

## Job Properties

*Commit(s):* [jw3126/julia@00c168e16a39183d7c7c0994245b7bf280ed9916](https://github.com/jw3126/julia/commit/00c168e16a39183d7c7c0994245b7bf280ed9916) vs [JuliaLang/julia@d2a0401dfc9ea657fefe595f56e170213d927138](https://github.com/JuliaLang/julia/commit/d2a0401dfc9ea657fefe595f56e170213d927138)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18931#issuecomment-257590221)

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
Julia Version 0.6.0-dev.1175
Commit 00c168e (2016-11-01 09:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11961.9140625 MB free)
Uptime: 1.366175e7 sec
Load Avg:  0.9228515625  0.9599609375  0.9296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20857709 s          0 s    4608461 s  1336795734 s         42 s
#2  3501 MHz   60187007 s          0 s    2846380 s  1302293312 s          6 s
#3  3501 MHz   20176540 s          0 s    2507154 s  1342844063 s         29 s
#4  3501 MHz   17357093 s          0 s    2507640 s  1345654945 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1166
Commit d2a0401 (2016-11-01 09:40 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11941.5390625 MB free)
Uptime: 1.3665267e7 sec
Load Avg:  1.01416015625  0.974609375  0.9482421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20907761 s          0 s    4615486 s  1337089198 s         42 s
#2  3501 MHz   60260740 s          0 s    2851994 s  1302565155 s          6 s
#3  3501 MHz   20214762 s          0 s    2513707 s  1343150150 s         29 s
#4  3501 MHz   17516408 s          0 s    2518745 s  1345835718 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
