# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@70a38a8f038585f2932af3dc8a3e6625fd580fb5](https://github.com/JuliaLang/julia/commit/70a38a8f038585f2932af3dc8a3e6625fd580fb5) vs [JuliaLang/julia@6484f4cebfc38cc6dc6934dd6eb4d8b544c27e59](https://github.com/JuliaLang/julia/commit/6484f4cebfc38cc6dc6934dd6eb4d8b544c27e59)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269886323)

*Tag Predicate:* `"string"`

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
| `["dates","string","Date"]` | 0.56 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.68 (15%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["io","read","readstring"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.28 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.39 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["problem","spellcheck","spellcheck"]` | 0.65 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["string","replace"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["problem","spellcheck"]`
- `["string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1838
Commit 70a38a8 (2016-12-31 23:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3565.4921875 MB free)
Uptime: 1.8877081e7 sec
Load Avg:  0.9951171875  0.9033203125  0.880859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   32354959 s          0 s    5174647 s  1846356586 s         56 s
#2  3501 MHz   97328555 s          0 s    6204132 s  1781031971 s         20 s
#3  3501 MHz   27708311 s          0 s    3489950 s  1855639529 s         32 s
#4  3501 MHz   23593755 s          0 s    3393646 s  1860011147 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1833
Commit 6484f4c (2016-12-31 21:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3553.625 MB free)
Uptime: 1.8880657e7 sec
Load Avg:  0.90869140625  0.88525390625  0.892578125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   32476130 s          0 s    5183922 s  1846583106 s         56 s
#2  3501 MHz   97390368 s          0 s    6211831 s  1781319287 s         20 s
#3  3501 MHz   27786446 s          0 s    3498453 s  1855909807 s         32 s
#4  3501 MHz   23657482 s          0 s    3401210 s  1860296933 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
