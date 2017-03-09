# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4a225ae364df77e8b37fc61f50d14ccd0a3583f8](https://github.com/JuliaLang/julia/commit/4a225ae364df77e8b37fc61f50d14ccd0a3583f8) vs [JuliaLang/julia@e59606376ea71508fd93a830b1207645509b5d34](https://github.com/JuliaLang/julia/commit/e59606376ea71508fd93a830b1207645509b5d34)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20952#issuecomment-285182787)

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
| `["dates","parse","Date"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.98
Commit 4a225ae (2017-03-08 21:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8828.890625 MB free)
Uptime: 2.4657671e7 sec
Load Avg:  0.98828125  1.53759765625  1.75830078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44622068 s          0 s    9059110 s  2404943804 s         71 s
#2  3501 MHz  173648799 s          0 s    5587193 s  2285087875 s         10 s
#3  3501 MHz   40381352 s          0 s    4881704 s  2419337785 s         51 s
#4  3501 MHz   37965442 s          0 s    5030661 s  2421594332 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.94
Commit e596063 (2017-03-08 21:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8726.44921875 MB free)
Uptime: 2.4659221e7 sec
Load Avg:  1.01025390625  1.59619140625  2.10595703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44716198 s          0 s    9067590 s  2404995608 s         71 s
#2  3501 MHz  173747260 s          0 s    5595571 s  2285135609 s         10 s
#3  3501 MHz   40463251 s          0 s    4890308 s  2419401585 s         51 s
#4  3501 MHz   38048394 s          0 s    5038508 s  2421658050 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
