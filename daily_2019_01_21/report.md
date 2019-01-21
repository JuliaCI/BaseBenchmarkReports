# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ee6d662e901ad120ff24ee82919e15447db4bfbd](https://github.com/JuliaLang/julia/commit/ee6d662e901ad120ff24ee82919e15447db4bfbd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ee6d662e901ad120ff24ee82919e15447db4bfbd#commitcomment-32003661)

*Tag Predicate:* `ALL`

*Daily Job:* 2019-01-21 vs 2019-01-20

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
| `["array", "cat", "(\"catnd\", 5)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_fast!"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Vector\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"90-10\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"deserialize\", \"Matrix{Float64}\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "small exp #29116"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["micro", "randmatmul"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "18129"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "23042", "Float64"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1, 1:1)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "fem", "sparse_fem"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "stockcorr", "stockcorr"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small String\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"zero\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["shootout", "meteor_contest"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "pidigits"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse matvec", "adjoint"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse matvec", "non-adjoint"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (default), matrix rhs"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (default), vector rhs"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (qr), matrix rhs"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (qr), vector rhs"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "square system (ldlt), vector rhs"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "square system (lu), matrix rhs"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "sparse solves", "square system (lu), vector rhs"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 1"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "repeat", "repeat str len 1"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (16, 16), (16, 16))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (2,))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 0.77 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.69 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Int64, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, BigInt}, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Complex{Float64}}, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, BigInt}, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Bool}, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.2.0-DEV.187
Commit ee6d662 (2019-01-21 03:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71987495 s       5014 s    8024360 s  2502597225 s         23 s
       #2  3501 MHz  416630837 s        203 s    6864486 s  2163374746 s         19 s
       #3  3501 MHz   55556390 s       3224 s    4708864 s  2526506387 s         26 s
       #4  3501 MHz   51940269 s          2 s    6109835 s  2528102819 s         17 s
       
  Memory: 31.383651733398438 GB (5398.46484375 MB free)
  Uptime: 2.5889552e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
