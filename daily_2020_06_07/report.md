# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@98e678fd9806856a4c0a12f711e1ee397994deeb](https://github.com/JuliaLang/julia/commit/98e678fd9806856a4c0a12f711e1ee397994deeb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/98e678fd9806856a4c0a12f711e1ee397994deeb#commitcomment-39723028)

*Tag Predicate:* `ALL`

*Daily Job:* 2020-06-07 vs 2020-06-06

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
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "3d"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"tup_tup\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"getindex\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"in\", \"true\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"getindex\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"pop!\", \"specified\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["micro", "fib"]` | 2254.08 (5%) :x: | 1.00 (1%)  |
| `["misc", "20517"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["misc", "parse", "Int"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"'a':'z'\")"]` | 1.87 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small BitSet\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float16\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"BigInt\")"]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"BigInt\")"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.77 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.35 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float3\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 2"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (8, 8), (8, 8))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.53 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 1.72 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.69 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, BigInt}, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, BigInt}, false)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, BigInt}, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.6.0-DEV.186
Commit 98e678f (2020-06-06 18:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  143552328 s       5056 s   16244823 s  6759294595 s         35 s
       #2  3501 MHz  1083549786 s        217 s   21515924 s  5824219736 s         27 s
       #3  3501 MHz  128478603 s       3307 s    9672662 s  6790725477 s         38 s
       #4  3501 MHz  120647819 s         43 s   13892790 s  6792455955 s         27 s
       
  Memory: 31.383651733398438 GB (20192.4765625 MB free)
  Uptime: 6.9346661e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
