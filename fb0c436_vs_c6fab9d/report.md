# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fb0c43646ed8bfe016644c062d4668b6a24a5396](https://github.com/JuliaLang/julia/commit/fb0c43646ed8bfe016644c062d4668b6a24a5396) vs [JuliaLang/julia@c6fab9ddbc70a5550ad727bdbccbc663ffb32c99](https://github.com/JuliaLang/julia/commit/c6fab9ddbc70a5550ad727bdbccbc663ffb32c99)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17613#issuecomment-235018513)

*Tag Predicate:* `"simd"`

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
| `["simd",("conditional_loop!","Int32",4095)]` | 0.00 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 0.00 (20%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","index"]`
- `["problem","seismic"]`
- `["simd"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-pre+5678
Commit fb0c436 (2016-07-25 17:05 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18320.18359375 MB free)
Uptime: 5.115583e6 sec
Load Avg:  1.0078125  0.9619140625  0.892578125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6901561 s          0 s    1565750 s  501708155 s         18 s
#2  3501 MHz   18882874 s          0 s     957186 s  491424004 s          2 s
#3  3501 MHz    7002256 s          0 s     887858 s  503423940 s          9 s
#4  3501 MHz    5845385 s          0 s     876512 s  504578038 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-pre+5676
Commit c6fab9d (2016-07-25 16:51 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18271.03125 MB free)
Uptime: 5.119062e6 sec
Load Avg:  0.9970703125  0.97119140625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    6932121 s          0 s    1571412 s  502018786 s         18 s
#2  3501 MHz   19076444 s          0 s     969510 s  491565743 s          2 s
#3  3501 MHz    7059831 s          0 s     894098 s  503707372 s          9 s
#4  3501 MHz    5881336 s          0 s     882296 s  504883645 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
