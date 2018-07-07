# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6014e7d9ef4d540b645c9b0ddd05f2998a03b31c](https://github.com/JuliaLang/julia/commit/6014e7d9ef4d540b645c9b0ddd05f2998a03b31c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/6014e7d9ef4d540b645c9b0ddd05f2998a03b31c#commitcomment-29628242)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-07-07 vs 2018-07-06

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
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"Statistics.mean\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"overwrite\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"Vector\")"]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "Date"]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.40 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "sequences", "(\"randcycle\", \"MersenneTwister\", \"5\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float64\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float32\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float64\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float32\")"]` | 1.69 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"normal path -> small, k = -150\", \"Float32\")"]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"overflow\", \"Float32\")"]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float64\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4096)"]` | 1.90 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 2"]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 9.73 (15%) :x: | 9.98 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 9.65 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 9.71 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 9.92 (15%) :x: | 9.97 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 9.78 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 10.01 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 9.73 (15%) :x: | 4.13 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 10.05 (15%) :x: | 8.50 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 10.03 (15%) :x: | 8.50 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 9.80 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 10.16 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 10.03 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 9.69 (15%) :x: | 9.35 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 10.01 (15%) :x: | 9.44 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 10.02 (15%) :x: | 9.44 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 9.73 (15%) :x: | 9.70 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 10.06 (15%) :x: | 9.73 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 10.09 (15%) :x: | 9.73 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 9.78 (15%) :x: | 9.70 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 10.04 (15%) :x: | 9.73 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 10.01 (15%) :x: | 9.73 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 9.87 (15%) :x: | 8.47 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 10.02 (15%) :x: | 8.97 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 10.16 (15%) :x: | 8.97 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 9.64 (15%) :x: | 9.98 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 9.70 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 10.43 (15%) :x: | 10.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 10.37 (15%) :x: | 9.95 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 9.91 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 10.03 (15%) :x: | 8.65 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 9.93 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 9.96 (15%) :x: | 9.74 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 9.65 (15%) :x: | 9.44 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 9.85 (15%) :x: | 9.48 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 9.64 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 9.80 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 9.66 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 9.99 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 9.54 (15%) :x: | 8.78 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 9.90 (15%) :x: | 9.08 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 9.90 (15%) :x: | 9.77 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 9.90 (15%) :x: | 9.81 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 12.07 (15%) :x: | 9.77 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 10.63 (15%) :x: | 9.81 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 9.90 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 10.07 (15%) :x: | 8.65 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 10.29 (15%) :x: | 9.86 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 9.91 (15%) :x: | 9.86 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 9.67 (15%) :x: | 9.44 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 9.95 (15%) :x: | 9.48 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 9.64 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 9.80 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 10.36 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 9.95 (15%) :x: | 9.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 9.90 (15%) :x: | 8.78 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 9.98 (15%) :x: | 9.08 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 9.68 (15%) :x: | 9.99 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 9.63 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 9.87 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 10.03 (15%) :x: | 9.98 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 9.85 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 9.97 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 9.52 (15%) :x: | 9.00 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 10.24 (15%) :x: | 9.08 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 10.83 (15%) :x: | 9.08 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 9.56 (15%) :x: | 9.90 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 10.02 (15%) :x: | 9.91 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 9.82 (15%) :x: | 9.91 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 9.08 (15%) :x: | 9.54 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 10.24 (15%) :x: | 9.58 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 9.76 (15%) :x: | 9.58 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 9.27 (15%) :x: | 9.80 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 10.33 (15%) :x: | 9.81 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 9.84 (15%) :x: | 9.81 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 9.56 (15%) :x: | 9.80 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 10.39 (15%) :x: | 9.81 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 10.01 (15%) :x: | 9.81 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 9.56 (15%) :x: | 9.00 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 10.27 (15%) :x: | 9.08 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 10.92 (15%) :x: | 9.08 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 9.70 (15%) :x: | 9.99 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 9.59 (15%) :x: | 9.89 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 10.34 (15%) :x: | 10.03 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 10.20 (15%) :x: | 9.97 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 9.57 (15%) :x: | 9.23 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 11.07 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 9.74 (15%) :x: | 9.83 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 9.40 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 8.58 (15%) :x: | 9.60 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 9.32 (15%) :x: | 9.64 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 8.94 (15%) :x: | 9.83 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 9.87 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 8.96 (15%) :x: | 9.83 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 9.84 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 9.65 (15%) :x: | 9.23 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 9.81 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 10.86 (15%) :x: | 9.83 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 10.59 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 13.86 (15%) :x: | 9.83 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 11.93 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 9.59 (15%) :x: | 9.23 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 10.06 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 10.92 (15%) :x: | 9.92 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 9.98 (15%) :x: | 9.93 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 8.46 (15%) :x: | 9.60 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 9.91 (15%) :x: | 9.64 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 8.72 (15%) :x: | 9.83 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 9.71 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 8.69 (15%) :x: | 9.83 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 10.40 (15%) :x: | 9.84 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 9.59 (15%) :x: | 9.23 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 10.56 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 9.71 (15%) :x: | 9.96 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 9.51 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 9.58 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 10.12 (15%) :x: | 9.97 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 9.91 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (true, true))"]` | 10.17 (15%) :x: | 9.88 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, false))"]` | 9.24 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, true))"]` | 10.72 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 10.52 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 9.84 (15%) :x: | 9.95 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 10.71 (15%) :x: | 9.95 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 10.69 (15%) :x: | 9.95 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, false))"]` | 9.53 (15%) :x: | 9.67 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 10.76 (15%) :x: | 9.67 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 11.50 (15%) :x: | 9.67 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 9.66 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 9.75 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 11.13 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 9.73 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, true))"]` | 11.13 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 11.03 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, false))"]` | 9.25 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 10.59 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 11.33 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"BigFloat\")"]` | 9.60 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 11.85 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 11.36 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 11.50 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 12.52 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 12.44 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 10.62 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 11.93 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 10.82 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 10.84 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 10.88 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 10.82 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 9.44 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 9.52 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 9.24 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 9.40 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 9.40 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 9.07 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 9.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 9.62 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 9.42 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 9.00 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 9.34 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 9.35 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, false)"]` | 12.68 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 11.15 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 15.02 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 12.49 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 8.05 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 9.91 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 13.33 (15%) :x: | 9.95 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 12.13 (15%) :x: | 9.95 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 10.71 (15%) :x: | 9.67 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 13.84 (15%) :x: | 9.67 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 12.99 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 14.70 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int64, false)"]` | 13.76 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 13.62 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 8.19 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 11.61 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 10.76 (15%) :x: | 9.97 (1%) :x: |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 10.68 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 9.58 (15%) :x: | 10.07 (1%) :x: |
| `["union", "array", "(\"perf_sum2\", BigInt, true)"]` | 9.39 (15%) :x: | 10.02 (1%) :x: |
| `["union", "array", "(\"perf_sum2\", Bool, false)"]` | 9.80 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 21.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, false)"]` | 9.78 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 12.75 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, false)"]` | 9.86 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 17.15 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, false)"]` | 9.83 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 11.31 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, false)"]` | 9.54 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 9.52 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 9.69 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 11.97 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, false)"]` | 9.96 (15%) :x: | 9.97 (1%) :x: |
| `["union", "array", "(\"perf_sum3\", BigFloat, true)"]` | 10.32 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 9.61 (15%) :x: | 10.07 (1%) :x: |
| `["union", "array", "(\"perf_sum3\", BigInt, true)"]` | 9.36 (15%) :x: | 10.02 (1%) :x: |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 9.84 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 10.65 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, false)"]` | 9.83 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 15.73 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, false)"]` | 10.05 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 20.44 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, false)"]` | 10.04 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 20.36 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 10.06 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, true)"]` | 23.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 9.89 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 10.85 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 11.02 (15%) :x: | 9.99 (1%) :x: |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 10.62 (15%) :x: | 9.99 (1%) :x: |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 9.97 (15%) :x: | 10.04 (1%) :x: |
| `["union", "array", "(\"perf_sum4\", BigInt, true)"]` | 10.45 (15%) :x: | 10.08 (1%) :x: |
| `["union", "array", "(\"perf_sum4\", Bool, false)"]` | 9.62 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Bool, true)"]` | 9.65 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, false)"]` | 9.78 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 12.11 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float32, false)"]` | 8.51 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float32, true)"]` | 8.47 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float64, false)"]` | 9.10 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float64, true)"]` | 9.31 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int64, false)"]` | 9.14 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int64, true)"]` | 8.77 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 2.60 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 2.36 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 10.27 (15%) :x: | 9.97 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 10.00 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 9.47 (15%) :x: | 10.07 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 9.32 (15%) :x: | 10.02 (1%) :x: |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 9.80 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 13.11 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, false)"]` | 9.80 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 12.55 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, false)"]` | 9.86 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 16.13 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, false)"]` | 9.83 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 15.38 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int64, false)"]` | 9.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int64, true)"]` | 8.76 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 2.64 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 2.31 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, BigFloat, false)"]` | 9.77 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, BigFloat, true)"]` | 10.25 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, BigInt, false)"]` | 9.62 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, BigInt, true)"]` | 10.27 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Bool, false)"]` | 10.12 (15%) :x: | 13.84 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Bool, true)"]` | 10.56 (15%) :x: | 13.84 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 9.73 (15%) :x: | 15.78 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, true)"]` | 10.08 (15%) :x: | 15.78 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Float32, false)"]` | 9.37 (15%) :x: | 15.25 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Float32, true)"]` | 10.20 (15%) :x: | 15.25 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Float64, false)"]` | 9.71 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Float64, true)"]` | 9.99 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Int64, false)"]` | 9.71 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Int64, true)"]` | 10.12 (15%) :x: | 15.59 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Int8, false)"]` | 10.12 (15%) :x: | 13.84 (1%) :x: |
| `["union", "array", "(\"skipmissing\", collect, Int8, true)"]` | 10.52 (15%) :x: | 13.84 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 10.86 (15%) :x: | 10.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, true)"]` | 9.80 (15%) :x: | 9.91 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 10.05 (15%) :x: | 9.98 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigInt, true)"]` | 9.61 (15%) :x: | 9.97 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Bool, false)"]` | 9.84 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 12.57 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 4.43 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, true)"]` | 11.74 (15%) :x: | 7.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 15.53 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 1.59 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 12.51 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 11.75 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 3.26 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 9.24 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Int8, true)"]` | 2.96 (15%) :x: | 5.00 (1%) :x: |
| `["union", "array", "(\"sort\", BigFloat, false)"]` | 14.47 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"sort\", BigFloat, true)"]` | 14.30 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"sort\", BigInt, false)"]` | 16.14 (15%) :x: | 9.69 (1%) :x: |
| `["union", "array", "(\"sort\", BigInt, true)"]` | 15.91 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"sort\", Bool, false)"]` | 22.14 (15%) :x: | 8.68 (1%) :x: |
| `["union", "array", "(\"sort\", Bool, true)"]` | 17.99 (15%) :x: | 9.24 (1%) :x: |
| `["union", "array", "(\"sort\", Float32, false)"]` | 30.09 (15%) :x: | 9.63 (1%) :x: |
| `["union", "array", "(\"sort\", Float32, true)"]` | 16.08 (15%) :x: | 9.67 (1%) :x: |
| `["union", "array", "(\"sort\", Float64, false)"]` | 27.46 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"sort\", Float64, true)"]` | 14.79 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"sort\", Int64, false)"]` | 33.20 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"sort\", Int64, true)"]` | 16.03 (15%) :x: | 9.85 (1%) :x: |
| `["union", "array", "(\"sort\", Int8, false)"]` | 24.40 (15%) :x: | 9.35 (1%) :x: |
| `["union", "array", "(\"sort\", Int8, true)"]` | 14.70 (15%) :x: | 9.24 (1%) :x: |

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
Julia Version 0.7.0-beta.189
Commit 6014e7d (2018-07-07 02:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   40410261 s        278 s    4176427 s  830389304 s          8 s
       #2  3501 MHz  183580977 s          0 s    2623656 s  690930794 s          4 s
       #3  3501 MHz   25932949 s       2379 s    2130480 s  848670535 s         14 s
       #4  3501 MHz   24207749 s          0 s    2456194 s  850250438 s          8 s
       
  Memory: 31.383651733398438 GB (5028.515625 MB free)
  Uptime: 8.776716e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
