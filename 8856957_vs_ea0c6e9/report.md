# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8856957737f3330db765d316bdb9b9424fdd1ec0](https://github.com/JuliaLang/julia/commit/8856957737f3330db765d316bdb9b9424fdd1ec0) vs [JuliaLang/julia@ea0c6e9e769df3722127c3a67a8e4894cf2a14ce](https://github.com/JuliaLang/julia/commit/ea0c6e9e769df3722127c3a67a8e4894cf2a14ce)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/31455#issuecomment-476421465)

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
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.2.0-DEV.547
Commit 8856957 (2019-03-25 23:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   45508250 s       2430 s    9716941 s  3074231158 s         12 s
       #2  3501 MHz  259448026 s         14 s    4702382 s  2872656401 s         19 s
       #3  3501 MHz   36491798 s       3161 s    4468056 s  3095628501 s         27 s
       #4  3501 MHz   35203314 s         14 s    3350070 s  3099434864 s         24 s
       
  Memory: 31.383651733398438 GB (5397.36328125 MB free)
  Uptime: 3.1391812e7 sec
  Load Avg:  1.0029296875  1.20361328125  1.65869140625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.2.0-DEV.544
Commit ea0c6e9 (2019-03-25 22:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   45615948 s       2430 s    9724531 s  3074337434 s         12 s
       #2  3501 MHz  259607234 s         14 s    4709788 s  2872711581 s         19 s
       #3  3501 MHz   36619349 s       3161 s    4475424 s  3095715265 s         27 s
       #4  3501 MHz   35314070 s         14 s    3357219 s  3099538807 s         24 s
       
  Memory: 31.383651733398438 GB (5293.703125 MB free)
  Uptime: 3.1394035e7 sec
  Load Avg:  0.9970703125  1.18798828125  1.77783203125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
