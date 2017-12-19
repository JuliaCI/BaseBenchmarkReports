# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@554ec0d1c39d1212e2a7f5bc8692120f3a7f3e8e](https://github.com/JuliaLang/julia/commit/554ec0d1c39d1212e2a7f5bc8692120f3a7f3e8e) vs [JuliaLang/julia@c16c0cb597e2910bb43ae597ac2946f51f785928](https://github.com/JuliaLang/julia/commit/c16c0cb597e2910bb43ae597ac2946f51f785928)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25190#issuecomment-352816433)

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
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Bool\", \"RangeGenerator(true:true)\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float16\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3110
Commit 554ec0d (2017-12-19 16:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109242297 s          0 s   19228050 s  4792200056 s        100 s
       #2  3501 MHz  461660194 s          0 s   12224391 s  4458312851 s         23 s
       #3  3501 MHz   91295782 s          0 s   10435954 s  4830956310 s         84 s
       #4  3501 MHz   87254531 s          0 s   10630773 s  4834792986 s         21 s
       
  Memory: 31.383651733398438 GB (2674.86328125 MB free)
  Uptime: 4.9350432e7 sec
  Load Avg:  0.9970703125  1.15185546875  1.5234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3108
Commit c16c0cb (2017-12-19 11:51 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109326224 s          0 s   19236160 s  4792307427 s        100 s
       #2  3501 MHz  461796956 s          0 s   12233841 s  4458366285 s         23 s
       #3  3501 MHz   91378045 s          0 s   10443948 s  4831065518 s         84 s
       #4  3501 MHz   87359722 s          0 s   10638591 s  4834879589 s         21 s
       
  Memory: 31.383651733398438 GB (2514.08203125 MB free)
  Uptime: 4.9352433e7 sec
  Load Avg:  1.0029296875  1.1435546875  1.67822265625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
