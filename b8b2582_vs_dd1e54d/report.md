# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b8b25823fc831e3f5e48d210b0e65b2ca6d1522a](https://github.com/JuliaLang/julia/commit/b8b25823fc831e3f5e48d210b0e65b2ca6d1522a) vs [JuliaLang/julia@dd1e54d54dc4b6c342602c9169de268c5e37ac2a](https://github.com/JuliaLang/julia/commit/dd1e54d54dc4b6c342602c9169de268c5e37ac2a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/35982#issuecomment-632454232)

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
| `["array", "accumulate", "(\"accumulate\", \"Int\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat\", 5)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "4467"]` | 0.08 (5%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 2.77 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.75 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.53 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 3.77 (5%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Int\", \"Float64\")"]` | 2.36 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 1.28 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 1.28 (50%)  | 1.40 (1%) :x: |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.40 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.40 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.40 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.45 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.44 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.45 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "26942"]` | 1.89 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 1.65 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 1.46 (25%) :x: | 1.21 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"pop!\")"]` | 2.13 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"pop!\")"]` | 1.94 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"String\", \"pop!\")"]` | 1.95 (25%) :x: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"iterate second\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"getindex\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"in\", \"false\")"]` | 1.76 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"in\", \"true\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"getindex\")"]` | 1.20 (25%)  | 2.00 (1%) :x: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"pop!\", \"specified\")"]` | 1.09 (25%)  | 1.33 (1%) :x: |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"getindex\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"new\")"]` | 1.44 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"pop!\", \"unspecified\")"]` | 2.13 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.63 (25%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "DateTime"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "string", "DateTime"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"10-90\")"]` | 1.47 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"90-10\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,1}(100000000,)\")"]` | 0.91 (5%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 0.82 (5%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(100000000, 1)\")"]` | 0.90 (5%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["io", "read", "read"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "read", "readstring"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"Vector\", 256)"]` | 1.09 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Vector\", 1024)"]` | 0.96 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Vector\", 256)"]` | 1.10 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"Vector\", 256)"]` | 1.06 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.50 (45%) :x: | 1.02 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.41 (45%)  | 1.02 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Bidiagonal\", \"Vector\", 1024)"]` | 1.10 (45%)  | 1.02 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Bidiagonal\", \"Vector\", 256)"]` | 1.38 (45%)  | 1.09 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"Vector\", 256)"]` | 1.06 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Tridiagonal\", \"Vector\", 256)"]` | 1.19 (45%)  | 1.02 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"Vector\", 256)"]` | 1.09 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"mul!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 1024)"]` | 0.92 (45%)  | 1.33 (1%) :x: |
| `["linalg", "arithmetic", "(\"mul!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 256)"]` | 0.92 (45%)  | 1.33 (1%) :x: |
| `["linalg", "blas", "gbmv!"]` | 0.93 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "gbmv"]` | 0.93 (40%)  | 1.01 (1%) :x: |
| `["linalg", "blas", "gemm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "gemv!"]` | 0.89 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "gemv"]` | 0.90 (40%)  | 1.01 (1%) :x: |
| `["linalg", "blas", "ger!"]` | 0.87 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "sbmv!"]` | 0.95 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "sbmv"]` | 0.95 (40%)  | 1.01 (1%) :x: |
| `["linalg", "blas", "symm!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "symv!"]` | 0.97 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "symv"]` | 0.96 (40%)  | 1.01 (1%) :x: |
| `["linalg", "blas", "syr!"]` | 0.88 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "trmv!"]` | 1.00 (40%)  | Inf (1%) :x: |
| `["linalg", "blas", "trsv!"]` | 0.95 (40%)  | Inf (1%) :x: |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 256)"]` | 1.37 (45%)  | 1.03 (1%) :x: |
| `["linalg", "small exp #29116"]` | 4.15 (5%) :x: | 1.30 (1%) :x: |
| `["micro", "fib"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "randmatstat"]` | 1.56 (5%) :x: | 1.03 (1%) :x: |
| `["misc", "allocation elision view", "conditional"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "issue 12165", "Float16"]` | 1.81 (5%) :x: | 1.00 (1%)  |
| `["misc", "issue 12165", "Float32"]` | 1.90 (5%) :x: | 1.00 (1%)  |
| `["misc", "issue 12165", "Float64"]` | 1.98 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "parse", "Int"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "chaosgame", "chaosgame"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 1.00 (5%)  | 0.98 (1%) :white_check_mark: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"'a':'z'\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 1.57 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 1.45 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large BitSet\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small BitSet\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small String\")"]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:1\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551615\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float32\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float3\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"frexp\", \"norm\", \"Float64\")"]` | 1.62 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 1.48 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["shootout", "fasta"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["shootout", "k_nucleotide"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 1.83 (5%) :x: | 1.00 (1%)  |
| `["shootout", "revcomp"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"forwards\", \"random\")"]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 2.20 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 1000)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 2.17 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.89 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 6.48 (5%) :x: | 1.31 (1%) :x: |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 3.51 (5%) :x: | 1.10 (1%) :x: |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 1.23 (5%) :x: | 1.01 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 2.10 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 10)"]` | 8.47 (30%) :x: | 1.60 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 100)"]` | 1.64 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 3.94 (30%) :x: | 1.49 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 1.13 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 7.05 (30%) :x: | 1.77 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 3.04 (30%) :x: | 1.26 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 1000)"]` | 1.12 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 10.70 (30%) :x: | 2.02 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 6.60 (30%) :x: | 1.39 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 1.78 (30%) :x: | 1.06 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 7.73 (30%) :x: | 1.87 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 100)"]` | 1.33 (30%) :x: | 1.09 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"range\", 10)"]` | 7.80 (30%) :x: | 1.81 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"range\", 100)"]` | 1.58 (30%) :x: | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 10)"]` | 4.25 (30%) :x: | 1.94 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 100)"]` | 1.86 (30%) :x: | 1.34 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 1.06 (30%)  | 1.19 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 3.91 (30%) :x: | 1.75 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 1.75 (30%) :x: | 1.27 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 1.11 (30%)  | 1.15 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 4.09 (30%) :x: | 1.50 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.88 (30%) :x: | 1.20 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 1.10 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 10)"]` | 3.99 (30%) :x: | 2.19 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 100)"]` | 1.66 (30%) :x: | 1.43 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.12 (30%)  | 1.24 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 2.11 (30%) :x: | 1.60 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 2.12 (30%) :x: | 1.60 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 2.45 (30%) :x: | 1.30 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 1.12 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 2.01 (30%) :x: | 1.15 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"logical\", 10000)"]` | 1.03 (30%)  | 1.02 (1%) :x: |
| `["string", "readuntil", "backtracking"]` | 2.02 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "barbarian backtrack"]` | 1.84 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "no backtracking"]` | 1.40 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 2.28 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 2"]` | 1.64 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 2.28 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (2,))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.53 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.35 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.42 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 1.41 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Float64, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, BigFloat}, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Bool, false)"]` | 2.66 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.6.0-DEV.78
Commit b8b2582 (2020-05-22 01:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  140446983 s       5056 s   15967727 s  6624592513 s         35 s
       #2  3501 MHz  1058219365 s        217 s   20905403 s  5712000409 s         27 s
       #3  3501 MHz  125322150 s       3304 s    9490558 s  6655773317 s         38 s
       #4  3501 MHz  117696254 s         43 s   13624961 s  6657482178 s         27 s
       
  Memory: 31.383651733398438 GB (18820.5078125 MB free)
  Uptime: 6.7963083e7 sec
  Load Avg:  1.01806640625  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.6.0-DEV.76
Commit dd1e54d (2020-05-21 21:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  140597969 s       5056 s   15977490 s  6625785405 s         35 s
       #2  3501 MHz  1059462441 s        217 s   20932785 s  5712087457 s         27 s
       #3  3501 MHz  125473876 s       3304 s    9496834 s  6656972995 s         38 s
       #4  3501 MHz  117851460 s         43 s   13630964 s  6658678856 s         27 s
       
  Memory: 31.383651733398438 GB (18420.390625 MB free)
  Uptime: 6.7976667e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
