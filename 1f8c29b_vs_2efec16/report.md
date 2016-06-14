# Benchmark Report

## Job Properties

*Commit(s):* [Sacha0/julia@1f8c29bd7e17757c6ddef3bfdb7727d73017a31c](https://github.com/Sacha0/julia/commit/1f8c29bd7e17757c6ddef3bfdb7727d73017a31c) vs [JuliaLang/julia@2efec16bd0fa22453b47d2d3be5040f7f5c5707d](https://github.com/JuliaLang/julia/commit/2efec16bd0fa22453b47d2d3be5040f7f5c5707d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16931#issuecomment-226014748)

*Tag Predicate:* `"sparse"`

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
| `["sparse","index",("spmat","splogical",100)]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.00 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.01 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 1.00 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 0.99 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 1.01 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.00 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(600,400))]` | 1.02 (15%)  | Inf (1%) :x: |
| `["sparse","transpose",("transpose!",(600,600))]` | 1.01 (15%)  | Inf (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["problem","fem"]`
- `["problem","laplacian"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4770
Commit 1f8c29b (2016-06-14 19:22 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27469.89453125 MB free)
Uptime: 1.586532e6 sec
Load Avg:  0.98046875  0.93359375  0.8857421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1516627 s          0 s     408224 s  156323232 s          4 s
#2  3501 MHz    4598547 s          0 s     272197 s  153686224 s          1 s
#3  3501 MHz    2112250 s          0 s     280112 s  156172122 s          1 s
#4  3501 MHz    1775146 s          0 s     256952 s  156538675 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4767
Commit 2efec16 (2016-06-14 17:10 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27462.140625 MB free)
Uptime: 1.589762e6 sec
Load Avg:  0.9970703125  0.96826171875  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1560138 s          0 s     414594 s  156595598 s          4 s
#2  3501 MHz    4769148 s          0 s     282587 s  153827947 s          1 s
#3  3501 MHz    2155271 s          0 s     285562 s  156445864 s          1 s
#4  3501 MHz    1812659 s          0 s     263001 s  156817540 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
