# Benchmark Report

## Job Properties

*Commit(s):* [MasonProtter/julia@8edd7de656ee369699e9aa6c5ef6832060348225](https://github.com/MasonProtter/julia/commit/8edd7de656ee369699e9aa6c5ef6832060348225) vs [JuliaLang/julia@3f620adcba358c58532c94551fdcd739c68adaa5](https://github.com/JuliaLang/julia/commit/3f620adcba358c58532c94551fdcd739c68adaa5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33921#issuecomment-557725952)

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
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1}\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"perf_reduce\", \"Int64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "26942"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "Date"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(100000000, 1)\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 256)"]` | 2.34 (45%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 1.58 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "sum(flatten(collect((i,i+1) for i in 1:1000))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000, 1:1000, 1:1000)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 24, 1)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_devec"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Vector\")"]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt32\", \"RangeGenerator(1:1)\")"]` | 1.44 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"BigInt\")"]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"BigInt\")"]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Int64\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float64\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"positive argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"medium\", \"negative argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"medium\", \"positive argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"one\", \"Float64\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.32 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.09 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.09 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.48 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.48 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.41 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.41 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.41 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 0.33 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 0.33 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 0.28 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 0.28 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.41 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow127\", \"negative argument\", Float32)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float32\")"]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float64\")"]` | 0.33 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float32\")"]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float64\")"]` | 0.32 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float64\")"]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float32\")"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float64\")"]` | 0.41 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp\", \"fast path, k = 1\", \"Float64\")"]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp\", \"no agument reduction, k = 9\", \"Float64\")"]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp\", \"normal path, k = 2\", \"Float64\")"]` | 0.33 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.46 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.41 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.41 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.39 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.41 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.45 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.32 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.33 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.33 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.32 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.32 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.32 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.31 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.32 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 0.30 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.42 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.43 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float64\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float64\")"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x500, dense 500x5 -> dense 50x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 1.66 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 0.77 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 0.61 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Complex{Float64}}, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float32}, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, BigInt}, false)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Bool}, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.520
Commit 8edd7de (2019-11-22 20:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109645106 s       5047 s   12783999 s  5096558893 s         30 s
       #2  3501 MHz  788401130 s        217 s   14351996 s  4424273345 s         25 s
       #3  3501 MHz   93567256 s       3256 s    7584996 s  5126037001 s         34 s
       #4  3501 MHz   87667676 s         34 s   10850033 s  5126530271 s         24 s
       
  Memory: 31.383651733398438 GB (14595.171875 MB free)
  Uptime: 5.2309397e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.516
Commit 3f620ad (2019-11-22 18:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109766985 s       5047 s   12793133 s  5097767120 s         31 s
       #2  3501 MHz  789643142 s        217 s   14378159 s  4424348499 s         25 s
       #3  3501 MHz   93696046 s       3256 s    7590740 s  5127245878 s         34 s
       #4  3501 MHz   87807260 s         34 s   10855518 s  5127728720 s         24 s
       
  Memory: 31.383651733398438 GB (14704.1484375 MB free)
  Uptime: 5.2322837e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, haswell)

```
