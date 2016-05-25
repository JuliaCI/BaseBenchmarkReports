# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@c7bab8980300cee091bd0ab99e231cd94b462ee0](https://github.com/pabloferz/julia/commit/c7bab8980300cee091bd0ab99e231cd94b462ee0) vs [JuliaLang/julia@2ce982d019a6e81f0858be3c6cdbd9e89c56bd48](https://github.com/JuliaLang/julia/commit/2ce982d019a6e81f0858be3c6cdbd9e89c56bd48)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16583#issuecomment-221643281)

*Tag Predicate:* `"sort"`

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

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["micro"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4322
Commit c7bab89 (2016-05-25 16:36 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16104.4921875 MB free)
Uptime: 1.727783e6 sec
Load Avg:  1.0419921875  1.0400390625  0.98681640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1126430 s          0 s     573088 s  170533037 s          3 s
#2  3501 MHz    1635163 s          0 s      78550 s  171039713 s          0 s
#3  3501 MHz     633599 s          0 s     180336 s  171867098 s          0 s
#4  3501 MHz     618309 s          0 s     103753 s  172009531 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4320
Commit 2ce982d (2016-05-25 16:34 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16085.19140625 MB free)
Uptime: 1.731119e6 sec
Load Avg:  0.9970703125  0.94091796875  0.91357421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1218832 s          0 s     581827 s  170764654 s          3 s
#2  3501 MHz    1717065 s          0 s      85384 s  171284175 s          0 s
#3  3501 MHz     682243 s          0 s     186444 s  172145190 s          0 s
#4  3501 MHz     699795 s          0 s     110394 s  172254493 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
