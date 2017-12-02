# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4a28387cc8572f2fe502945393ecde8d244c1cfd](https://github.com/JuliaLang/julia/commit/4a28387cc8572f2fe502945393ecde8d244c1cfd) vs [JuliaLang/julia@255b5d5c8ce0970258e4ce28c4239d62feabd842](https://github.com/JuliaLang/julia/commit/255b5d5c8ce0970258e4ce28c4239d62feabd842)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24885#issuecomment-348713623)

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
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 1.00 (25%)  | 0.44 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 1.00 (25%)  | 0.46 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.00 (25%)  | 0.44 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.89 (25%)  | 0.44 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.00 (25%)  | 0.90 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 1.00 (25%)  | 0.44 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967297)\")"]` | 1.00 (25%)  | 0.44 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"ImplicitRNG\", \"Int64\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float16\")"]` | 1.01 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int128\")"]` | 0.98 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int16\")"]` | 0.90 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int32\")"]` | 0.94 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int64\")"]` | 0.96 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int8\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt128\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt16\")"]` | 0.90 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt32\")"]` | 0.94 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt64\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt8\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.2730
Commit 4a28387 (2017-12-02 19:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96106495 s          0 s   14971418 s  4667441912 s        219 s
       #2  3501 MHz  382647484 s          0 s   16154290 s  4382045074 s         76 s
       #3  3501 MHz   78567586 s          0 s    8921176 s  4699851708 s         98 s
       #4  3501 MHz   73740587 s          0 s    8833435 s  4705165764 s         42 s
       
  Memory: 31.383651733398438 GB (1689.43359375 MB free)
  Uptime: 4.7892816e7 sec
  Load Avg:  1.2431640625  1.34375  2.1259765625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2728
Commit 255b5d5 (2017-12-02 18:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96210928 s          0 s   14979261 s  4667519547 s        220 s
       #2  3501 MHz  382771060 s          0 s   16163536 s  4382102307 s         76 s
       #3  3501 MHz   78654096 s          0 s    8928888 s  4699947527 s         99 s
       #4  3501 MHz   73824083 s          0 s    8841382 s  4705264525 s         42 s
       
  Memory: 31.383651733398438 GB (1734.16015625 MB free)
  Uptime: 4.7894724e7 sec
  Load Avg:  1.021484375  1.27197265625  1.9072265625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
