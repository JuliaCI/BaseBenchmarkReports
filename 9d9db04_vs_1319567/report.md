# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9d9db04d7e12bb5cc4384d542c05652a2c10e8bb](https://github.com/JuliaLang/julia/commit/9d9db04d7e12bb5cc4384d542c05652a2c10e8bb) vs [JuliaLang/julia@131956783faa5a3ee36eab3db084a9d840e95501](https://github.com/JuliaLang/julia/commit/131956783faa5a3ee36eab3db084a9d840e95501)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23528#issuecomment-352919435)

*Tag Predicate:* `"collection"`

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
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.89 (25%)  | 0.42 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 1.00 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.16 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 1.11 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.07 (25%) :white_check_mark: | 1.40 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\")"]` | 1.33 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.00 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.90 (25%)  | 0.64 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.08 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.85 (25%)  | 0.38 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.00 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.19 (25%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.90 (25%)  | 0.64 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.01 (25%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.01 (25%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.30 (25%) :white_check_mark: | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.26 (25%) :white_check_mark: | 1.04 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 0.20 (25%) :white_check_mark: | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.22 (25%) :white_check_mark: | 1.04 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 0.08 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.17 (25%) :white_check_mark: | 2.76 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"BitSet\")"]` | 0.08 (25%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Set\")"]` | 0.07 (25%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.06 (25%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\")"]` | 9.67 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.59 (25%) :white_check_mark: | 0.52 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.54 (25%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 0.54 (25%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.54 (25%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.54 (25%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.52 (25%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 10.37 (25%) :x: | 4.79 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\")"]` | 28.03 (25%) :x: | 51.73 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 28.33 (25%) :x: | 51.79 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\")"]` | 12.51 (25%) :x: | 51.73 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 12.47 (25%) :x: | 51.79 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\")"]` | 5.27 (25%) :x: | 53.66 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 5.96 (25%) :x: | 55.62 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"BitSet\")"]` | 1.13 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 1.08 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 1.10 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 158.29 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.38 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.40 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 0.37 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.40 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.29 (25%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.31 (25%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 0.52 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\")"]` | 0.51 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.56 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 0.54 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.51 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 0.53 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.55 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "optimizations"]`
- `["collection", "queries & updates"]`
- `["collection", "set operations"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3119
Commit 9d9db04 (2017-12-19 22:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100546378 s          0 s   15562459 s  4810225917 s        234 s
       #2  3501 MHz  395849524 s          0 s   16617893 s  4516384145 s         80 s
       #3  3501 MHz   81188836 s          0 s    9181573 s  4845133225 s        106 s
       #4  3501 MHz   76366539 s          0 s    9101227 s  4850440330 s         43 s
       
  Memory: 31.383651733398438 GB (5599.71484375 MB free)
  Uptime: 4.9374944e7 sec
  Load Avg:  0.943359375  1.10791015625  1.47265625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3115
Commit 1319567 (2017-12-19 22:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100631734 s          0 s   15570918 s  4810339733 s        234 s
       #2  3501 MHz  395995118 s          0 s   16625833 s  4516438589 s         80 s
       #3  3501 MHz   81276439 s          0 s    9189718 s  4845245219 s        106 s
       #4  3501 MHz   76470040 s          0 s    9109531 s  4850536412 s         43 s
       
  Memory: 31.383651733398438 GB (5544.3671875 MB free)
  Uptime: 4.9377029e7 sec
  Load Avg:  0.9228515625  1.11279296875  1.64306640625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
