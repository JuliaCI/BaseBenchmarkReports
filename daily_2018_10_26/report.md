# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ffaf849f36b9fd4f1c63b6fed4c56aca8a3f06af](https://github.com/JuliaLang/julia/commit/ffaf849f36b9fd4f1c63b6fed4c56aca8a3f06af)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ffaf849f36b9fd4f1c63b6fed4c56aca8a3f06af#commitcomment-31052763)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-10-26 vs 2018-10-24

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
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim2\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.66 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 8)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"1.0:1.0:100000.0\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"100000:-1:1\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"1:100000\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"Array{Float32,2}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"Array{Int32,2}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_fast!"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate second\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"getindex\")"]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"push!\", \"new\")"]` | 1.61 (25%) :x: | 1.00 (1%)  |
| `["dates", "accessor", "second"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["dates", "query", "(\"daysofweekinmonth\", \"Date\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"deserialize\", \"Matrix{Float64}\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["io", "serialization", "(\"deserialize\", \"Vector{String}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["io", "skipchars"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 1.75 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 1.77 (45%) :x: | 1.00 (1%)  |
| `["micro", "printfd"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["micro", "randmatmul"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "18129"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Float64"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["problem", "simplex", "simplex"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["problem", "stockcorr", "stockcorr"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt16\", \"RangeGenerator(1:1)\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"Float64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigInt\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.50 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow127\", \"negative argument\", Float32)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "13786"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 2.08 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["shootout", "meteor_contest"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["shootout", "pidigits"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 1000)"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint\", (20000, 20000))"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.85 (40%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (2, 2))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 1.42 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Bool, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Float32, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Int64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |

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
- `["io"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["micro"]`
- `["misc"]`
- `["misc", "23042"]`
- `["misc", "afoldl"]`
- `["misc", "bitshift"]`
- `["misc", "issue 12165"]`
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
- `["tuple", "misc"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-DEV.552
Commit ffaf849 (2018-10-25 23:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   57676718 s       5003 s    6337590 s  1768190131 s         21 s
       #2  3501 MHz  303418090 s        203 s    4847635 s  1527108566 s         14 s
       #3  3501 MHz   42149300 s       3206 s    3608183 s  1789617257 s         24 s
       #4  3501 MHz   39062216 s          0 s    4468404 s  1791556127 s         14 s
       
  Memory: 31.383651733398438 GB (4827.61328125 MB free)
  Uptime: 1.8369694e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
