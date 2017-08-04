# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1ae115d3c4b072dd4034c88f56a13a1d1bac433d](https://github.com/JuliaLang/julia/commit/1ae115d3c4b072dd4034c88f56a13a1d1bac433d) vs [JuliaLang/julia@b6e229be132015c715291053c022ec0cbb8e6d67](https://github.com/JuliaLang/julia/commit/b6e229be132015c715291053c022ec0cbb8e6d67)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23035#issuecomment-320131832)

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
Julia Version 0.7.0-DEV.1234
Commit 1ae115d (2017-08-04 01:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77876440 s          0 s   12046685 s  3647672123 s        129 s
       #2  3501 MHz  306158712 s          0 s   12988416 s  3419948656 s         45 s
       #3  3501 MHz   65988042 s          0 s    7588040 s  3670579136 s         61 s
       #4  3501 MHz   61363647 s          0 s    7514627 s  3675627889 s         21 s
       
  Memory: 31.383651733398438 GB (4340.890625 MB free)
  Uptime: 3.745799e7 sec
  Load Avg:  0.9970703125  1.10693359375  1.47900390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1231
Commit b6e229b (2017-08-04 00:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77955534 s          0 s   12054356 s  3647790258 s        129 s
       #2  3501 MHz  306308974 s          0 s   12995668 s  3419996365 s         45 s
       #3  3501 MHz   66084084 s          0 s    7595366 s  3670680911 s         61 s
       #4  3501 MHz   61442365 s          0 s    7522208 s  3675746734 s         21 s
       
  Memory: 31.383651733398438 GB (4343.91796875 MB free)
  Uptime: 3.7460048e7 sec
  Load Avg:  1.01220703125  1.1083984375  1.583984375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
