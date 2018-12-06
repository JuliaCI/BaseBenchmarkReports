# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b222b5dae29311dc540df559ec62db644c7fb532](https://github.com/JuliaLang/julia/commit/b222b5dae29311dc540df559ec62db644c7fb532) vs [JuliaLang/julia@089420859e78ef13cd28bce9ffcfee8829553317](https://github.com/JuliaLang/julia/commit/089420859e78ef13cd28bce9ffcfee8829553317)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30289#issuecomment-444978717)

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
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |

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
- `["sparse", "transpose"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-DEV.826
Commit b222b5d (2018-12-06 17:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   65045946 s       5009 s    7164168 s  2117830045 s         22 s
       #2  3501 MHz  362446947 s        203 s    5868067 s  1825438664 s         18 s
       #3  3501 MHz   48993895 s       3214 s    4148808 s  2140534005 s         26 s
       #4  3501 MHz   45675119 s          0 s    5293482 s  2142254933 s         15 s
       
  Memory: 31.383651733398438 GB (4423.37109375 MB free)
  Uptime: 2.19557e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.19482421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.824
Commit 0894208 (2018-12-06 17:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   65172915 s       5009 s    7171730 s  2118027768 s         22 s
       #2  3501 MHz  362700533 s        203 s    5875757 s  1825510119 s         18 s
       #3  3501 MHz   49113418 s       3214 s    4156576 s  2140739440 s         26 s
       #4  3501 MHz   45792167 s          0 s    5300612 s  2142463527 s         15 s
       
  Memory: 31.383651733398438 GB (4190.65234375 MB free)
  Uptime: 2.1959034e7 sec
  Load Avg:  1.00927734375  1.01904296875  1.232421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
