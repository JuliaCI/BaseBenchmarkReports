# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@438c880abf385eea6fa35684c2df874eae6cf67e](https://github.com/JuliaLang/julia/commit/438c880abf385eea6fa35684c2df874eae6cf67e) vs [JuliaLang/julia@131956783faa5a3ee36eab3db084a9d840e95501](https://github.com/JuliaLang/julia/commit/131956783faa5a3ee36eab3db084a9d840e95501)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25197#issuecomment-352915222)

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
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 1.67 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"RandomDevice\", \"Int\", \"1:1000\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3118
Commit 438c880 (2017-12-19 22:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109496010 s          0 s   19255256 s  4794232805 s        100 s
       #2  3501 MHz  462008662 s          0 s   12251176 s  4460256712 s         23 s
       #3  3501 MHz   91568668 s          0 s   10459984 s  4832977940 s         84 s
       #4  3501 MHz   87550722 s          0 s   10654070 s  4836792724 s         21 s
       
  Memory: 31.383651733398438 GB (1816.18359375 MB free)
  Uptime: 4.9373645e7 sec
  Load Avg:  1.0029296875  1.14453125  1.49755859375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3115
Commit 1319567 (2017-12-19 22:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109583029 s          0 s   19262638 s  4794336358 s        100 s
       #2  3501 MHz  462134482 s          0 s   12260354 s  4460319883 s         23 s
       #3  3501 MHz   91652647 s          0 s   10467618 s  4833084277 s         84 s
       #4  3501 MHz   87659049 s          0 s   10661444 s  4836875202 s         21 s
       
  Memory: 31.383651733398438 GB (1985.28515625 MB free)
  Uptime: 4.9375632e7 sec
  Load Avg:  0.9169921875  1.1279296875  1.66796875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
