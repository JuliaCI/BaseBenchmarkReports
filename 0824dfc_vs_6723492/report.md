# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0824dfcdaa923b874aea156683f70de67849a099](https://github.com/JuliaLang/julia/commit/0824dfcdaa923b874aea156683f70de67849a099) vs [JuliaLang/julia@67234925efbac41f58249839ff03b4b9d36c1ec0](https://github.com/JuliaLang/julia/commit/67234925efbac41f58249839ff03b4b9d36c1ec0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33007#issuecomment-523423176)

*Tag Predicate:* `"broadcast"`

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
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 0.99 (5%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 1.01 (5%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["broadcast"]`
- `["broadcast", "dotop"]`
- `["broadcast", "fusion"]`
- `["broadcast", "mix_scalar_tuple"]`
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.4.0-DEV.26
Commit 0824dfc (2019-08-21 11:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   50513940 s       2440 s   13646376 s  4343898391 s         14 s
       #2  3501 MHz  303760085 s         36 s    5685677 s  4109639193 s         21 s
       #3  3501 MHz   41559543 s       3182 s    4946422 s  4372569998 s         34 s
       #4  3501 MHz   40094717 s         16 s    3776119 s  4376936771 s         30 s
       
  Memory: 31.383651733398438 GB (12324.09375 MB free)
  Uptime: 4.4222175e7 sec
  Load Avg:  0.9169921875  1.13623046875  1.4990234375
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
       #1  3501 MHz   50620689 s       2440 s   13651343 s  4343991214 s         14 s
       #2  3501 MHz  303896545 s         36 s    5691111 s  4109702011 s         21 s
       #3  3501 MHz   41657992 s       3182 s    4951181 s  4372671459 s         34 s
       #4  3501 MHz   40202798 s         16 s    3780813 s  4377028771 s         30 s
       
  Memory: 31.383651733398438 GB (12157.07421875 MB free)
  Uptime: 4.4224226e7 sec
  Load Avg:  1.0029296875  1.1806640625  1.6982421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
