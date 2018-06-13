# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@547ecd5821f465ffebc3d7a26a27573f36bd2132](https://github.com/JuliaLang/julia/commit/547ecd5821f465ffebc3d7a26a27573f36bd2132) vs [JuliaLang/julia@521dec9bf4990a0ec0fb827e1167e6c5195d392d](https://github.com/JuliaLang/julia/commit/521dec9bf4990a0ec0fb827e1167e6c5195d392d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27495#issuecomment-396648326)

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
| `["array", "bool", "boolarray_true_load!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3darray\")"]` | 5.79 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "2d"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 1.44 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"mean\", \"Int64\")"]` | 1.54 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 1.35 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 1.48 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 9.24 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs2\", \"Int64\")"]` | 3.03 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 1.39 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 1.30 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 4.06 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 3.47 (15%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["problem", "ziggurat", "ziggurat"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Int64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.81 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Int64\")"]` | 0.79 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"UInt64\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.80 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float32\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float64\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.80 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.93 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigInt\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigInt\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigFloat\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.84 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigFloat\")"]` | 0.91 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 0.89 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.76 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.61 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.75 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 0.86 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Int64\")"]` | 0.87 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"UInt64\")"]` | 0.88 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigInt\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.74 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float32\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float64\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 0.77 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"UInt64\")"]` | 0.78 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.83 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.73 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.75 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.76 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 0.75 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 0.75 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 0.73 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.84 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 0.73 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 0.75 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.61 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.76 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.75 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.76 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 0.89 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigInt\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.75 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 0.89 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigInt\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.73 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigFloat\")"]` | 0.89 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigInt\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigFloat\")"]` | 0.89 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigInt\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigFloat\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 0.75 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 0.79 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 0.78 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Int64\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"UInt64\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 0.75 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 0.67 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 0.67 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float32\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float64\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.57 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.57 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.61 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.61 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 0.67 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.61 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 0.67 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.61 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.57 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Float32\")"]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 0.78 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigInt\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigFloat\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigFloat\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.67 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.66 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.66 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.61 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.61 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Int64\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"UInt64\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float32\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float64\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.72 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.77 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.82 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.61 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.61 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.61 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.67 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.67 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigInt\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigInt\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigFloat\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigFloat\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"positive argument\", \"Float32\")"]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"zero\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigFloat\")"]` | 0.74 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 0.70 (40%)  | 1.23 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigFloat\")"]` | 0.92 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigInt\")"]` | 0.80 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 0.63 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.69 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"BigFloat\")"]` | 0.83 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 0.62 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"BigFloat\")"]` | 0.48 (40%) :white_check_mark: | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 0.65 (40%)  | 1.23 (1%) :x: |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 0.74 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 0.82 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 0.84 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 0.62 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 0.80 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 0.71 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 0.75 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 0.76 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 0.58 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 0.61 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 0.72 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 0.72 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 0.75 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.58 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 0.58 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 0.65 (15%) :white_check_mark: | 1.27 (1%) :x: |
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
Julia Version 0.7.0-alpha.96
Commit 547ecd5 (2018-06-12 19:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   27764665 s        276 s    2989832 s  634711077 s          6 s
       #2  3501 MHz  114620364 s          0 s    1604764 s  551006444 s          3 s
       #3  3501 MHz   14953534 s       2373 s    1289026 s  650662317 s          8 s
       #4  3501 MHz   14138433 s          0 s    1522077 s  651403582 s          6 s
       
  Memory: 31.383651733398438 GB (5108.578125 MB free)
  Uptime: 6.675857e6 sec
  Load Avg:  1.0458984375  1.02783203125  1.04736328125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.88
Commit 521dec9 (2018-06-12 14:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   27916867 s        276 s    3002226 s  635677545 s          6 s
       #2  3501 MHz  115651721 s          0 s    1615920 s  551098691 s          3 s
       #3  3501 MHz   15074352 s       2373 s    1298315 s  651666549 s          8 s
       #4  3501 MHz   14250939 s          0 s    1531333 s  652416486 s          6 s
       
  Memory: 31.383651733398438 GB (4815.453125 MB free)
  Uptime: 6.687212e6 sec
  Load Avg:  0.97509765625  1.0  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
