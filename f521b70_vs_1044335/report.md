# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f521b701995406488f75cc418256c0fa2e291829](https://github.com/JuliaLang/julia/commit/f521b701995406488f75cc418256c0fa2e291829) vs [JuliaLang/julia@10443357f65438ec2cc935615eec3d3f7f189086](https://github.com/JuliaLang/julia/commit/10443357f65438ec2cc935615eec3d3f7f189086)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25029#issuecomment-352660341)

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
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"iterator\")"]` | 0.87 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\")"]` | 0.87 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\", \"sizehint!\")"]` | 2.80 (25%) :x: | 52.50 (1%) :x: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"iterator\")"]` | 0.86 (25%)  | 1.29 (1%) :x: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\")"]` | 0.89 (25%)  | 1.29 (1%) :x: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\", \"sizehint!\")"]` | 2.94 (25%) :x: | 52.50 (1%) :x: |
| `["collection", "optimizations", "(\"BitSet\", \"Int8\")"]` | 0.86 (25%)  | 0.91 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 0.74 (25%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"<\", \"BitSet\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 1.00 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 1.00 (25%)  | 1.25 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 1.00 (25%)  | 0.61 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"BitSet\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Set\")"]` | 0.90 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.89 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"big\")"]` | 204.23 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.89 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.91 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 0.92 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.92 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 204.09 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\")"]` | 0.89 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.91 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\")"]` | 1.00 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\")"]` | 0.90 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"self\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"empty\", \"Int\", \"<\", \"BitSet\")"]` | 1.00 (25%)  | 0.91 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"empty\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.00 (25%)  | 0.91 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.3105
Commit f521b70 (2017-12-19 07:19 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100200335 s          0 s   15525225 s  4804766945 s        232 s
       #2  3501 MHz  395239058 s          0 s   16570041 s  4511199780 s         80 s
       #3  3501 MHz   80812616 s          0 s    9148844 s  4839690525 s        105 s
       #4  3501 MHz   76023852 s          0 s    9066593 s  4844966704 s         42 s
       
  Memory: 31.383651733398438 GB (4105.9609375 MB free)
  Uptime: 4.9316391e7 sec
  Load Avg:  1.0029296875  1.13134765625  1.505859375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3095
Commit 1044335 (2017-12-19 01:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100285320 s          0 s   15533657 s  4804880492 s        233 s
       #2  3501 MHz  395375985 s          0 s   16578344 s  4511261763 s         80 s
       #3  3501 MHz   80923867 s          0 s    9156866 s  4839778566 s        105 s
       #4  3501 MHz   76111369 s          0 s    9074764 s  4845078391 s         43 s
       
  Memory: 31.383651733398438 GB (4067.703125 MB free)
  Uptime: 4.931847e7 sec
  Load Avg:  1.0029296875  1.12646484375  1.650390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
