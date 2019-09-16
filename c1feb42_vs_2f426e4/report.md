# Benchmark Report

## Job Properties

*Commit(s):* [tpapp/julia@c1feb42c688f32afeafcc272f4086bb21cdee8e1](https://github.com/tpapp/julia/commit/c1feb42c688f32afeafcc272f4086bb21cdee8e1) vs [JuliaLang/julia@2f426e45c24e0d94c11f503aa696a902f1bb6aed](https://github.com/JuliaLang/julia/commit/2f426e45c24e0d94c11f503aa696a902f1bb6aed)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33251#issuecomment-531761492)

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
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"Float64\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.152
Commit c1feb42 (2019-09-16 12:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   51812844 s       2440 s   14336636 s  4566148037 s         15 s
       #2  3501 MHz  314272126 s         36 s    5937126 s  4323713640 s         21 s
       #3  3501 MHz   42824408 s       3192 s    5083572 s  4596045257 s         34 s
       #4  3501 MHz   41312960 s         16 s    3861430 s  4600595751 s         30 s
       
  Memory: 31.383651733398438 GB (14640.65625 MB free)
  Uptime: 4.6472213e7 sec
  Load Avg:  0.9228515625  1.0380859375  1.36767578125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.148
Commit 2f426e4 (2019-09-16 12:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   51910073 s       2440 s   14341543 s  4566286792 s         15 s
       #2  3501 MHz  314433475 s         36 s    5948784 s  4323782057 s         21 s
       #3  3501 MHz   42944882 s       3192 s    5088330 s  4596161260 s         34 s
       #4  3501 MHz   41414850 s         16 s    3865959 s  4600730736 s         30 s
       
  Memory: 31.383651733398438 GB (14565.609375 MB free)
  Uptime: 4.647463e7 sec
  Load Avg:  1.0029296875  1.05615234375  1.46728515625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
