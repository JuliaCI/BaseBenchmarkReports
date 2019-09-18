# Benchmark Report

## Job Properties

*Commit(s):* [tpapp/julia@3579cf330302dedddbae7ff0a448153d11d9ae0e](https://github.com/tpapp/julia/commit/3579cf330302dedddbae7ff0a448153d11d9ae0e) vs [JuliaLang/julia@493c79703643f5579e033178bab7bd411b06b6b1](https://github.com/JuliaLang/julia/commit/493c79703643f5579e033178bab7bd411b06b6b1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33251#issuecomment-532762801)

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
| `["problem", "monte carlo", "euro_option_devec"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"Float64\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.176
Commit 3579cf3 (2019-09-18 15:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101093683 s       5044 s   11733814 s  4542296907 s         28 s
       #2  3501 MHz  696057434 s        208 s   12179400 s  3954176499 s         24 s
       #3  3501 MHz   84667426 s       3251 s    6983383 s  4570790956 s         33 s
       #4  3501 MHz   79420400 s         27 s    9913230 s  4571231860 s         22 s
       
  Memory: 31.383651733398438 GB (16673.34765625 MB free)
  Uptime: 4.6658556e7 sec
  Load Avg:  1.0029296875  1.05126953125  1.37109375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.171
Commit 493c797 (2019-09-18 15:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101203597 s       5044 s   11738671 s  4542423290 s         28 s
       #2  3501 MHz  696221665 s        208 s   12191042 s  3954242032 s         24 s
       #3  3501 MHz   84776175 s       3251 s    6988030 s  4570918835 s         33 s
       #4  3501 MHz   79519866 s         27 s    9917680 s  4571369295 s         22 s
       
  Memory: 31.383651733398438 GB (16365.31640625 MB free)
  Uptime: 4.6660973e7 sec
  Load Avg:  1.0029296875  1.056640625  1.470703125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
