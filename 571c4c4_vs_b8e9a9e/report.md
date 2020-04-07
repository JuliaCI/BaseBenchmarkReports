# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@571c4c41f7354414e4e80348b9f9d691818e26be](https://github.com/JuliaLang/julia/commit/571c4c41f7354414e4e80348b9f9d691818e26be) vs [JuliaLang/julia@b8e9a9ecc62ab49003bd4f1834771bdeb8cb1aa2](https://github.com/JuliaLang/julia/commit/b8e9a9ecc62ab49003bd4f1834771bdeb8cb1aa2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/35229#issuecomment-610287648)

*Tag Predicate:* `ALL`

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
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_bool_load!"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"BitArray\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 2048)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"perf_reduce\", \"Int64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "26942"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "Date"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 0.89 (5%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["io", "serialization", "(\"deserialize\", \"Matrix{Float64}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "fib"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["micro", "printfd"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Float64"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "afoldl", "Int"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 1.80 (5%) :x: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["misc", "julia", "(\"macroexpand\", \"evalpoly\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Vector\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int32\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"ImplicitRNG\", \"Float64\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float32\")"]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float64\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float32\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 1.50 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"negative argument\", \"Float64\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"positive argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4,))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float32}, true)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Bool}, false)"]` | 1.59 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Int8}, false)"]` | 0.63 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Int8}, false)"]` | 1.65 (5%) :x: | 1.00 (1%)  |

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
- `["broadcast"]`
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
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["find", "findall"]`
- `["find", "findnext"]`
- `["find", "findprev"]`
- `["io", "array_limit"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["io"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`
- `["micro"]`
- `["misc"]`
- `["misc", "23042"]`
- `["misc", "afoldl"]`
- `["misc", "allocation elision view"]`
- `["misc", "bitshift"]`
- `["misc", "issue 12165"]`
- `["misc", "iterators"]`
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
- `["shootout"]`
- `["simd"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "sparse matvec"]`
- `["sparse", "sparse solves"]`
- `["sparse", "transpose"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["string", "repeat"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "misc"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.4.0
Commit 571c4c4 (2020-04-07 06:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   55538664 s       2449 s   19468634 s  6313810990 s         18 s
       #2  3501 MHz  346721731 s         62 s    7230226 s  6052028927 s         26 s
       #3  3501 MHz   46695988 s       3224 s    5524807 s  6352575868 s         40 s
       #4  3501 MHz   44928610 s         19 s    4345996 s  6358774436 s         36 s
       
  Memory: 31.383651733398438 GB (18590.38671875 MB free)
  Uptime: 6.4098574e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0
Commit b8e9a9e (2020-03-21 16:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   55674964 s       2449 s   19478508 s  6315052425 s         18 s
       #2  3501 MHz  348019138 s         62 s    7255711 s  6052098256 s         26 s
       #3  3501 MHz   46824271 s       3224 s    5530282 s  6353833126 s         40 s
       #4  3501 MHz   45046658 s         19 s    4351228 s  6360043406 s         36 s
       
  Memory: 31.383651733398438 GB (18196.85546875 MB free)
  Uptime: 6.41125e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, haswell)

```
