# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@10443357f65438ec2cc935615eec3d3f7f189086](https://github.com/JuliaLang/julia/commit/10443357f65438ec2cc935615eec3d3f7f189086)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/10443357f65438ec2cc935615eec3d3f7f189086#commitcomment-26357746)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-12-19 vs 2017-12-11

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
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.24 (15%) :x: | 1.01 (1%) :x: |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 0.20 (15%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 0.00 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 0.00 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 0.00 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.86 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.86 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.90 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.85 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "sub2ind"]` | 381.80 (50%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.01 (15%)  | 0.96 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Month\")"]` | 0.99 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"DateTime\", \"Year\")"]` | 0.95 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"Date\", \"Year\")"]` | 0.96 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "construction", "Date"]` | 0.55 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "construction", "DateTime"]` | 0.56 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.11 (15%)  | 1.12 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 5.02 (15%) :x: | 8.50 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 8.72 (15%) :x: | 5.57 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 6.24 (15%) :x: | 3.13 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 8.64 (15%) :x: | 5.57 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.06 (15%)  | 1.11 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 22.08 (15%) :x: | 17.00 (1%) :x: |
| `["dates", "parse", "Date"]` | 32.77 (15%) :x: | 17.00 (1%) :x: |
| `["dates", "parse", "DateTime"]` | 7.10 (15%) :x: | 8.50 (1%) :x: |
| `["dates", "string", "DateTime"]` | 0.94 (15%)  | 0.97 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "(\"ispos\", \"Base.Generator{Array{Int8,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 1024)"]` | 1.05 (45%)  | 0.60 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 256)"]` | 1.01 (45%)  | 0.60 (1%) :white_check_mark: |
| `["micro", "parseint"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["micro", "randmatstat"]` | 0.96 (15%)  | 1.11 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.07 (15%)  | 1.03 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["misc", "parse", "DateTime"]` | 7.46 (15%) :x: | 8.45 (1%) :x: |
| `["misc", "parse", "Float64"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["misc", "parse", "Int"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.17 (15%) :x: | 1.20 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.17 (15%) :x: | 1.41 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.17 (15%) :x: | 1.08 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.17 (15%) :x: | 1.26 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.19 (15%) :x: | 1.39 (1%) :x: |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem", "json", "parse_json"]` | 4.69 (15%) :x: | 3.53 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.00 (15%)  | 0.95 (1%) :white_check_mark: |
| `["problem", "raytrace", "raytrace"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 2.18 (15%) :x: | 2.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large String\")"]` | 1.05 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small String\")"]` | 0.97 (25%)  | 0.78 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large String\")"]` | 1.05 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small String\")"]` | 0.98 (25%)  | 0.78 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large String\")"]` | 0.99 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small BitSet\")"]` | 28.13 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small String\")"]` | 0.97 (25%)  | 0.78 (1%) :white_check_mark: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 0.81 (25%)  | 0.93 (1%) :white_check_mark: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 0.94 (25%)  | 0.97 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 1.66 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.62 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 1.69 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 1.60 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551615\")"]` | 1.66 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:170141183460469231731687303715884105728\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551615\")"]` | 1.79 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 1.21 (25%)  | 0.17 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 1.13 (25%)  | 0.19 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.13 (25%)  | 0.17 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.90 (25%)  | 0.17 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.28 (25%) :x: | 0.84 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 0.94 (25%)  | 0.17 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967297)\")"]` | 1.18 (25%)  | 0.17 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967295)\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967297)\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:4294967297)\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967295)\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967297)\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967297)\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"ImplicitRNG\", \"Int64\")"]` | 0.97 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float16\")"]` | 1.04 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 0.94 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int128\")"]` | 0.98 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int16\")"]` | 0.87 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int32\")"]` | 0.94 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int64\")"]` | 0.97 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int8\")"]` | 0.88 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt128\")"]` | 0.99 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt16\")"]` | 0.93 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt32\")"]` | 0.93 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt64\")"]` | 0.96 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt8\")"]` | 0.76 (25%)  | 0.00 (1%) :white_check_mark: |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigInt\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Int64}\")"]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{UInt64}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Int64\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 2.10 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 2.05 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.19 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 2.10 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 2.22 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.18 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{UInt64}\")"]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigInt\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigInt}\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigInt\")"]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"UInt64\")"]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 2.26 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.57 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Int64\")"]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"UInt64\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigInt\")"]` | 2.24 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigInt\")"]` | 2.02 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigInt}\")"]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"BigInt\")"]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigInt\")"]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigInt}\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Int64}\")"]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{UInt64}\")"]` | 2.25 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Int64\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 2.02 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.13 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 2.32 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 2.18 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.45 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 1.85 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigInt}\")"]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 2.18 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 2.32 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 1.72 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 2.06 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 1.77 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.70 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigInt}\")"]` | 2.04 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"+\")"]` | 1.53 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"-\")"]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 2.46 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 2.30 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["shootout", "fannkuch"]` | 0.72 (15%) :white_check_mark: | 0.03 (1%) :white_check_mark: |
| `["shootout", "fasta"]` | 0.13 (15%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["sparse", "arithmetic", "(\"unary minus\", (20000, 20000))"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 0.42 (15%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 1.21 (30%)  | 1.16 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 1.00 (30%)  | 1.02 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 0.80 (30%)  | 1.11 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 0.83 (30%)  | 0.65 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 1.01 (30%)  | 1.01 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 0.99 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 0.97 (30%)  | 1.03 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 0.98 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 1.00 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 1.00 (30%)  | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 1.20 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 1.15 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 1.13 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.12 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.14 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.09 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x200, sparse 2000x200 -> dense 20x2000\")"]` | 1.09 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 1.11 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 200x2000 -> dense 20x200\")"]` | 1.09 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.04 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x40, sparse 400x40 -> dense 400x400\")"]` | 1.03 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.04 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.05 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.01 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 1.01 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.02 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 1.03 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.01 (30%)  | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 1.02 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x2000, dense 2000x20 -> dense 2000x20\")"]` | 1.02 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.02 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.03 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 1.07 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 1.00 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x200, dense 20x200 -> dense 200x200\")"]` | 1.03 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.07 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.01 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.01 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.11 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 1.10 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 1.10 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.12 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.10 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.10 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 1.13 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.15 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x200, dense 20x2000 -> dense 200x20\")"]` | 1.12 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 1.14 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.10 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.14 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x2000, dense 20x200 -> dense 2000x20\")"]` | 1.15 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.16 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x200, dense 200x20 -> dense 200x200\")"]` | 1.17 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.16 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 1.08 (30%)  | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.10 (30%)  | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 1.01 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 1.03 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.02 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 0.99 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.31 (30%) :x: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 1.01 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 1.02 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 1.03 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.02 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.01 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.02 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 1.03 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 1.01 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.04 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.04 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.01 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 1.03 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.04 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x400, dense 40x4000 -> dense 400x40\")"]` | 1.12 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 1.14 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.11 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 1.14 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x4000, dense 40x400 -> dense 4000x40\")"]` | 1.16 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 1.16 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x400, dense 400x40 -> dense 400x400\")"]` | 1.18 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 1.18 (30%)  | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.01 (30%)  | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 1.09 (30%)  | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.10 (30%)  | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 2.04 (40%) :x: | 1.00 (1%)  |
| `["string", "search", "Char"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["string", "searchindex", "Char"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["string", "searchindex", "String"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, BigFloat}Union{Void, BigFloat}\")"]` | 1.09 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, BigInt}Union{Void, BigInt}\")"]` | 1.00 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, Bool}Union{Void, Bool}\")"]` | 1.02 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, Complex{Float64}}Union{Void, Complex{Float64}}\")"]` | 1.01 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, Float32}Union{Void, Float32}\")"]` | 0.96 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, Float64}Union{Void, Float64}\")"]` | 1.03 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, Int64}Union{Void, Int64}\")"]` | 0.98 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Void, Int8}Union{Void, Int8}\")"]` | 1.04 (15%)  | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", \"Array{Union{Void, BigFloat},1}\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", \"Array{Union{Void, Int8},1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", \"Array{Union{Void, Complex{Float64}},1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |

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
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "cos"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "tan"]`
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
Julia Version 0.7.0-DEV.3095
Commit 1044335 (2017-12-19 01:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  108962438 s          0 s   19200079 s  4789011551 s        100 s
       #2  3501 MHz  461261817 s          0 s   12194522 s  4455239248 s         23 s
       #3  3501 MHz   91000484 s          0 s   10410137 s  4827775785 s         84 s
       #4  3501 MHz   87005548 s          0 s   10605910 s  4831564418 s         21 s
       
  Memory: 31.383651733398438 GB (2192.9765625 MB free)
  Uptime: 4.9315379e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
