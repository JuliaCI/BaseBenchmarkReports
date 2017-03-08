# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6477d13d281f024027ac2813ac74d63557958c48](https://github.com/JuliaLang/julia/commit/6477d13d281f024027ac2813ac74d63557958c48) vs [JuliaLang/julia@c29fc1ece97e5c7d1812dd115a0758396c7e2384](https://github.com/JuliaLang/julia/commit/c29fc1ece97e5c7d1812dd115a0758396c7e2384)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20933#issuecomment-285076073)

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
| `["dates","construction","DateTime"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.82
Commit 6477d13 (2017-03-08 13:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8820.57421875 MB free)
Uptime: 2.4635103e7 sec
Load Avg:  1.00927734375  1.57958984375  1.7568359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44296139 s          0 s    9021288 s  2403059356 s         71 s
#2  3501 MHz  172379060 s          0 s    5553519 s  2284136988 s         10 s
#3  3501 MHz   40057560 s          0 s    4847985 s  2417441469 s         51 s
#4  3501 MHz   37600903 s          0 s    4997509 s  2419737328 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.80
Commit c29fc1e (2017-03-08 13:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8759.54296875 MB free)
Uptime: 2.4636635e7 sec
Load Avg:  1.01123046875  1.70849609375  2.18701171875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44377384 s          0 s    9029769 s  2403122203 s         71 s
#2  3501 MHz  172475859 s          0 s    5561509 s  2284184924 s         10 s
#3  3501 MHz   40137416 s          0 s    4856349 s  2417505781 s         51 s
#4  3501 MHz   37696543 s          0 s    5005738 s  2419786189 s          9 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
