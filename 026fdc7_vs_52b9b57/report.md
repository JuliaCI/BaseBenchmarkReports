# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@026fdc7a8ca72bd7cc5ec8bf7121906e420a3e36](https://github.com/JuliaLang/julia/commit/026fdc7a8ca72bd7cc5ec8bf7121906e420a3e36) vs [JuliaLang/julia@52b9b574e41ee3605b5c2e5a07022654b3170940](https://github.com/JuliaLang/julia/commit/52b9b574e41ee3605b5c2e5a07022654b3170940)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22752#issuecomment-322425622)

*Tag Predicate:* `"random"`

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
| `["random","types",("rand","MersenneTwister","Int32")]` | 1.03 (25%)  | 1.07 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["problem","monte carlo"]`
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1355
Commit 026fdc7 (2017-08-15 09:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   85203706 s          0 s   15331600 s  3732055271 s         88 s
       #2  3501 MHz  354620112 s          0 s    9735012 s  3477241610 s         13 s
       #3  3501 MHz   74494728 s          0 s    8549611 s  3758942862 s         74 s
       #4  3501 MHz   71119602 s          0 s    8734826 s  3762126672 s         17 s
       
  Memory: 31.383651733398438 GB (3488.73828125 MB free)
  Uptime: 3.843834e7 sec
  Load Avg:  1.0029296875  1.12451171875  1.4521484375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1349
Commit 52b9b57 (2017-08-15 02:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   85282169 s          0 s   15338932 s  3732164103 s         88 s
       #2  3501 MHz  354755549 s          0 s    9745550 s  3477290639 s         13 s
       #3  3501 MHz   74575336 s          0 s    8556862 s  3759049845 s         74 s
       #4  3501 MHz   71209952 s          0 s    8741998 s  3762224141 s         17 s
       
  Memory: 31.383651733398438 GB (3390.28125 MB free)
  Uptime: 3.8440294e7 sec
  Load Avg:  0.9228515625  1.11572265625  1.62890625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
