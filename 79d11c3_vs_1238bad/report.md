# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@79d11c3d836d1ca64f4f09e228f2aecbe08bb0c3](https://github.com/JuliaLang/julia/commit/79d11c3d836d1ca64f4f09e228f2aecbe08bb0c3) vs [JuliaLang/julia@1238bad60fc7d3b5984fbf25423d60159147462c](https://github.com/JuliaLang/julia/commit/1238bad60fc7d3b5984fbf25423d60159147462c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25277#issuecomment-354293140)

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
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3201
Commit 79d11c3 (2017-12-27 22:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101254007 s          0 s   15682870 s  4883572651 s        239 s
       #2  3501 MHz  399436500 s          0 s   16861996 s  4586720421 s         81 s
       #3  3501 MHz   81925929 s          0 s    9253559 s  4918627547 s        108 s
       #4  3501 MHz   77101551 s          0 s    9193953 s  4923902669 s         45 s
       
  Memory: 31.383651733398438 GB (3161.46484375 MB free)
  Uptime: 5.0118126e7 sec
  Load Avg:  1.0029296875  1.15673828125  1.53515625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3199
Commit 1238bad (2017-12-27 20:40 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101342581 s          0 s   15690993 s  4883679557 s        239 s
       #2  3501 MHz  399592416 s          0 s   16871706 s  4586758559 s         81 s
       #3  3501 MHz   82010566 s          0 s    9261658 s  4918738526 s        108 s
       #4  3501 MHz   77187354 s          0 s    9202058 s  4924012495 s         45 s
       
  Memory: 31.383651733398438 GB (4615.59375 MB free)
  Uptime: 5.012017e7 sec
  Load Avg:  1.0029296875  1.14794921875  1.68115234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
