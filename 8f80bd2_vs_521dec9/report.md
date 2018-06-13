# Benchmark Report

## Job Properties

*Commit(s):* [tkoolen/julia@8f80bd2a16950bb2f35fe470f780511bdf1b983a](https://github.com/tkoolen/julia/commit/8f80bd2a16950bb2f35fe470f780511bdf1b983a) vs [JuliaLang/julia@521dec9bf4990a0ec0fb827e1167e6c5195d392d](https://github.com/JuliaLang/julia/commit/521dec9bf4990a0ec0fb827e1167e6c5195d392d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27302#issuecomment-396681302)

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
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_load!"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"first\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["dates", "query", "(\"firstdayofmonth\", \"DateTime\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967295)\")"]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.90 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Int64\")"]` | 0.76 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"UInt64\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.80 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float32\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float64\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.75 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.56 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.85 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 0.69 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 0.69 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigInt\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.82 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigInt\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.82 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigFloat\")"]` | 0.92 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.71 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Int64\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"UInt64\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigFloat\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigInt\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float32\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float64\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"UInt64\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.83 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.73 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.71 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.79 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 0.75 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 0.74 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.60 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.85 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 0.74 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 0.74 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 0.75 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.80 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.76 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 0.89 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigInt\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.70 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 0.88 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigInt\")"]` | 0.79 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigFloat\")"]` | 0.90 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigInt\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigFloat\")"]` | 0.91 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigInt\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigFloat\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.50 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Int64\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"UInt64\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 0.68 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 0.67 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float32\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float64\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.64 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.67 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.57 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.57 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.65 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.57 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.62 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.61 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 0.68 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.61 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 0.68 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.58 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.57 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 0.79 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigInt\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigFloat\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigFloat\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.57 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 0.75 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.67 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.67 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.61 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.62 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Int64\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"UInt64\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float32\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float64\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.77 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.69 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.56 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 1.12 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.82 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.84 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.74 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 0.69 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.64 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.67 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.67 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigInt\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigInt\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigFloat\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Float32}\")"]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigFloat\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigFloat\")"]` | 0.72 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 0.69 (40%)  | 1.23 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigFloat\")"]` | 0.91 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigInt\")"]` | 0.80 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 0.65 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.66 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"BigFloat\")"]` | 0.83 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 0.62 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"BigFloat\")"]` | 0.78 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 0.67 (40%)  | 1.23 (1%) :x: |
| `["scalar", "floatexp", "(\"significand\", \"subnorm\", \"Float64\")"]` | 1.53 (40%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 0.75 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 0.86 (15%)  | 1.23 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 0.87 (15%)  | 1.23 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 0.66 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 0.78 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 0.72 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 0.74 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 0.75 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 0.60 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 0.62 (15%) :white_check_mark: | 1.23 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 0.71 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 0.72 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 0.73 (15%) :white_check_mark: | 1.25 (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"BigFloat\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 0.45 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.58 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 0.59 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 0.68 (15%) :white_check_mark: | 1.27 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, true)"]` | 0.70 (15%) :white_check_mark: | 1.27 (1%) :x: |

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
Julia Version 0.7.0-alpha.99
Commit 8f80bd2 (2018-06-12 20:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   11147653 s        256 s    2043559 s  653356490 s          5 s
       #2  3501 MHz   54747890 s          0 s     910689 s  612168713 s          4 s
       #3  3501 MHz    7407415 s       2388 s    1052562 s  659505661 s         10 s
       #4  3501 MHz    7178008 s          4 s     736314 s  660377568 s          2 s
       
  Memory: 31.383651733398438 GB (4828.5 MB free)
  Uptime: 6.685616e6 sec
  Load Avg:  0.94775390625  1.00830078125  1.0400390625
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
       #1  3501 MHz   11302618 s        256 s    2055793 s  654290079 s          5 s
       #2  3501 MHz   55755980 s          0 s     921779 s  612254271 s          4 s
       #3  3501 MHz    7525086 s       2388 s    1061931 s  660483036 s         10 s
       #4  3501 MHz    7283909 s          4 s     745194 s  661367386 s          2 s
       
  Memory: 31.383651733398438 GB (4872.7265625 MB free)
  Uptime: 6.69667e6 sec
  Load Avg:  0.97412109375  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
