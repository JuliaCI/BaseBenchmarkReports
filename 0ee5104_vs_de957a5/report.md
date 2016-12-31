# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0ee510449ded51f68fa86f809465552e3b8e994c](https://github.com/JuliaLang/julia/commit/0ee510449ded51f68fa86f809465552e3b8e994c) vs [JuliaLang/julia@de957a5d7e5bb3a17a2e6576676e15bc1bb3c126](https://github.com/JuliaLang/julia/commit/de957a5d7e5bb3a17a2e6576676e15bc1bb3c126)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269880649)

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
| `["dates","string","Date"]` | 0.54 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.67 (15%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.28 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.41 (15%) :white_check_mark: | 1.11 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 0.60 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["string","join"]` | 0.85 (40%)  | 1.98 (1%) :x: |
| `["string","replace"]` | 0.79 (15%) :white_check_mark: | 1.81 (1%) :x: |

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
Julia Version 0.6.0-dev.1837
Commit 0ee5104 (2016-12-31 19:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3689.1015625 MB free)
Uptime: 1.8865019e7 sec
Load Avg:  1.0263671875  0.9853515625  0.962890625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   32150805 s          0 s    5155106 s  1845376740 s         55 s
#2  3501 MHz   97112328 s          0 s    6185136 s  1780062986 s         20 s
#3  3501 MHz   27585214 s          0 s    3473781 s  1854574711 s         32 s
#4  3501 MHz   23491609 s          0 s    3380607 s  1858921458 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1832
Commit de957a5 (2016-12-31 19:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3469.45703125 MB free)
Uptime: 1.8868576e7 sec
Load Avg:  1.0078125  0.9306640625  0.9248046875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   32199487 s          0 s    5161892 s  1845676027 s         55 s
#2  3501 MHz   97248146 s          0 s    6195390 s  1780271993 s         20 s
#3  3501 MHz   27661234 s          0 s    3482442 s  1854844799 s         32 s
#4  3501 MHz   23553787 s          0 s    3387872 s  1859207002 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
