# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@461c2687ecdc507325055f76b7557c00c0d23fc6](https://github.com/pkofod/julia/commit/461c2687ecdc507325055f76b7557c00c0d23fc6) vs [JuliaLang/julia@e7acea7c72c41c8283127ebadf8b81652b9ecf6e](https://github.com/JuliaLang/julia/commit/e7acea7c72c41c8283127ebadf8b81652b9ecf6e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24859#issuecomment-406709034)

*Tag Predicate:* `"scalar" && "exp2"`

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
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"one\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["scalar", "exp2"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta2.60
Commit 461c268 (2018-07-20 15:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   44731204 s        282 s    4625253 s  942588896 s         11 s
       #2  3501 MHz  211001486 s          0 s    3045016 s  780256421 s          8 s
       #3  3501 MHz   30354325 s       2381 s    2486294 s  961071286 s         16 s
       #4  3501 MHz   28233549 s          0 s    2900540 s  962883550 s          9 s
       
  Memory: 31.383651733398438 GB (9055.59765625 MB free)
  Uptime: 9.949374e6 sec
  Load Avg:  1.02392578125  1.35107421875  1.8125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta2.57
Commit e7acea7 (2018-07-20 13:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   44841540 s        282 s    4634318 s  942681107 s         11 s
       #2  3501 MHz  211143399 s          0 s    3054070 s  780317254 s          8 s
       #3  3501 MHz   30469864 s       2381 s    2495301 s  961158336 s         17 s
       #4  3501 MHz   28360398 s          0 s    2908858 s  962960024 s          9 s
       
  Memory: 31.383651733398438 GB (8990.9609375 MB free)
  Uptime: 9.951497e6 sec
  Load Avg:  1.0029296875  1.3798828125  2.02392578125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
