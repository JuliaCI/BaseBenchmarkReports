# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@62b93bba01bcf8dddd1e3cd4965b004837c60f5d](https://github.com/JuliaLang/julia/commit/62b93bba01bcf8dddd1e3cd4965b004837c60f5d) vs [JuliaLang/julia@83ce7ba119ae49f968a74f64e423e0ff5c2fbc71](https://github.com/JuliaLang/julia/commit/83ce7ba119ae49f968a74f64e423e0ff5c2fbc71)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27337#issuecomment-396488898)

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
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_indexing\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 1.05 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.26 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.27 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.26 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.27 (50%)  | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 5.88 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 1.36 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 1.00 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 1.01 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 0.99 (15%)  | 2.00 (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 0.99 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 1.00 (15%)  | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 163.48 (15%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Vector\", \"abstract\", \"Nothing\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"unspecified\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 1.82 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 1.68 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 9.82 (25%) :x: | 1.12 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 3.79 (25%) :x: | 1.12 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 4.68 (25%) :x: | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 3.61 (25%) :x: | 1.12 (1%) :x: |
| `["dates", "string", "Date"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "string", "DateTime"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.06 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 1.02 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 1.07 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.09 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 0.98 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.99 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.06 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 0.97 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.09 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 1.07 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.93 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 1.03 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.10 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.09 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 1.03 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.47 (45%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.08 (15%)  | 1.07 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large String\")"]` | 1.06 (25%)  | 1.01 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Vector\")"]` | 1.09 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small String\")"]` | 1.06 (25%)  | 1.43 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Vector\")"]` | 1.07 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large String\")"]` | 1.04 (25%)  | 1.01 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Vector\")"]` | 1.06 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small String\")"]` | 1.04 (25%)  | 1.43 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Vector\")"]` | 1.06 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large String\")"]` | 1.05 (25%)  | 1.01 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Vector\")"]` | 1.07 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small String\")"]` | 1.04 (25%)  | 1.43 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Vector\")"]` | 1.05 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"'a':'z'\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 1.57 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 1.25 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 1.07 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 1.49 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.38 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.52 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 1.17 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.28 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"'a':'z'\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 1.46 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 1.44 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 1.36 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 1.40 (25%) :x: | Inf (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\")"]` | 1.30 (25%) :x: | 1.38 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", 100)"]` | 1.06 (25%)  | 1.15 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 1.03 (25%)  | 1.12 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 1.04 (25%)  | 1.04 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\")"]` | 1.13 (25%)  | 1.38 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\", 100)"]` | 1.05 (25%)  | 1.15 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["random", "sequences", "(\"randcycle\", \"MersenneTwister\", \"1000\")"]` | 1.51 (25%) :x: | 1.00 (1%)  |
| `["random", "sequences", "(\"randperm\", \"MersenneTwister\", \"1000\")"]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["random", "sequences", "(\"shuffle!\", \"MersenneTwister\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float16\")"]` | 1.62 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float16\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float16\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 1.03 (50%)  | 1.03 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 1.01 (50%)  | 1.03 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow127\", \"negative argument\", Float32)"]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 3.46 (15%) :x: | 20.74 (1%) :x: |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 0.59 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 2.56 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 3.21 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 1.07 (30%)  | 12.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 1.03 (30%)  | 10.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.06 (30%)  | 74.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.06 (30%)  | 10.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.02 (30%)  | 12.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x200, sparse 2000x200 -> dense 20x2000\")"]` | 1.07 (30%)  | 92.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 1.07 (30%)  | 915.29 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 200x2000 -> dense 20x200\")"]` | 1.04 (30%)  | 92.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x20, dense 20x20 -> dense 2000x20\")"]` | 1.06 (30%)  | 12.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x200, dense 20x200 -> dense 2000x20\")"]` | 1.07 (30%)  | 92.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 1.07 (30%)  | 915.29 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x20, dense 200x20 -> dense 200x200\")"]` | 1.05 (30%)  | 10.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.06 (30%)  | 74.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x2000, dense 20x2000 -> dense 200x20\")"]` | 1.06 (30%)  | 92.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.05 (30%)  | 12.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x200, dense 200x200 -> dense 20x200\")"]` | 1.06 (30%)  | 10.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.10 (30%)  | 1.08 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 1.18 (30%)  | 1.06 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 1.09 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 1.18 (30%)  | 1.05 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.18 (30%)  | 1.48 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 1.18 (30%)  | 1.43 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.00 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.03 (30%)  | 1.04 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 1.90 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.91 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 2.00 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.07 (30%)  | 1829.57 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 1.07 (30%)  | 183.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 1.07 (30%)  | 183.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.06 (30%)  | 147.29 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.06 (30%)  | 19.29 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.02 (30%)  | 23.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 1.03 (30%)  | 19.29 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.07 (30%)  | 23.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x200, dense 20x2000 -> dense 200x20\")"]` | 1.07 (30%)  | 183.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 1.07 (30%)  | 1829.57 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.05 (30%)  | 19.29 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.06 (30%)  | 147.29 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x2000, dense 20x200 -> dense 2000x20\")"]` | 1.03 (30%)  | 183.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.07 (30%)  | 23.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x200, dense 200x20 -> dense 200x200\")"]` | 1.05 (30%)  | 19.29 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.05 (30%)  | 23.86 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.10 (30%)  | 1.16 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.17 (30%)  | 1.11 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.02 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.03 (30%)  | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 1.15 (30%)  | 1.85 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.18 (30%)  | 1.95 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.04 (30%)  | 1.09 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.06 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 1.17 (30%)  | 1.10 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.00 (30%)  | 1.05 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.07 (30%)  | 1.05 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 1.90 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.71 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 1.97 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.59 (40%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1"]` | 1.28 (15%) :x: | 1.20 (1%) :x: |
| `["string", "readuntil", "target length 1000"]` | 1.00 (15%)  | 1.29 (1%) :x: |
| `["string", "readuntil", "target length 2"]` | 1.20 (15%) :x: | 1.29 (1%) :x: |
| `["string", "readuntil", "target length 50000"]` | 1.00 (15%)  | 1.29 (1%) :x: |
| `["tuple", "linear algebra", "(\"matmat\", (4, 4), (4, 4))"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (4, 4), (4,))"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, false)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 1.27 (15%) :x: | 7.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 1.31 (15%) :x: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 1.19 (15%) :x: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 1.43 (15%) :x: | 4.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 1.34 (15%) :x: | 2.00 (1%) :x: |

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
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["micro"]`
- `["misc", "afoldl"]`
- `["misc", "bitshift"]`
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
- `["sparse", "transpose"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha.89
Commit 62b93bb (2018-06-12 07:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   27250994 s        276 s    2940192 s  630681961 s          6 s
       #2  3501 MHz  110379560 s          0 s    1558984 s  550683826 s          3 s
       #3  3501 MHz   14458310 s       2373 s    1251891 s  646586819 s          8 s
       #4  3501 MHz   13646905 s          0 s    1485649 s  647322915 s          5 s
       
  Memory: 31.383651733398438 GB (4712.25390625 MB free)
  Uptime: 6.629741e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.83
Commit 83ce7ba (2018-06-12 05:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   27369234 s        276 s    2952603 s  631682900 s          6 s
       #2  3501 MHz  111446105 s          0 s    1570662 s  550741375 s          3 s
       #3  3501 MHz   14575677 s       2373 s    1260909 s  647595739 s          8 s
       #4  3501 MHz   13764446 s          0 s    1494742 s  648331784 s          5 s
       
  Memory: 31.383651733398438 GB (4427.0546875 MB free)
  Uptime: 6.641105e6 sec
  Load Avg:  0.9453125  1.0078125  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
