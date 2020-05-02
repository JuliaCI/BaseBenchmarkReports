# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f2fa6cf665ce078cd46f8ce0d139bf6b644884ad](https://github.com/JuliaLang/julia/commit/f2fa6cf665ce078cd46f8ce0d139bf6b644884ad)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f2fa6cf665ce078cd46f8ce0d139bf6b644884ad#commitcomment-38888817)

*Tag Predicate:* `ALL`

*Daily Job:* 2020-05-02 vs 2020-05-01

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 0.63 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.52 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 1.49 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"perf_reduce\", \"Int64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"IdDict\", \"Int\", \"filter!\")"]` | 1.21 (25%)  | 1.03 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter!\")"]` | 0.97 (25%)  | 1.01 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 1.43 (25%) :x: | 3.75 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 0.93 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\")"]` | 0.91 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.82 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"iterator\")"]` | 0.95 (25%)  | 1.01 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\")"]` | 0.95 (25%)  | 1.01 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.95 (25%)  | 1.01 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"iterator\")"]` | 1.28 (25%) :x: | 2.65 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\")"]` | 1.30 (25%) :x: | 2.65 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\", \"sizehint!\")"]` | 1.33 (25%) :x: | 3.07 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 0.93 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 0.91 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.89 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"iterate second\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 1.00 (25%)  | 1.04 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"in\", \"false\")"]` | 0.24 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"new\")"]` | 0.31 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"new\")"]` | 0.32 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"overwrite\")"]` | 0.94 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"in\", \"true\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"in\", \"false\")"]` | 0.67 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"push!\", \"new\")"]` | 0.84 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"setindex!\", \"new\")"]` | 0.83 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"setindex!\", \"overwrite\")"]` | 0.95 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"in\", \"false\")"]` | 0.63 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"push!\", \"new\")"]` | 0.90 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"new\")"]` | 0.88 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"overwrite\")"]` | 1.05 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"false\")"]` | 0.23 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"new\")"]` | 0.26 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"new\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 0.90 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 0.41 (25%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"setindex!\")"]` | 0.89 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 0.04 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 0.95 (25%)  | 0.73 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.93 (25%)  | 0.73 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 0.97 (25%)  | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.93 (25%)  | 0.65 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"BitSet\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.27 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(100000000, 1)\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 256)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "conditional"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["misc", "allocation elision view", "no conditional"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small BitSet\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Vector\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small String\")"]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Vector\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"'a':'z'\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large String\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small String\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", 100)"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"1 <= abs(x) < 2\", \"positive argument\", \"Float32\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.35 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.53 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinf\", \"Complex{BigFloat}\")"]` | 2.81 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 0.95 (5%)  | 0.84 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 0.99 (30%)  | 1.03 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 1.09 (30%)  | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 10)"]` | 1.06 (30%)  | 1.14 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 1000)"]` | 1.01 (30%)  | 1.06 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 0.95 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 1.00 (30%)  | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 0.97 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 1.04 (30%)  | 1.14 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 1000)"]` | 0.86 (30%)  | 1.06 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 0.88 (30%)  | 0.82 (1%) :white_check_mark: |
| `["string", "findfirst", "Char"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 0.56 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.52 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 1.35 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.41 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Complex{Float64}}, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Float64}, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.5.0-DEV.780
Commit f2fa6cf (2020-05-02 01:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  137052469 s       5056 s   15637707 s  6456018712 s         35 s
       #2  3501 MHz  1032584119 s        217 s   20276304 s  5565910317 s         26 s
       #3  3501 MHz  121871167 s       3296 s    9265136 s  6486898531 s         38 s
       #4  3501 MHz  114448159 s         43 s   13315833 s  6488570617 s         27 s
       
  Memory: 31.383651733398438 GB (18875.08984375 MB free)
  Uptime: 6.6236607e7 sec
  Load Avg:  1.03955078125  1.0341796875  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
