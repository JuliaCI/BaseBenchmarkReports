# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@296d5728a2974ac1e3efaf358288c40b05e3abee](https://github.com/JuliaLang/julia/commit/296d5728a2974ac1e3efaf358288c40b05e3abee)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/296d5728a2974ac1e3efaf358288c40b05e3abee#commitcomment-27120315)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-01-26 vs 2018-01-25

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
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 2048)"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"100000:-1:1\")"]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"pop!\", \"unspecified\")"]` | 1.96 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"'a':'z'\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large BitSet\")"]` | 1.45 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Vector\")"]` | 1.63 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small BitSet\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Vector\")"]` | 1.63 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float64\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 0.64 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.82 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.79 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.79 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 0.63 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 0.73 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 0.65 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.66 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.83 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.64 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.74 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.81 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.84 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.85 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.84 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 0.69 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 0.79 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 0.34 (50%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 0.56 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 0.52 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.78 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.74 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.74 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.72 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.85 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.39 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.64 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.70 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.66 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.73 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.79 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.73 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.67 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 0.78 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.86 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.92 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 0.83 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.92 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.86 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 0.40 (50%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.50 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.66 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.61 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 0.60 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 0.71 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 0.40 (50%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.46 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"UInt64\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.45 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.56 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.67 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.69 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.67 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.51 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.54 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.64 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.65 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 0.71 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 0.88 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 0.58 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.71 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.82 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 0.69 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 0.68 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 0.63 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.78 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.64 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.75 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.72 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.70 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.77 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.76 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.92 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 0.64 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.80 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 0.69 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.78 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Float64}\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.68 (40%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "floatexp", "(\"ldexp\", \"inf -> inf\", \"Float32\")"]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3580
Commit 296d572 (2018-01-26 00:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  115503869 s          0 s   20342491 s  5108558205 s        101 s
       #2  3501 MHz  495471912 s          0 s   12777738 s  4748506839 s         25 s
       #3  3501 MHz   95325600 s          0 s   10889860 s  5151055692 s         85 s
       #4  3501 MHz   91193110 s          0 s   11077015 s  5154997665 s         22 s
       
  Memory: 31.383651733398438 GB (4942.8671875 MB free)
  Uptime: 5.2597541e7 sec
  Load Avg:  0.88916015625  0.9814453125  1.03466796875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
