# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d9ecc6369b744c61562b8311033f930021b3e9ed](https://github.com/JuliaLang/julia/commit/d9ecc6369b744c61562b8311033f930021b3e9ed) vs [JuliaLang/julia@88c34fc51d962aaef973935942b2e073e2e2f398](https://github.com/JuliaLang/julia/commit/88c34fc51d962aaef973935942b2e073e2e2f398)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33690#issuecomment-546977902)

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
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"iterate second\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.382
Commit d9ecc63 (2019-10-28 14:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   53179440 s       2445 s   15373012 s  4926044732 s         16 s
       #2  3501 MHz  326957404 s         42 s    6318875 s  4674115837 s         23 s
       #3  3501 MHz   44255497 s       3196 s    5197730 s  4957811259 s         35 s
       #4  3501 MHz   42639278 s         16 s    4042902 s  4962550638 s         32 s
       
  Memory: 31.383651733398438 GB (14940.1640625 MB free)
  Uptime: 5.010797e7 sec
  Load Avg:  0.9970703125  1.05029296875  1.3759765625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.379
Commit 88c34fc (2019-10-28 14:08 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   53276592 s       2445 s   15378035 s  4926186753 s         16 s
       #2  3501 MHz  327141235 s         42 s    6323757 s  4674171795 s         23 s
       #3  3501 MHz   44366270 s       3196 s    5202257 s  4957940559 s         35 s
       #4  3501 MHz   42740973 s         16 s    4047271 s  4962689233 s         32 s
       
  Memory: 31.383651733398438 GB (14881.671875 MB free)
  Uptime: 5.0110419e7 sec
  Load Avg:  0.9169921875  1.02978515625  1.4462890625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
