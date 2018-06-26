# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d201e628a82ff704d2fa92c5d43902dc68dc1780](https://github.com/JuliaLang/julia/commit/d201e628a82ff704d2fa92c5d43902dc68dc1780) vs [JuliaLang/julia@a23be084d30ccd947e54a6a90933dee016a2aedf](https://github.com/JuliaLang/julia/commit/a23be084d30ccd947e54a6a90933dee016a2aedf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27743#issuecomment-400394055)

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
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, false)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, false)"]` | 1.03 (15%)  | 3.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 0.61 (15%) :white_check_mark: | 3.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 1.31 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, true)"]` | 0.16 (15%) :white_check_mark: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 1.38 (15%) :x: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 0.59 (15%) :white_check_mark: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 1.32 (15%) :x: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 0.54 (15%) :white_check_mark: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 1.22 (15%) :x: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 0.39 (15%) :white_check_mark: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 1.08 (15%)  | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int8, true)"]` | 0.52 (15%) :white_check_mark: | 4.00 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "set operations"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.33
Commit d201e62 (2018-06-26 16:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   18533376 s        259 s    2788286 s  763229537 s          5 s
       #2  3501 MHz   92379102 s          0 s    1458430 s  692326876 s          5 s
       #3  3501 MHz   13444651 s       2389 s    1559542 s  771266702 s         11 s
       #4  3501 MHz   12958064 s          4 s    1196314 s  772488472 s          4 s
       
  Memory: 31.383651733398438 GB (4970.31640625 MB free)
  Uptime: 7.869866e6 sec
  Load Avg:  1.0029296875  1.1005859375  1.78271484375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.31
Commit a23be08 (2018-06-26 16:51 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   18644408 s        259 s    2796819 s  763362232 s          5 s
       #2  3501 MHz   92575160 s          0 s    1466516 s  692375606 s          5 s
       #3  3501 MHz   13563043 s       2389 s    1568198 s  771392203 s         12 s
       #4  3501 MHz   13069775 s          4 s    1205030 s  772620850 s          4 s
       
  Memory: 31.383651733398438 GB (4846.33203125 MB free)
  Uptime: 7.872401e6 sec
  Load Avg:  0.9970703125  1.087890625  1.63916015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
