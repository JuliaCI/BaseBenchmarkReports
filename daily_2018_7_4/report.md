# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@60174a96f4708db7498625a3e99a10d966cc0001](https://github.com/JuliaLang/julia/commit/60174a96f4708db7498625a3e99a10d966cc0001)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/60174a96f4708db7498625a3e99a10d966cc0001#commitcomment-29589593)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-07-04 vs 2018-07-02

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
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 0.31 (15%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 0.05 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 0.05 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"next\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"next\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.06 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.06 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"true\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 2.44 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.44 (45%) :x: | 1.00 (1%)  |
| `["micro", "parseint"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["misc", "afoldl", "Complex{Float64}"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "afoldl", "Float64"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "afoldl", "Int"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "parse", "DateTime"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "parse", "Float64"]` | 0.50 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "parse", "Int"]` | 0.50 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Int64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"Float64\")"]` | 1.44 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"RandomDevice\", \"Float64\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{UInt64}\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 1.36 (20%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["string", "join"]` | 1.67 (40%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (16, 16), (16,))"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta.133
Commit 60174a9 (2018-07-03 20:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   38403568 s        278 s    4002444 s  806761097 s          8 s
       #2  3501 MHz  174468895 s          0 s    2455874 s  674350715 s          4 s
       #3  3501 MHz   23944421 s       2379 s    1981499 s  824962440 s         12 s
       #4  3501 MHz   22335890 s          0 s    2293889 s  826438511 s          8 s
       
  Memory: 31.383651733398438 GB (5106.72265625 MB free)
  Uptime: 8.51791e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
