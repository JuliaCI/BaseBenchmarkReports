# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b9f04a10a9c57b275bcc92a40e68e48874de59a4](https://github.com/JuliaLang/julia/commit/b9f04a10a9c57b275bcc92a40e68e48874de59a4) vs [JuliaLang/julia@ee07b8cb23e5330d25d0b05accdc0278997a0b3f](https://github.com/JuliaLang/julia/commit/ee07b8cb23e5330d25d0b05accdc0278997a0b3f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27743#issuecomment-402709408)

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
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, true)"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, false)"]` | 3.12 (15%) :x: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 0.88 (15%)  | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 1.35 (15%) :x: | 7.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, true)"]` | 1.25 (15%) :x: | 7.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 1.34 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 1.46 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 1.34 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 1.24 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 7.48 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 0.36 (15%) :white_check_mark: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 5.56 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int8, true)"]` | 0.52 (15%) :white_check_mark: | 5.00 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "set operations"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.155
Commit b9f04a1 (2018-07-04 23:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   22158162 s        259 s    3166673 s  834844449 s          6 s
       #2  3501 MHz  108966306 s          0 s    1724624 s  751159011 s          6 s
       #3  3501 MHz   16233606 s       2392 s    1809722 s  843966016 s         13 s
       #4  3501 MHz   15586648 s          4 s    1412923 s  845417633 s          6 s
       
  Memory: 31.383651733398438 GB (3919.578125 MB free)
  Uptime: 8.627995e6 sec
  Load Avg:  1.0029296875  1.09375  1.509765625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.152
Commit ee07b8c (2018-07-04 17:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   22281979 s        259 s    3175077 s  834955320 s          6 s
       #2  3501 MHz  109142439 s          0 s    1732480 s  751218219 s          6 s
       #3  3501 MHz   16341062 s       2392 s    1818028 s  844093329 s         13 s
       #4  3501 MHz   15693197 s          4 s    1420879 s  845546362 s          6 s
       
  Memory: 31.383651733398438 GB (6111.328125 MB free)
  Uptime: 8.630433e6 sec
  Load Avg:  0.9970703125  1.0849609375  1.60400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
