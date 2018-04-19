# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@14e9450796f66844debb8ccbc32ba94fac530fc2](https://github.com/JuliaLang/julia/commit/14e9450796f66844debb8ccbc32ba94fac530fc2) vs [JuliaLang/julia@50413a46a05b4f522e09fac2fb9b6a705cac31d7](https://github.com/JuliaLang/julia/commit/50413a46a05b4f522e09fac2fb9b6a705cac31d7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25377#issuecomment-382599915)

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
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 0.84 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 0.78 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.35 (15%) :x: | 1.03 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.34 (15%) :x: | 1.05 (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 271.92 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 4.37 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 2.49 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 4.26 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.58 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 2.80 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 0.99 (15%)  | Inf (1%) :x: |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.20 (15%) :x: | 1.02 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 10.04 (15%) :x: | 2.36 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 4.42 (15%) :x: | 2.00 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 6.18 (15%) :x: | 2.11 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 15.53 (15%) :x: | 25.00 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 14.95 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 17.46 (15%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 1.74 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"unspecified\")"]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 1024)"]` | 4.67 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 10.21 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 1024)"]` | 5.02 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 10.65 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 4.52 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 9.10 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 4.97 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 9.99 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 4.60 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 8.97 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 4.46 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 8.23 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 4.92 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 10.23 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 4.24 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 8.15 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 5.14 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 10.47 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 4.23 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 7.71 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 4.14 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 7.81 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 4.73 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 9.86 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 1024)"]` | 2.20 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 4.38 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 1024)"]` | 2.24 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 4.83 (45%) :x: | 1.16 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 1024)"]` | 2.31 (45%) :x: | 1.04 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 5.01 (45%) :x: | 1.16 (1%) :x: |
| `["problem", "go", "go_game"]` | 6.21 (15%) :x: | 7.58 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.18 (15%) :x: | 1.02 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.26 (15%) :x: | 1.02 (1%) :x: |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.30 (15%) :x: | 1.50 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"UInt64\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"UInt64\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 1.43 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2f0^-12 <= abs(x) < 1f0\", \"negative argument\", \"Float32\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 79.13 (15%) :x: | 68.66 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 1.01 (15%)  | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 1.55 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 1.58 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 1.02 (15%)  | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.55 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 1.55 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.28 (15%) :x: | 0.36 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 4.75 (15%) :x: | 0.81 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 4.71 (15%) :x: | 0.81 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 0.93 (15%)  | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 3.96 (15%) :x: | 0.96 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 3.99 (15%) :x: | 0.96 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 1.06 (15%)  | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 4.68 (15%) :x: | 0.89 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 4.83 (15%) :x: | 0.89 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.93 (15%)  | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 4.14 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 4.21 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 0.93 (15%)  | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 4.14 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 4.15 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 1.18 (15%) :x: | 0.53 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 5.02 (15%) :x: | 0.77 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 4.97 (15%) :x: | 0.77 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 2.10 (15%) :x: | 0.99 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.07 (15%)  | 0.97 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 2.28 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.65 (15%) :x: | 0.40 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 7.70 (15%) :x: | 0.85 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 1.18 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 5.33 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.44 (15%) :x: | 0.82 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 7.12 (15%) :x: | 0.91 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 1.18 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 5.82 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 1.18 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 5.83 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.53 (15%) :x: | 0.57 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 7.48 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 1.40 (15%) :x: | 0.90 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 5.75 (15%) :x: | 0.95 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 1.40 (15%) :x: | 0.90 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 5.73 (15%) :x: | 0.95 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.76 (15%) :x: | 0.40 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 7.54 (15%) :x: | 0.85 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.19 (15%) :x: | 0.94 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 5.32 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 1.45 (15%) :x: | 0.82 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 7.19 (15%) :x: | 0.91 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 1.13 (15%)  | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 6.04 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 1.17 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 5.63 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.51 (15%) :x: | 0.57 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 7.56 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, false)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.4941
Commit 14e9450 (2018-04-19 03:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    3997971 s        259 s     554104 s  189927637 s          2 s
       #2  3501 MHz   30772782 s          0 s     455702 s  163557630 s          0 s
       #3  3501 MHz    3526113 s       2368 s     358901 s  190659057 s          2 s
       #4  3501 MHz    3479240 s          0 s     456630 s  190772326 s          1 s
       
  Memory: 31.383651733398438 GB (15987.25390625 MB free)
  Uptime: 1.949105e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4898
Commit 50413a4 (2018-04-19 00:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    4114210 s        259 s     564218 s  190687297 s          2 s
       #2  3501 MHz   31581378 s          0 s     465239 s  163628174 s          0 s
       #3  3501 MHz    3615645 s       2368 s     366572 s  191449752 s          2 s
       #4  3501 MHz    3565306 s          0 s     464114 s  191567376 s          1 s
       
  Memory: 31.383651733398438 GB (15663.765625 MB free)
  Uptime: 1.957997e6 sec
  Load Avg:  1.0234375  1.02392578125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
