# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d3f628bae9bf8f7928f1fd366d4aedbb6dccf86a](https://github.com/JuliaLang/julia/commit/d3f628bae9bf8f7928f1fd366d4aedbb6dccf86a) vs [JuliaLang/julia@2af5c86fbf8a6c03dbe177cbc3e6073c9f40784e](https://github.com/JuliaLang/julia/commit/2af5c86fbf8a6c03dbe177cbc3e6073c9f40784e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33079#issuecomment-524890638)

*Tag Predicate:* `"arithmetic"`

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
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 0.39 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 0.25 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 0.39 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 0.23 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 0.40 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 0.41 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 0.23 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 0.45 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.25 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 0.35 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 0.20 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 0.40 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 0.24 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 0.38 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 0.22 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 0.41 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 0.28 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 0.43 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.27 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 0.40 (45%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 0.22 (45%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"BigInt\")"]` | 1.64 (40%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates", "arithmetic"]`
- `["linalg", "arithmetic"]`
- `["scalar", "arithmetic"]`
- `["scalar", "fastmath"]`
- `["sparse", "arithmetic"]`

## Version Info

#### Primary Build

```
Julia Version 1.4.0-DEV.52
Commit d3f628b (2019-08-26 14:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   50741414 s       2440 s   13784683 s  4387726981 s         14 s
       #2  3501 MHz  304135071 s         36 s    5703792 s  4153575954 s         21 s
       #3  3501 MHz   41760804 s       3185 s    4967589 s  4416690211 s         34 s
       #4  3501 MHz   40301974 s         16 s    3792008 s  4421065867 s         30 s
       
  Memory: 31.383651733398438 GB (13633.50390625 MB free)
  Uptime: 4.4665746e7 sec
  Load Avg:  1.076171875  1.03076171875  1.181640625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.50
Commit 2af5c86 (2019-08-26 12:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   50839249 s       2440 s   13790028 s  4387936058 s         14 s
       #2  3501 MHz  304383691 s         36 s    5708797 s  4153635282 s         21 s
       #3  3501 MHz   41866800 s       3185 s    4972434 s  4416892280 s         34 s
       #4  3501 MHz   40408777 s         16 s    3796471 s  4421267617 s         30 s
       
  Memory: 31.383651733398438 GB (13434.56640625 MB free)
  Uptime: 4.4668879e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.2158203125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
