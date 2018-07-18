# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3984d54b37cf7e67ad9632a6cca785846775c286](https://github.com/JuliaLang/julia/commit/3984d54b37cf7e67ad9632a6cca785846775c286) vs [JuliaLang/julia@5369849a859d134ea3039eb5fa5b45d7e9993882](https://github.com/JuliaLang/julia/commit/5369849a859d134ea3039eb5fa5b45d7e9993882)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28027#issuecomment-405986762)

*Tag Predicate:* `"union"`

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
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 1.22 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "set operations"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta2.37
Commit 3984d54 (2018-07-18 16:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   25264629 s        260 s    3526568 s  944638763 s          7 s
       #2  3501 MHz  125952422 s          0 s    2055793 s  847314831 s          7 s
       #3  3501 MHz   19352812 s       2395 s    2144981 s  953947234 s         15 s
       #4  3501 MHz   18553356 s          4 s    1689518 s  955666270 s          8 s
       
  Memory: 31.383651733398438 GB (3873.60546875 MB free)
  Uptime: 9.763671e6 sec
  Load Avg:  0.9169921875  1.060546875  1.5048828125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta2.35
Commit 5369849 (2018-07-18 12:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   25376808 s        260 s    3535744 s  944770990 s          7 s
       #2  3501 MHz  126142907 s          0 s    2064135 s  847370052 s          7 s
       #3  3501 MHz   19479769 s       2395 s    2153834 s  954065296 s         15 s
       #4  3501 MHz   18662056 s          4 s    1698288 s  955802723 s          8 s
       
  Memory: 31.383651733398438 GB (6020.87109375 MB free)
  Uptime: 9.766217e6 sec
  Load Avg:  1.0029296875  1.0849609375  1.6103515625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
