# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9babbf5dc6d2d08b9ed422386830460516cb8aed](https://github.com/JuliaLang/julia/commit/9babbf5dc6d2d08b9ed422386830460516cb8aed)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/9babbf5dc6d2d08b9ed422386830460516cb8aed#commitcomment-36207462)

*Tag Predicate:* `ALL`

*Daily Job:* 2019-12-01 vs 2019-11-30

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
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 2048)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "26942"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"unspecified\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 2.53 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"50-50\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 1.10 (5%) :x: | 1.10 (1%) :x: |
| `["io", "serialization", "(\"deserialize\", \"Matrix{Float64}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 0.63 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "sum(flatten(collect((i,i+1) for i in 1:1000))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000, 1:1000)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000, 1:1000, 1:1000)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt8\", \"RangeGenerator(1:1)\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"Float64\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Int64\")"]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Int64\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"UInt64\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"BigInt\")"]` | 1.79 (40%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "backtracking"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 1.75 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.64 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.52 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.77 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Complex{Float64}}, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.535
Commit 9babbf5 (2019-11-30 20:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110936611 s       5048 s   12938146 s  5166096470 s         31 s
       #2  3501 MHz  800979574 s        217 s   14656571 s  4482452625 s         26 s
       #3  3501 MHz   94919300 s       3258 s    7658958 s  5195727549 s         35 s
       #4  3501 MHz   88934447 s         34 s   10965439 s  5196232170 s         24 s
       
  Memory: 31.383651733398438 GB (15108.34765625 MB free)
  Uptime: 5.3020845e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, haswell)

```
