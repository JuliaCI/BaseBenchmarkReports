# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@051468b24c79f014a60bff1d3ab96a1f78d73c84](https://github.com/JuliaLang/julia/commit/051468b24c79f014a60bff1d3ab96a1f78d73c84) vs [JuliaLang/julia@fcd031b50cf40769b68c27248f61061ed7aaa139](https://github.com/JuliaLang/julia/commit/fcd031b50cf40769b68c27248f61061ed7aaa139)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30289#issuecomment-445117516)

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
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (default), matrix rhs"]` | 0.13 (5%) :white_check_mark: | 1.14 (1%) :x: |
| `["sparse", "sparse solves", "least squares (default), vector rhs"]` | 0.22 (5%) :white_check_mark: | 1.15 (1%) :x: |
| `["sparse", "sparse solves", "least squares (qr), matrix rhs"]` | 0.13 (5%) :white_check_mark: | 1.14 (1%) :x: |
| `["sparse", "sparse solves", "least squares (qr), vector rhs"]` | 0.22 (5%) :white_check_mark: | 1.15 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["broadcast", "sparse"]`
- `["problem", "fem"]`
- `["problem", "laplacian"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "sparse matvec"]`
- `["sparse", "sparse solves"]`
- `["sparse", "transpose"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-DEV.832
Commit 051468b (2018-12-06 22:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   39501830 s       2415 s    7014062 s  2145790055 s         11 s
       #2  3501 MHz  213282077 s         14 s    3832426 s  1980129421 s         17 s
       #3  3501 MHz   30655075 s       3138 s    3589697 s  2162860000 s         26 s
       #4  3501 MHz   29447906 s         11 s    2772502 s  2165912516 s         21 s
       
  Memory: 31.383651733398438 GB (5126.7890625 MB free)
  Uptime: 2.1990765e7 sec
  Load Avg:  1.0693359375  1.04833984375  1.205078125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.830
Commit fcd031b (2018-12-06 21:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   39608694 s       2415 s    7021445 s  2146010463 s         11 s
       #2  3501 MHz  213553461 s         14 s    3839551 s  1980186334 s         17 s
       #3  3501 MHz   30775979 s       3138 s    3596900 s  2163067113 s         26 s
       #4  3501 MHz   29564203 s         11 s    2779272 s  2166124880 s         21 s
       
  Memory: 31.383651733398438 GB (4256.3515625 MB free)
  Uptime: 2.1994124e7 sec
  Load Avg:  1.01513671875  1.04931640625  1.255859375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
