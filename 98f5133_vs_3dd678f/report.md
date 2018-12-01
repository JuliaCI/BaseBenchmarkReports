# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@98f5133f1c7e4f26331d42e7fa32f941d368354a](https://github.com/JuliaLang/julia/commit/98f5133f1c7e4f26331d42e7fa32f941d368354a) vs [JuliaLang/julia@3dd678f646e4403aede51389fcca7262839b5d15](https://github.com/JuliaLang/julia/commit/3dd678f646e4403aede51389fcca7262839b5d15)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30222)

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
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim2\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 0.37 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"BitArray\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 8)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 8)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_fast!"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 0.77 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate second\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"false\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"true\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"specified\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Vector\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "skipchars"]` | 0.86 (5%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["misc", "20517"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "conditional"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000, 1:1000)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "splatting", "(3, 3, 3)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.61 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float64\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.37 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float64\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float64\")"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float64\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float64\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float64\")"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float64\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"2.0^-28 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"2.0^-28 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"1.0 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"1.0 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 0.99 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 1.09 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 1.02 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.01 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 0.98 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 1.01 (30%)  | 0.00 (1%) :white_check_mark: |
| `["string", "findfirst", "Char"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "repeat", "repeat str len 16"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (8,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.30 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, false)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, true)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.1.0-DEV.775
Commit 98f5133 (2018-11-30 22:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   38913385 s       2414 s    6852028 s  2093676838 s         11 s
       #2  3501 MHz  209365892 s         14 s    3758839 s  1931125659 s         17 s
       #3  3501 MHz   30047722 s       3138 s    3515172 s  2110550942 s         24 s
       #4  3501 MHz   28831476 s         11 s    2723449 s  2113564080 s         20 s
       
  Memory: 31.383651733398438 GB (4866.01953125 MB free)
  Uptime: 2.1460479e7 sec
  Load Avg:  1.0234375  1.02392578125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.772
Commit 3dd678f (2018-11-30 22:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   39024871 s       2414 s    6863130 s  2094800466 s         11 s
       #2  3501 MHz  210536741 s         14 s    3774704 s  1931189279 s         17 s
       #3  3501 MHz   30167752 s       3138 s    3522304 s  2111674015 s         24 s
       #4  3501 MHz   28954322 s         11 s    2730729 s  2114684472 s         20 s
       
  Memory: 31.383651733398438 GB (4689.984375 MB free)
  Uptime: 2.147299e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
