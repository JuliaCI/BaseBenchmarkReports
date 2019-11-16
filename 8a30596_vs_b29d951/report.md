# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8a3059662904fff1282dc6c5b41fdf0be077258d](https://github.com/JuliaLang/julia/commit/8a3059662904fff1282dc6c5b41fdf0be077258d) vs [JuliaLang/julia@b29d95119d1f1bd485ba015c2bbfc9b08fcc09b9](https://github.com/JuliaLang/julia/commit/b29d95119d1f1bd485ba015c2bbfc9b08fcc09b9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33829#issuecomment-554555402)

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
| `["array", "accumulate", "(\"accumulate\", \"Int\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.60 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"BitArray\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 256)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Int64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"perf_mapreduce\", \"Int64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"true\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"getindex\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"false\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,1}(100000000,)\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(100000000, 1)\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["micro", "fib"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 1.92 (5%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "json", "parse_json"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Vector\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int64\")"]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"Float64\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"UInt64\")"]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float32\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float3\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"zero\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["shootout", "meteor_contest"]` | 0.96 (5%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 1.69 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat str len 16"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4,))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, BigInt}, false)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigInt, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.484
Commit 8a30596 (2019-11-15 22:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   53582616 s       2445 s   15835619 s  5084088050 s         16 s
       #2  3501 MHz  328644933 s         44 s    6385329 s  4831769755 s         25 s
       #3  3501 MHz   44689018 s       3198 s    5273242 s  5116625571 s         36 s
       #4  3501 MHz   43060520 s         16 s    4092704 s  5121490062 s         32 s
       
  Memory: 31.383651733398438 GB (14458.17578125 MB free)
  Uptime: 5.170249e7 sec
  Load Avg:  0.93505859375  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.482
Commit b29d951 (2019-11-15 22:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   53683762 s       2445 s   15844442 s  5085292504 s         16 s
       #2  3501 MHz  329885802 s         44 s    6410874 s  4831822409 s         25 s
       #3  3501 MHz   44797907 s       3198 s    5277905 s  5117830413 s         36 s
       #4  3501 MHz   43155694 s         16 s    4097140 s  5122709445 s         32 s
       
  Memory: 31.383651733398438 GB (14272.31640625 MB free)
  Uptime: 5.1715683e7 sec
  Load Avg:  1.0078125  1.017578125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
