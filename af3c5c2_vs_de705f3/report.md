# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@af3c5c2fb141fd4e9eea2c89d84cb2178efd568d](https://github.com/JuliaLang/julia/commit/af3c5c2fb141fd4e9eea2c89d84cb2178efd568d) vs [JuliaLang/julia@de705f3b6961a288c0b79d2f88010597e846faa8](https://github.com/JuliaLang/julia/commit/de705f3b6961a288c0b79d2f88010597e846faa8)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25377#issuecomment-383413030)

*Tag Predicate:* `!"arithmetic"`

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 0.87 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 0.76 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.28 (15%) :x: | 1.03 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.34 (15%) :x: | 1.05 (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.02 (15%)  | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 1.02 (15%)  | 1.10 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 1.02 (15%)  | 1.14 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 1.07 (15%)  | 1.13 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 1.29 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 1.12 (15%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"getindex\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 6.61 (15%) :x: | 7.58 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 2"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 1.54 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 1.54 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 0.99 (15%)  | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.50 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 1.55 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.34 (15%) :x: | 0.32 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 4.90 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 4.96 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 0.93 (15%)  | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 4.00 (15%) :x: | 0.96 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 4.03 (15%) :x: | 0.96 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 1.07 (15%)  | 0.78 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 4.60 (15%) :x: | 0.89 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 4.72 (15%) :x: | 0.89 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.97 (15%)  | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 4.22 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 4.23 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 0.97 (15%)  | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 4.16 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 4.16 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 1.17 (15%) :x: | 0.52 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 4.52 (15%) :x: | 0.76 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 4.95 (15%) :x: | 0.76 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 2.09 (15%) :x: | 0.99 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.07 (15%)  | 0.97 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 2.36 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.67 (15%) :x: | 0.38 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 7.93 (15%) :x: | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 1.25 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 5.36 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.45 (15%) :x: | 0.81 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 7.15 (15%) :x: | 0.91 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 1.20 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 5.84 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 1.16 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 6.11 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.45 (15%) :x: | 0.56 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 7.52 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 1.43 (15%) :x: | 0.90 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 5.83 (15%) :x: | 0.95 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 1.43 (15%) :x: | 0.90 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 5.75 (15%) :x: | 0.95 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.61 (15%) :x: | 0.38 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 7.92 (15%) :x: | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.25 (15%) :x: | 0.94 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 5.46 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 1.37 (15%) :x: | 0.81 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 7.29 (15%) :x: | 0.91 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 1.13 (15%)  | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 6.14 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 1.20 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 6.04 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.48 (15%) :x: | 0.56 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 7.50 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 1.18 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "accumulate"]`
- `["array", "any/all"]`
- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "equality"]`
- `["array", "growth"]`
- `["array", "index"]`
- `["array", "reductions"]`
- `["array", "reverse"]`
- `["array", "setindex!"]`
- `["array", "subarray"]`
- `["broadcast", "dotop"]`
- `["broadcast", "fusion"]`
- `["broadcast", "mix_scalar_tuple"]`
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "optimizations"]`
- `["collection", "queries & updates"]`
- `["collection", "set operations"]`
- `["dates", "accessor"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["find", "findall"]`
- `["find", "findnext"]`
- `["find", "findprev"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["micro"]`
- `["misc", "afoldl"]`
- `["misc", "bitshift"]`
- `["misc", "julia"]`
- `["misc", "parse"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
- `["parallel", "remotecall"]`
- `["problem", "chaosgame"]`
- `["problem", "fem"]`
- `["problem", "go"]`
- `["problem", "grigoriadis khachiyan"]`
- `["problem", "imdb"]`
- `["problem", "json"]`
- `["problem", "laplacian"]`
- `["problem", "monte carlo"]`
- `["problem", "raytrace"]`
- `["problem", "seismic"]`
- `["problem", "simplex"]`
- `["problem", "spellcheck"]`
- `["problem", "stockcorr"]`
- `["problem", "ziggurat"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["scalar", "acos"]`
- `["scalar", "acosh"]`
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
- `["shootout"]`
- `["simd"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "transpose"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.4986
Commit af3c5c2 (2018-04-22 21:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    5901110 s        261 s     737044 s  219821375 s          2 s
       #2  3501 MHz   36832374 s          0 s     544884 s  189463216 s          0 s
       #3  3501 MHz    4289432 s       2368 s     426088 s  221845260 s          2 s
       #4  3501 MHz    4194856 s          0 s     534165 s  222027947 s          1 s
       
  Memory: 31.383651733398438 GB (6092.84375 MB free)
  Uptime: 2.269805e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4931
Commit de705f3 (2018-04-22 20:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    6013478 s        261 s     746685 s  220402803 s          2 s
       #2  3501 MHz   37462302 s          0 s     554213 s  189529505 s          0 s
       #3  3501 MHz    4375572 s       2368 s     433675 s  222456579 s          2 s
       #4  3501 MHz    4283150 s          0 s     541680 s  222637632 s          1 s
       
  Memory: 31.383651733398438 GB (5851.91015625 MB free)
  Uptime: 2.276865e6 sec
  Load Avg:  1.00634765625  1.01611328125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
