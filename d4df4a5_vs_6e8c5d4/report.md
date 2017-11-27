# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d4df4a5ed4a7926a2044cb570ea3979e01fc409b](https://github.com/JuliaLang/julia/commit/d4df4a5ed4a7926a2044cb570ea3979e01fc409b) vs [JuliaLang/julia@6e8c5d4cdfc8a8ce628c4bb06b130d2df1702a38](https://github.com/JuliaLang/julia/commit/6e8c5d4cdfc8a8ce628c4bb06b130d2df1702a38)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23964#issuecomment-347287279)

*Tag Predicate:* `"random" && ("types" && ("Complex{Int128}" || ("Complex{UInt128}" || "Complex{Float64}")))`

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
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 1.99 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["random", "types"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2673
Commit d4df4a5 (2017-11-27 18:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  104325080 s          0 s   18490364 s  4609075846 s         98 s
       #2  3501 MHz  445116320 s          0 s   11813912 s  4286033994 s         22 s
       #3  3501 MHz   88103428 s          0 s   10097930 s  4645236563 s         81 s
       #4  3501 MHz   84278724 s          0 s   10287159 s  4648861417 s         21 s
       
  Memory: 31.383651733398438 GB (5618.55859375 MB free)
  Uptime: 4.7457082e7 sec
  Load Avg:  1.0185546875  1.70751953125  1.87646484375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2671
Commit 6e8c5d4 (2017-11-27 18:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  104422944 s          0 s   18497925 s  4609132604 s         98 s
       #2  3501 MHz  445214025 s          0 s   11821829 s  4286090676 s         22 s
       #3  3501 MHz   88190455 s          0 s   10105512 s  4645304077 s         81 s
       #4  3501 MHz   84360214 s          0 s   10295009 s  4648934325 s         21 s
       
  Memory: 31.383651733398438 GB (5592.4375 MB free)
  Uptime: 4.7458711e7 sec
  Load Avg:  1.0078125  1.61279296875  2.1318359375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
