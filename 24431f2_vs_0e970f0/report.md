# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@24431f20387e5b5b53709e187cc54dcbbc1b20a9](https://github.com/JuliaLang/julia/commit/24431f20387e5b5b53709e187cc54dcbbc1b20a9) vs [JuliaLang/julia@0e970f05fc9fb16b46d285f8b3fc5ff88fe53b44](https://github.com/JuliaLang/julia/commit/0e970f05fc9fb16b46d285f8b3fc5ff88fe53b44)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20952#issuecomment-285808972)

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
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.22 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.125
Commit 24431f2 (2017-03-10 23:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4586.41796875 MB free)
Uptime: 2.4834297e7 sec
Load Avg:  0.93115234375  1.56298828125  1.79345703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52663975 s          0 s    8129498 s  2417336432 s         75 s
#2  3501 MHz  189844658 s          0 s    8696236 s  2280848373 s         26 s
#3  3501 MHz   43613841 s          0 s    5097400 s  2433594310 s         40 s
#4  3501 MHz   39397970 s          0 s    5035116 s  2438105439 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.116
Commit 0e970f0 (2017-03-10 19:40 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4480.26171875 MB free)
Uptime: 2.4835878e7 sec
Load Avg:  0.92529296875  1.56298828125  2.10693359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52746891 s          0 s    8137922 s  2417402606 s         75 s
#2  3501 MHz  189946030 s          0 s    8704691 s  2280896112 s         26 s
#3  3501 MHz   43710534 s          0 s    5105847 s  2433646641 s         40 s
#4  3501 MHz   39481724 s          0 s    5043827 s  2438170549 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
