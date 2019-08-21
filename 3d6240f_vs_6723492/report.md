# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3d6240fa69713fc81e51af33d326804f8b778f1a](https://github.com/JuliaLang/julia/commit/3d6240fa69713fc81e51af33d326804f8b778f1a) vs [JuliaLang/julia@67234925efbac41f58249839ff03b4b9d36c1ec0](https://github.com/JuliaLang/julia/commit/67234925efbac41f58249839ff03b4b9d36c1ec0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33009#issuecomment-523473579)

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
| `["collection", "deletion", "(\"IdDict\", \"Int\", \"filter\")"]` | 0.67 (25%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"iterator\")"]` | 0.61 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\")"]` | 0.60 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.55 (25%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"Bool\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"Int8\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"UInt16\")"]` | 0.66 (25%) :white_check_mark: | 0.74 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"IdDict\", \"concrete\", \"Bool\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"IdDict\", \"concrete\", \"Int8\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"IdDict\", \"concrete\", \"UInt16\")"]` | 0.65 (25%) :white_check_mark: | 0.74 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"pop!\", \"specified\")"]` | 0.53 (25%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"push!\", \"new\")"]` | 0.43 (25%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"push!\", \"overwrite\")"]` | 0.42 (25%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"new\")"]` | 0.43 (25%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"overwrite\")"]` | 0.43 (25%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.26
Commit 3d6240f (2019-08-21 14:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   97571708 s       5041 s   11311522 s  4303955453 s         28 s
       #2  3501 MHz  658263809 s        208 s   11326329 s  3750237540 s         24 s
       #3  3501 MHz   81035754 s       3245 s    6719961 s  4332081614 s         32 s
       #4  3501 MHz   76014543 s         24 s    9485278 s  4332587416 s         22 s
       
  Memory: 31.383651733398438 GB (14506.04296875 MB free)
  Uptime: 4.4230883e7 sec
  Load Avg:  1.2431640625  1.1044921875  1.38134765625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.24
Commit 6723492 (2019-08-21 11:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   97680796 s       5041 s   11316382 s  4304087178 s         28 s
       #2  3501 MHz  658450268 s        208 s   11331230 s  3750292206 s         24 s
       #3  3501 MHz   81137734 s       3245 s    6724739 s  4332220731 s         32 s
       #4  3501 MHz   76111037 s         24 s    9489902 s  4332732210 s         22 s
       
  Memory: 31.383651733398438 GB (14407.703125 MB free)
  Uptime: 4.4233345e7 sec
  Load Avg:  0.9228515625  1.02685546875  1.43359375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
