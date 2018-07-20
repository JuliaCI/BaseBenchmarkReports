# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@b1ba1118e5c0b23fe210dfd066a20c1800c9d4b0](https://github.com/pkofod/julia/commit/b1ba1118e5c0b23fe210dfd066a20c1800c9d4b0) vs [JuliaLang/julia@e7acea7c72c41c8283127ebadf8b81652b9ecf6e](https://github.com/JuliaLang/julia/commit/e7acea7c72c41c8283127ebadf8b81652b9ecf6e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25903#issuecomment-406708265)

*Tag Predicate:* `"scalar"`

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
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Int64\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float64\")"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float64\")"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float64\")"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float64\")"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float64\")"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["scalar", "acos"]`
- `["scalar", "acosh"]`
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "asinh"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "atanh"]`
- `["scalar", "cbrt"]`
- `["scalar", "cos"]`
- `["scalar", "cosh"]`
- `["scalar", "exp2"]`
- `["scalar", "expm1"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "sinh"]`
- `["scalar", "tan"]`
- `["scalar", "tanh"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta2.65
Commit b1ba111 (2018-07-20 13:33 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   25494302 s        260 s    3570262 s  962991817 s          7 s
       #2  3501 MHz  126427046 s          0 s    2085490 s  865483638 s          8 s
       #3  3501 MHz   19599561 s       2395 s    2178383 s  972338834 s         15 s
       #4  3501 MHz   18776848 s          4 s    1717784 s  974088675 s          9 s
       
  Memory: 31.383651733398438 GB (7644.08203125 MB free)
  Uptime: 9.950528e6 sec
  Load Avg:  1.00341796875  1.0146484375  1.19482421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta2.57
Commit e7acea7 (2018-07-20 13:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   25616594 s        260 s    3579630 s  963206878 s          7 s
       #2  3501 MHz  126705143 s          0 s    2094146 s  865544303 s          8 s
       #3  3501 MHz   19718980 s       2395 s    2187277 s  972557751 s         15 s
       #4  3501 MHz   18888375 s          4 s    1726496 s  974315808 s          9 s
       
  Memory: 31.383651733398438 GB (7117.49609375 MB free)
  Uptime: 9.954008e6 sec
  Load Avg:  1.2431640625  1.064453125  1.240234375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
