# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d579c15512f31182634121bb5bd1234fa9a3b679](https://github.com/JuliaLang/julia/commit/d579c15512f31182634121bb5bd1234fa9a3b679) vs [JuliaLang/julia@4d062a514a178f54fccc6c81aec3fcfb7dbd501f](https://github.com/JuliaLang/julia/commit/4d062a514a178f54fccc6c81aec3fcfb7dbd501f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/35235#issuecomment-646381368)

*Tag Predicate:* `"random"`

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
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small String\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 1.54 (25%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["problem", "monte carlo"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 1.6.0-DEV.265
Commit d579c15 (2020-06-19 01:11 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  145777753 s       5056 s   16460265 s  6858445668 s         35 s
       #2  3501 MHz  1099984463 s        217 s   21947980 s  5908958961 s         27 s
       #3  3501 MHz  130726842 s       3312 s    9787402 s  6890126262 s         38 s
       #4  3501 MHz  122747570 s         43 s   14068884 s  6891899941 s         28 s
       
  Memory: 31.383651733398438 GB (19874.42578125 MB free)
  Uptime: 7.0364794e7 sec
  Load Avg:  1.00390625  1.0517578125  1.44677734375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.6.0-DEV.263
Commit 4d062a5 (2020-06-18 19:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  145919950 s       5056 s   16466774 s  6858607711 s         36 s
       #2  3501 MHz  1100204148 s        217 s   21961319 s  5909037190 s         27 s
       #3  3501 MHz  130881384 s       3312 s    9793589 s  6890276389 s         38 s
       #4  3501 MHz  122904435 s         43 s   14075083 s  6892048133 s         28 s
       
  Memory: 31.383651733398438 GB (19829.00390625 MB free)
  Uptime: 7.036791e7 sec
  Load Avg:  1.0029296875  1.0498046875  1.48779296875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
