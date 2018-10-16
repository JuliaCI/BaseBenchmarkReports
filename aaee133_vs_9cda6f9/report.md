# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@aaee13338b60758e465fa4c92ccfc5d3f1d6a8ec](https://github.com/JuliaLang/julia/commit/aaee13338b60758e465fa4c92ccfc5d3f1d6a8ec) vs [JuliaLang/julia@9cda6f99a1708c612f3346884240bf0ae4840f97](https://github.com/JuliaLang/julia/commit/9cda6f99a1708c612f3346884240bf0ae4840f97)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/29678#issuecomment-430405449)

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
| `["problem", "spellcheck", "spellcheck"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 0.61 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "replace"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["problem", "spellcheck"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-DEV.466
Commit aaee133 (2018-10-16 21:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   55349230 s       5002 s    6088518 s  1689860428 s         21 s
       #2  3501 MHz  283816764 s        203 s    4521735 s  1466013217 s         13 s
       #3  3501 MHz   39904200 s       3205 s    3444490 s  1711004662 s         24 s
       #4  3501 MHz   36978169 s          0 s    4272821 s  1712815258 s         13 s
       
  Memory: 31.383651733398438 GB (3807.27734375 MB free)
  Uptime: 1.7558707e7 sec
  Load Avg:  1.0029296875  1.25634765625  1.68896484375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.464
Commit 9cda6f9 (2018-10-16 15:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   55471613 s       5002 s    6095596 s  1689986338 s         21 s
       #2  3501 MHz  283969020 s        203 s    4529156 s  1466109169 s         13 s
       #3  3501 MHz   40019590 s       3205 s    3451796 s  1711137369 s         24 s
       #4  3501 MHz   37087917 s          0 s    4280074 s  1712953793 s         14 s
       
  Memory: 31.383651733398438 GB (3801.1640625 MB free)
  Uptime: 1.756127e7 sec
  Load Avg:  1.00341796875  1.30322265625  1.837890625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
