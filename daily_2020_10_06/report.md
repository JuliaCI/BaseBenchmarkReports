# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@be1f3abcc64567153305edddfa516c0a3bb27ac6](https://github.com/JuliaLang/julia/commit/be1f3abcc64567153305edddfa516c0a3bb27ac6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/be1f3abcc64567153305edddfa516c0a3bb27ac6#commitcomment-42990591)

*Tag Predicate:* `ALL`

*Daily Job:* 2020-10-06 vs 2020-10-05

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
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 1.42 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Int64}\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Int64} isequal Vector{Float64}\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 8)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"Vector{Bool}\", \"10-90\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"Vector{Bool}\", \"50-50\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Vector{Bool}\", \"50-50\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Vector{Float32}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Vector{Float64}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Vector{UInt64}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Vector{UInt64}\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Matrix{Float64}(10000, 10000)\")"]` | 1.04 (5%)  | 1.09 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"typename(UpperTriangular)\", \"typename(UpperTriangular)\", 256)"]` | 2.33 (45%) :x: | 1.00 (1%)  |
| `["micro", "fib"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "23042", "ComplexF32"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "afoldl", "Int"]` | 0.69 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "conditional"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "no conditional"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "issue 12165", "Float64"]` | 1.45 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1, 1:1)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "parse", "Float64"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["problem", "simplex", "simplex"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large BitSet\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "sequences", "(\"randcycle\", \"MersenneTwister\", \"1000\")"]` | 1.67 (25%) :x: | 1.00 (1%)  |
| `["random", "sequences", "(\"randperm\", \"MersenneTwister\", \"1000\")"]` | 1.65 (25%) :x: | 1.00 (1%)  |
| `["random", "sequences", "(\"randperm\", \"MersenneTwister\", \"5\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random", "sequences", "(\"shuffle!\", \"MersenneTwister\")"]` | 1.66 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"BigInt\")"]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigInt\")"]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"zero\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.68 (40%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.40 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4095)"]` | 1.30 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4096)"]` | 1.31 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Float64\", 4095)"]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Float64\", 4096)"]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Int32\", 4095)"]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Int32\", 4096)"]` | 1.28 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Int64\", 4096)"]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 1.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 1.31 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float64\", 4095)"]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float64\", 4096)"]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Int32\", 4095)"]` | 1.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Int32\", 4096)"]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Int64\", 4096)"]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, ComplexF64, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 1.41 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, ComplexF64, false)"]` | 1.59 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, ComplexF64, true)"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, ComplexF64, (false, true))"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, ComplexF64, (true, true))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 1.35 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 1.44 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, ComplexF64, true)"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, ComplexF64, (false, false))"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, ComplexF64, (true, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 1.42 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Float32}, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float32}, true)"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.6.0-DEV.1139
Commit be1f3ab (2020-10-06 02:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   16289226 s        508 s    1792771 s  778251972 s          4 s
       #2  3501 MHz  124230715 s         22 s    2539812 s  670635120 s          3 s
       #3  3501 MHz   14846351 s        332 s    1089684 s  781289299 s          4 s
       #4  3501 MHz   13893936 s          4 s    1596426 s  781570944 s          3 s
       
  Memory: 31.383651733398438 GB (14493.8671875 MB free)
  Uptime: 7.9801858e7 sec
  Load Avg:  0.97  1.0  1.04
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-10.0.1 (ORCJIT, haswell)

```
