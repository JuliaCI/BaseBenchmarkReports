# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c23b3e746c9f645f9674e021bbcab31a38c76977](https://github.com/JuliaLang/julia/commit/c23b3e746c9f645f9674e021bbcab31a38c76977) vs [JuliaLang/julia@ee4b18fd98d3e1a7ab394a88cbbae6f6953bbae6](https://github.com/JuliaLang/julia/commit/ee4b18fd98d3e1a7ab394a88cbbae6f6953bbae6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26795#issuecomment-388185720)

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
| `["array", "accumulate", "(\"accumulate!\", \"Float64\")"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 1.77 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float32,1}\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float64,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Int16,1}\")"]` | 1.59 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float32,1}\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float64,1}\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int16,1}\")"]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float64,1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int16,1}\")"]` | 1.59 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Bool}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"BitArray{2}\")"]` | 5.22 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcartesian_view\", \"BitArray{2}\")"]` | 5.93 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcolon_view\", \"1:100000\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"Array{Float32,2}\")"]` | 0.14 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"Array{Int32,2}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"BitArray{2}\")"]` | 2.47 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BitArray{2}\")"]` | 6.23 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 1.17 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumelt\", \"BitArray{2}\")"]` | 5.93 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumelt_boundscheck\", \"BitArray{2}\")"]` | 4.70 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear\", \"BitArray{2}\")"]` | 6.23 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 1.17 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.14 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumrange_view\", \"1:100000\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"Array{Float32,2}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"Array{Int32,2}\")"]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 2.05 (50%) :x: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.14 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.17 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.14 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.17 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"tup_tup\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"tup_tup\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"false\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"BitSet\")"]` | 2.69 (25%) :x: | 1.11 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Set\")"]` | 1.99 (25%) :x: | 1.11 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.90 (15%)  | 0.40 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.91 (15%)  | 0.68 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.90 (15%)  | 0.40 (1%) :white_check_mark: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.01 (15%)  | 1.03 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.99 (15%)  | 1.03 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.03 (15%)  | 1.01 (1%) :x: |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 1.45 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 1024)"]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 256)"]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 1024)"]` | 1.74 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 256)"]` | 2.33 (45%) :x: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.05 (15%)  | 1.07 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.05 (15%)  | 1.07 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.05 (15%)  | 1.03 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.05 (15%)  | 1.09 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.04 (15%)  | 1.07 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 0.89 (15%)  | 0.96 (1%) :white_check_mark: |
| `["problem", "raytrace", "raytrace"]` | 0.69 (15%) :white_check_mark: | 1.12 (1%) :x: |
| `["problem", "simplex", "simplex"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 0.84 (15%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.04 (25%)  | 0.80 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 1.04 (25%)  | 0.80 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 1.06 (25%)  | 0.80 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 1.05 (25%)  | 0.80 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 1.03 (25%)  | 0.80 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 1.01 (25%)  | 0.80 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 1.19 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 1.10 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 1.24 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 1.17 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.27 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.06 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 1.35 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.00 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 1.30 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 1.07 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 1.39 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 1.25 (25%)  | Inf (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967297)\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int128\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt128\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Int64}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 0.51 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 0.45 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigInt}\")"]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 2.30 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float32\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "meteor_contest"]` | 1.07 (15%)  | 1.18 (1%) :x: |
| `["shootout", "regex_dna"]` | 1.15 (15%) :x: | 1.65 (1%) :x: |
| `["shootout", "spectralnorm"]` | 1.00 (15%)  | 4.57 (1%) :x: |
| `["simd", "(\"two_reductions\", \"Int32\", 4095)"]` | 11.52 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int32\", 4096)"]` | 11.52 (20%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["string", "replace"]` | 1.79 (15%) :x: | 3.72 (1%) :x: |
| `["tuple", "linear algebra", "(\"matmat\", (2, 2), (2, 2))"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (2, 2), (2,))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (4, 4), (4,))"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 1.11 (15%)  | 1.08 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 1.14 (15%)  | 1.11 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 2.23 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 12.72 (15%) :x: | 26.99 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 3.00 (15%) :x: | 11.30 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 3.02 (15%) :x: | 11.30 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 4.38 (15%) :x: | 17.62 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 1.19 (15%) :x: | 5.50 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.18 (15%) :x: | 5.50 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 3.92 (15%) :x: | 9.66 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 1.15 (15%) :x: | 3.47 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 1.14 (15%)  | 3.47 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 4.86 (15%) :x: | 9.66 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 1.27 (15%) :x: | 3.47 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 1.26 (15%) :x: | 3.47 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 3.60 (15%) :x: | 7.35 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 1.28 (15%) :x: | 1.08 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.61 (15%) :x: | 1.24 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 5.40 (15%) :x: | 15.54 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 1.51 (15%) :x: | 5.94 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 4.76 (15%) :x: | 14.06 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 1.15 (15%)  | 4.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 4.16 (15%) :x: | 7.77 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 1.13 (15%)  | 2.65 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 5.51 (15%) :x: | 9.71 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 1.31 (15%) :x: | 3.47 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 4.71 (15%) :x: | 7.61 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 2.08 (15%) :x: | 1.95 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 2.00 (15%) :x: | 1.95 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 3.01 (15%) :x: | 3.45 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 3.16 (15%) :x: | 6.57 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 2.99 (15%) :x: | 3.89 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 3.12 (15%) :x: | 3.89 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 2.92 (15%) :x: | 7.61 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 5.64 (15%) :x: | 12.77 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 3.37 (15%) :x: | 5.99 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 4.17 (15%) :x: | 8.64 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 1.62 (15%) :x: | 4.07 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 3.74 (15%) :x: | 4.92 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.44 (15%) :x: | 2.66 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 6.70 (15%) :x: | 6.88 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 2.54 (15%) :x: | 3.50 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 6.69 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 2.22 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 0.45 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 1.83 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, false))"]` | 3.72 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, true))"]` | 3.02 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 3.11 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 12.97 (15%) :x: | 23.45 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 12.33 (15%) :x: | 21.23 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 12.35 (15%) :x: | 21.23 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, false))"]` | 3.47 (15%) :x: | 10.26 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 2.95 (15%) :x: | 9.34 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 2.98 (15%) :x: | 9.34 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 3.08 (15%) :x: | 6.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 2.64 (15%) :x: | 5.73 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 2.59 (15%) :x: | 5.73 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 4.35 (15%) :x: | 6.24 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, true))"]` | 3.75 (15%) :x: | 5.73 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 3.73 (15%) :x: | 5.73 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, false))"]` | 3.46 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 2.94 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 2.90 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 9.20 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 2.77 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 2.47 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 3.03 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, false)"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 4.28 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 3.74 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, false)"]` | 7.00 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 6.46 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float32, false)"]` | 5.61 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 4.84 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float64, false)"]` | 3.95 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 3.48 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Int64, false)"]` | 6.93 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Int64, true)"]` | 5.94 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 3.80 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 3.30 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.5061
Commit c23b3e7 (2018-05-10 21:04 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    4967431 s        248 s     962742 s  375819740 s          3 s
       #2  3501 MHz   32650834 s          0 s     573811 s  348765018 s          3 s
       #3  3501 MHz    4187839 s       2385 s     674528 s  377346453 s          6 s
       #4  3501 MHz    4144020 s          2 s     460516 s  377843481 s          1 s
       
  Memory: 31.383651733398438 GB (8534.47265625 MB free)
  Uptime: 3.826283e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.5057
Commit ee4b18f (2018-05-10 16:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    5092520 s        248 s     974515 s  376655162 s          3 s
       #2  3501 MHz   33551890 s          0 s     584340 s  348828730 s          3 s
       #3  3501 MHz    4305227 s       2385 s     682995 s  378195252 s          6 s
       #4  3501 MHz    4257310 s          2 s     468758 s  378697270 s          1 s
       
  Memory: 31.383651733398438 GB (8237.94921875 MB free)
  Uptime: 3.836042e6 sec
  Load Avg:  0.9970703125  1.01416015625  1.044921875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
