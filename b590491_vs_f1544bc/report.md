# Benchmark Report

## Job Properties

*Commit(s):* [jw3126/julia@b59049112448516fdc48bbca100c129bbeb71802](https://github.com/jw3126/julia/commit/b59049112448516fdc48bbca100c129bbeb71802) vs [JuliaLang/julia@f1544bc3a44e7a46f514a406658e3344aad8f207](https://github.com/JuliaLang/julia/commit/f1544bc3a44e7a46f514a406658e3344aad8f207)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18931#issuecomment-258622307)

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
Julia Version 0.6.0-dev.1194
Commit b590491 (2016-11-05 14:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12035.47265625 MB free)
Uptime: 1.4012246e7 sec
Load Avg:  1.2431640625  1.03515625  0.9443359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22571475 s          0 s    3757631 s  1371991566 s         45 s
#2  3501 MHz   60518118 s          0 s    4282104 s  1334352937 s         14 s
#3  3501 MHz   19405504 s          0 s    2496492 s  1378652305 s         22 s
#4  3501 MHz   16280654 s          0 s    2424766 s  1381970741 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1192
Commit f1544bc (2016-11-05 14:33 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12011.171875 MB free)
Uptime: 1.4015902e7 sec
Load Avg:  1.0029296875  0.9814453125  0.95068359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22697515 s          0 s    3766752 s  1372221150 s         45 s
#2  3501 MHz   60628230 s          0 s    4289436 s  1334600412 s         14 s
#3  3501 MHz   19465578 s          0 s    2504348 s  1378949245 s         22 s
#4  3501 MHz   16319378 s          0 s    2431132 s  1382290724 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
