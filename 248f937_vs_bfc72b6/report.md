# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@248f9376393a23cee811dfb6e63931ca08cb1e12](https://github.com/JuliaLang/julia/commit/248f9376393a23cee811dfb6e63931ca08cb1e12) vs [JuliaLang/julia@bfc72b6fe913236ccb2bdd1ef254bceccb0cc31a](https://github.com/JuliaLang/julia/commit/bfc72b6fe913236ccb2bdd1ef254bceccb0cc31a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19545#issuecomment-267093623)

*Tag Predicate:* `"dates"`

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
| `["dates","parse","Date"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.44 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.38 (15%) :white_check_mark: | 0.48 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 1.63 (15%) :x: | 1.50 (1%) :x: |
| `["dates","string","DateTime"]` | 2.27 (15%) :x: | 1.62 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1567
Commit 248f937 (2016-12-14 10:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10612.921875 MB free)
Uptime: 1.7384306e7 sec
Load Avg:  0.9833984375  0.9375  0.91357421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26739758 s          0 s    4455206 s  1703716518 s         53 s
#2  3501 MHz   76691337 s          0 s    5429428 s  1653431905 s         20 s
#3  3501 MHz   23496290 s          0 s    2992650 s  1711153674 s         28 s
#4  3501 MHz   19423450 s          0 s    2898170 s  1715459185 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1563
Commit bfc72b6 (2016-12-14 10:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10662.515625 MB free)
Uptime: 1.7387559e7 sec
Load Avg:  0.9970703125  0.912109375  0.88916015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26807428 s          0 s    4462544 s  1703966031 s         53 s
#2  3501 MHz   76821753 s          0 s    5439173 s  1653616686 s         20 s
#3  3501 MHz   23563429 s          0 s    3000540 s  1711403197 s         28 s
#4  3501 MHz   19453096 s          0 s    2903649 s  1715748714 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
