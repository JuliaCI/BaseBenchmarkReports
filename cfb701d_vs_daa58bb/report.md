# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@cfb701d28ddf03ffb903dce2a931ffa99cbebf71](https://github.com/JuliaLang/julia/commit/cfb701d28ddf03ffb903dce2a931ffa99cbebf71) vs [JuliaLang/julia@daa58bb183799aac11f069e5b17a689e7fb8ec1b](https://github.com/JuliaLang/julia/commit/daa58bb183799aac11f069e5b17a689e7fb8ec1b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24578#issuecomment-343843349)

*Tag Predicate:* `"linalg"`

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
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 1024)"]` | 0.35 (45%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 256)"]` | 0.31 (45%) :white_check_mark: | 0.25 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2497
Commit cfb701d (2017-11-13 08:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100839229 s          0 s   18024961 s  4488614725 s         97 s
       #2  3501 MHz  440033902 s          0 s   11656234 s  4166572950 s         21 s
       #3  3501 MHz   87136078 s          0 s    9982271 s  4521591187 s         81 s
       #4  3501 MHz   83296106 s          0 s   10143358 s  4525282946 s         20 s
       
  Memory: 31.383651733398438 GB (14169.2109375 MB free)
  Uptime: 4.6209416e7 sec
  Load Avg:  1.0029296875  1.10693359375  1.46240234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2495
Commit daa58bb (2017-11-13 04:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100923585 s          0 s   18032751 s  4488734067 s         97 s
       #2  3501 MHz  440183550 s          0 s   11663711 s  4166627689 s         21 s
       #3  3501 MHz   87221979 s          0 s    9989776 s  4521709515 s         81 s
       #4  3501 MHz   83393665 s          0 s   10150950 s  4525389654 s         20 s
       
  Memory: 31.383651733398438 GB (13997.94921875 MB free)
  Uptime: 4.6211539e7 sec
  Load Avg:  1.0029296875  1.10693359375  1.6044921875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
