# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9bd738800b0faa612d07cf9e228e0dd9c68f0f68](https://github.com/JuliaLang/julia/commit/9bd738800b0faa612d07cf9e228e0dd9c68f0f68) vs [JuliaLang/julia@c16c0cb597e2910bb43ae597ac2946f51f785928](https://github.com/JuliaLang/julia/commit/c16c0cb597e2910bb43ae597ac2946f51f785928)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25058#issuecomment-352877443)

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
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"RandomDevice\", \"Int\", \"1:1000\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["problem", "monte carlo"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3110
Commit 9bd7388 (2017-12-19 17:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100371740 s          0 s   15544950 s  4809301177 s        234 s
       #2  3501 MHz  395533338 s          0 s   16598566 s  4515602672 s         80 s
       #3  3501 MHz   81015136 s          0 s    9165297 s  4844205191 s        106 s
       #4  3501 MHz   76194938 s          0 s    9084720 s  4849509848 s         43 s
       
  Memory: 31.383651733398438 GB (5740.83203125 MB free)
  Uptime: 4.9363746e7 sec
  Load Avg:  1.0029296875  1.14306640625  1.51513671875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3108
Commit c16c0cb (2017-12-19 11:51 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100460060 s          0 s   15553475 s  4809405722 s        234 s
       #2  3501 MHz  395684756 s          0 s   16608279 s  4515643134 s         80 s
       #3  3501 MHz   81105191 s          0 s    9173187 s  4844308664 s        106 s
       #4  3501 MHz   76277991 s          0 s    9092726 s  4849620432 s         43 s
       
  Memory: 31.383651733398438 GB (5620.11328125 MB free)
  Uptime: 4.9365768e7 sec
  Load Avg:  0.9970703125  1.15380859375  1.70556640625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
