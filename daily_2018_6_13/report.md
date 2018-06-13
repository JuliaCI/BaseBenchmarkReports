# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8c89802f1bad4b27f26dbff4e6488a93047885ac](https://github.com/JuliaLang/julia/commit/8c89802f1bad4b27f26dbff4e6488a93047885ac)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/8c89802f1bad4b27f26dbff4e6488a93047885ac#commitcomment-29342945)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-06-13 vs 2018-06-12

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
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Float64\", \"Int\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"getindex\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"getindex\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"in\", \"true\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.66 (45%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 0.97 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 0.96 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 0.95 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 0.97 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 0.90 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 0.93 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 0.77 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 0.80 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.86 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 0.86 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 0.90 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 0.86 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 0.67 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 0.86 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 0.76 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 0.76 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 0.75 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 0.80 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigFloat\")"]` | 0.64 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.66 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.64 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.64 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Int64\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"UInt64\")"]` | 0.75 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float32\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float64\")"]` | 0.65 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.66 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.74 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.90 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.77 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.64 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.65 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigInt\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigInt\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.79 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigFloat\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.79 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.73 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Int64\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"UInt64\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigFloat\")"]` | 0.79 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigInt\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.76 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.75 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float32\")"]` | 0.75 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float64\")"]` | 0.75 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"UInt64\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.55 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.72 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.71 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 0.71 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 0.71 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.61 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 0.71 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.66 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 0.76 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.81 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.76 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.73 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 0.90 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigInt\")"]` | 0.75 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.75 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.74 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 0.92 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigInt\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.75 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.75 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigFloat\")"]` | 0.85 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigInt\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigFloat\")"]` | 0.88 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigInt\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigFloat\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.90 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.90 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 1.00 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 1.01 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Int64\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"UInt64\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 0.72 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 0.73 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float32\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float64\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.76 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.76 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.90 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.90 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 2.44 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 0.74 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 0.76 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.90 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 0.73 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.75 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.65 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.87 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 0.73 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 2.45 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.43 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 1.00 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 0.74 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 1.02 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigInt\")"]` | 0.86 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 0.77 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigFloat\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.63 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.58 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Int64\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"UInt64\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float32\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float64\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.74 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.77 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.88 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.74 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.76 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 0.69 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigInt\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigInt\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigFloat\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigFloat\")"]` | 0.66 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 0.91 (40%)  | 1.23 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigFloat\")"]` | 0.81 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigInt\")"]` | 0.74 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 0.64 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.63 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"BigFloat\")"]` | 0.91 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 0.67 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 2.35 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigFloat\")"]` | 0.80 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 0.65 (40%)  | 1.23 (1%) :x: |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"+\")"]` | 1.67 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"-\")"]` | 1.64 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isequal\", \"BigFloat\")"]` | 1.76 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isequal\", \"Complex{BigFloat}\")"]` | 1.43 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{BigFloat}\")"]` | 1.61 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 1.96 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isless\", \"BigFloat\")"]` | 1.72 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isnan\", \"Complex{BigFloat}\")"]` | 1.67 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 0.56 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4096)"]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.49 (40%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 0.75 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 0.84 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 0.85 (15%)  | 1.23 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 0.67 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 0.81 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 0.20 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 0.20 (15%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 0.21 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 0.41 (15%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 0.39 (15%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 0.39 (15%) :white_check_mark: | 0.72 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.05 (15%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 0.06 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 0.07 (15%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 0.07 (15%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 0.05 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.05 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 0.04 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.05 (15%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 0.56 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 0.62 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 0.72 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 0.73 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 0.74 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"BigFloat\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.57 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 0.59 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 0.66 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, true)"]` | 0.66 (15%) :white_check_mark: | 1.27 (1%) :x: |

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
Julia Version 0.7.0-alpha.95
Commit 8c89802 (2018-06-13 03:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   28197914 s        276 s    3030628 s  637688789 s          6 s
       #2  3501 MHz  117819910 s          0 s    1643916 s  551230609 s          3 s
       #3  3501 MHz   15344920 s       2373 s    1321621 s  653699899 s          8 s
       #4  3501 MHz   14498194 s          0 s    1553564 s  654474586 s          6 s
       
  Memory: 31.383651733398438 GB (4034.1953125 MB free)
  Uptime: 6.710509e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
