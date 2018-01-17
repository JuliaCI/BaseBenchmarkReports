# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d6f079a483e2f6a2867e8a5f1709103205841f8a](https://github.com/JuliaLang/julia/commit/d6f079a483e2f6a2867e8a5f1709103205841f8a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/d6f079a483e2f6a2867e8a5f1709103205841f8a#commitcomment-26903779)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-01-17 vs 2018-01-11

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
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"BitArray\")"]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["find", "(\"Array{Bool,1}\", \"50-50\")"]` | 11.60 (15%) :x: | 2.40 (1%) :x: |
| `["find", "(\"Base.Generator{Array{Bool,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##3#6\\\"))}\", \"50-50\")"]` | 9.70 (15%) :x: | 2.40 (1%) :x: |
| `["find", "(\"Base.Generator{BitArray{1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##3#6\\\"))}\", \"10-90\")"]` | 21.61 (15%) :x: | 5.98 (1%) :x: |
| `["find", "(\"Base.Generator{BitArray{1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##3#6\\\"))}\", \"90-10\")"]` | 6.58 (15%) :x: | 1.72 (1%) :x: |
| `["find", "(\"BitArray{1}\", \"10-90\")"]` | 73.04 (15%) :x: | 14.73 (1%) :x: |
| `["find", "(\"BitArray{1}\", \"50-50\")"]` | 58.13 (15%) :x: | 3.94 (1%) :x: |
| `["find", "(\"BitArray{1}\", \"90-10\")"]` | 52.37 (15%) :x: | 2.66 (1%) :x: |
| `["find", "(\"ispos\", \"Array{Bool,1}\")"]` | 24.32 (15%) :x: | 2.49 (1%) :x: |
| `["find", "(\"ispos\", \"Array{Float32,1}\")"]` | 15.85 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Array{Float64,1}\")"]` | 15.48 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Array{Int64,1}\")"]` | 20.82 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Array{Int8,1}\")"]` | 22.85 (15%) :x: | 2.50 (1%) :x: |
| `["find", "(\"ispos\", \"Array{UInt64,1}\")"]` | 16.08 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Array{UInt8,1}\")"]` | 15.95 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Bool,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 20.08 (15%) :x: | 2.49 (1%) :x: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Float32,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 13.36 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Float64,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 12.90 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Int64,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 18.69 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Int8,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 20.99 (15%) :x: | 2.50 (1%) :x: |
| `["find", "(\"ispos\", \"Base.Generator{Array{UInt64,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 13.68 (15%) :x: | 1.77 (1%) :x: |
| `["find", "(\"ispos\", \"Base.Generator{Array{UInt8,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 13.47 (15%) :x: | 1.77 (1%) :x: |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"10-90\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"90-10\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 0.89 (15%)  | 0.50 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 0.50 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 0.93 (15%)  | 0.65 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 2.73 (15%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"one\", \"Float32\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"UInt64\")"]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 2.21 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 2.18 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 2.23 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 2.18 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "regex_dna"]` | 0.80 (15%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 0.98 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.00 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.01 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 0.71 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x400, dense 400x40 -> dense 4000x40\")"]` | 0.92 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 0.97 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x40, dense 40x400 -> dense 400x400\")"]` | 0.91 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 0.99 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x4000, dense 4000x40 -> dense 400x40\")"]` | 0.99 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 0.98 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 0.99 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 0.93 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 0.97 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 0.90 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 0.83 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.05 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x200, sparse 2000x200 -> dense 20x2000\")"]` | 0.96 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 0.97 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 200x2000 -> dense 20x200\")"]` | 0.91 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x20, dense 20x20 -> dense 2000x20\")"]` | 0.95 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x200, dense 20x200 -> dense 2000x20\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x20, dense 200x20 -> dense 200x200\")"]` | 0.95 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x2000, dense 20x2000 -> dense 200x20\")"]` | 0.97 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 0.94 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x200, dense 200x200 -> dense 20x200\")"]` | 0.96 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 0.88 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 0.88 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.86 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.38 (30%) :white_check_mark: | 0.70 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.98 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 0.94 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.93 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.66 (30%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 0.49 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 0.84 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 0.98 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 0.38 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.76 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 0.85 (30%)  | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 0.45 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 0.29 (30%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x40, sparse 400x40 -> dense 400x400\")"]` | 1.12 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 0.90 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.42 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 1.15 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.00 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 0.87 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 53.58 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x400, dense 40x400 -> dense 4000x40\")"]` | 150.42 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 184.57 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x40, dense 400x40 -> dense 400x400\")"]` | 17.46 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 19.14 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x4000, dense 40x4000 -> dense 400x40\")"]` | 19.97 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 2.39 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 2.14 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 4.76 (30%) :x: | 4.59 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 4.43 (30%) :x: | 6.26 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 5.53 (30%) :x: | 5.97 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.44 (30%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 14.98 (30%) :x: | 7.09 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 17.61 (30%) :x: | 6.84 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 39.73 (30%) :x: | 6.94 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 3.09 (30%) :x: | 1.57 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 0.81 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 4.86 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 31.50 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 0.56 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 2.25 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 3.49 (30%) :x: | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 0.49 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 0.27 (30%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 0.97 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 0.94 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 1.01 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 0.99 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.01 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 0.97 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 0.96 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 0.98 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x2000, dense 2000x20 -> dense 2000x20\")"]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 0.12 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 0.02 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 0.14 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x200, dense 20x200 -> dense 200x200\")"]` | 0.05 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 0.03 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.87 (30%)  | 0.73 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.96 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 0.95 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.54 (30%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.93 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 0.95 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 0.90 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.90 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 0.02 (30%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 0.01 (30%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 0.13 (30%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.04 (30%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 0.02 (30%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 0.21 (30%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 0.10 (30%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 0.08 (30%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 0.97 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 0.91 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 0.96 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 0.90 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 0.82 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.04 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 0.96 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 0.92 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x200, dense 20x2000 -> dense 200x20\")"]` | 0.97 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 0.97 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 0.95 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 0.90 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x2000, dense 20x200 -> dense 2000x20\")"]` | 0.91 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 0.95 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x200, dense 200x20 -> dense 200x200\")"]` | 0.85 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 0.86 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.93 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.67 (30%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 0.94 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.87 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.39 (30%) :white_check_mark: | 0.70 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.99 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 0.88 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.89 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 0.79 (30%)  | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 0.92 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 0.32 (30%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.71 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 0.68 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 0.49 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 0.38 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 0.45 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 4.50 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 4.53 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 4.68 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 5.20 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 5.44 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 6.85 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 8.72 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 7.12 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 0.68 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 0.86 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 0.58 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 0.78 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.65 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 0.76 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 1.70 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 3.22 (30%) :x: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 7.38 (30%) :x: | 1.55 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 62.85 (30%) :x: | 6.93 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 16.36 (30%) :x: | 6.83 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.09 (30%)  | 1.31 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 12.40 (30%) :x: | 2.95 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 10.98 (30%) :x: | 7.08 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 6.84 (30%) :x: | 3.10 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 5.73 (30%) :x: | 4.58 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 0.19 (30%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 0.34 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 0.19 (30%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.33 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 0.20 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 0.34 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 0.20 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 0.17 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.00 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 0.86 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 1.15 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 0.89 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.41 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 1.11 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.99 (30%)  | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x400, dense 40x4000 -> dense 400x40\")"]` | 22.36 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 186.37 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 2.55 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 19.33 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x4000, dense 40x400 -> dense 4000x40\")"]` | 140.38 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 2.41 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x400, dense 400x40 -> dense 400x400\")"]` | 16.52 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 47.48 (30%) :x: | 0.03 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 39.79 (30%) :x: | 6.94 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 3.08 (30%) :x: | 1.57 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 17.31 (30%) :x: | 6.84 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 5.42 (30%) :x: | 5.97 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.43 (30%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 15.18 (30%) :x: | 7.09 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 4.35 (30%) :x: | 6.26 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 4.72 (30%) :x: | 4.59 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 4.57 (30%) :x: | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 32.87 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 0.29 (30%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 2.24 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 4.10 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 0.49 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 0.55 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 0.70 (30%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["string", "join"]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["string", "replace"]` | 0.86 (15%)  | 2.10 (1%) :x: |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, BigFloat}Union{Nothing, BigFloat}\")"]` | 1.05 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, BigInt}Union{Nothing, BigInt}\")"]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, Bool}Union{Nothing, Bool}\")"]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, Complex{Float64}}Union{Nothing, Complex{Float64}}\")"]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, Float32}Union{Nothing, Float32}\")"]` | 0.94 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, Float64}Union{Nothing, Float64}\")"]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, Int64}Union{Nothing, Int64}\")"]` | 1.02 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, Int8}Union{Nothing, Int8}\")"]` | 0.96 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countnothing\", \"Array{Union{Nothing, BigFloat},1}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

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
- `["find"]`
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
- `["scalar", "cos"]`
- `["scalar", "cosh"]`
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
- `["string"]`
- `["string", "readuntil"]`
- `["string", "search"]`
- `["string", "searchindex"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3429
Commit d6f079a (2018-01-17 04:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  114332159 s          0 s   20113525 s  5033220579 s        100 s
       #2  3501 MHz  487431966 s          0 s   12655120 s  4679755198 s         24 s
       #3  3501 MHz   94417387 s          0 s   10778817 s  5075159731 s         84 s
       #4  3501 MHz   90399394 s          0 s   10978660 s  5078966631 s         21 s
       
  Memory: 31.383651733398438 GB (4624.1171875 MB free)
  Uptime: 5.1827997e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
