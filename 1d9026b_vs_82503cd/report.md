# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1d9026b554367dba8eb7c678e6e9f7beb8fc27ac](https://github.com/JuliaLang/julia/commit/1d9026b554367dba8eb7c678e6e9f7beb8fc27ac) vs [JuliaLang/julia@82503cd16c95626c900924bcf004ca642c66ec45](https://github.com/JuliaLang/julia/commit/82503cd16c95626c900924bcf004ca642c66ec45)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/1d9026b554367dba8eb7c678e6e9f7beb8fc27ac#commitcomment-30643470)

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
| `["array", "bool", "boolarray_true_load!"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 0.87 (5%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 500)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "convert", "(\"Complex{Float64}\", \"Int\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 2048)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 256)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 4.34 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 4.17 (50%) :x: | 1.40 (1%) :x: |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"tup_tup\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Set\", \"Int\", \"iterate\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"big\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Vector\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"deserialize\", \"Matrix{Float64}\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "fib"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "23042", "Float32"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "23042", "Float64"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 24, 1)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "stockcorr", "stockcorr"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt8\", \"RangeGenerator(1:1)\")"]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Float64\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 3.15 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 3.15 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 2.31 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 2.31 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 1.62 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 2.46 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 1.85 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 1.77 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{Float64}\")"]` | 2.38 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Float64}\")"]` | 2.46 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Int64}\")"]` | 3.23 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{UInt64}\")"]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Float32}\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Float64}\")"]` | 2.38 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Int64}\")"]` | 3.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{UInt64}\")"]` | 3.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float64\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float32\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float64\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.92 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.92 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 2.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 2.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 2.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 2.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 3.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.47 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"div\", \"Complex{Int64}\")"]` | 1.77 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"div\", \"Complex{UInt64}\")"]` | 1.85 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float32\")"]` | 1.92 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float32\")"]` | 1.92 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float32\")"]` | 1.69 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float32\")"]` | 1.85 (40%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.00 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 3.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 3.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 1.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 2.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 3.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 3.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 3.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 3.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 1.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 3.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 1.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 3.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["shootout", "meteor_contest"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "pidigits"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.52 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (16, 16), (16, 16))"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (2, 2))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 1.43 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigFloat, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.1.0-DEV.321
Commit 1d9026b (2018-09-25 18:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   51371010 s       5000 s    5637426 s  1513400542 s         21 s
       #2  3501 MHz  252905920 s        203 s    3963032 s  1316279778 s         11 s
       #3  3501 MHz   35767993 s       3200 s    3137809 s  1534245961 s         22 s
       #4  3501 MHz   33251811 s          0 s    3860840 s  1535823917 s         11 s
       
  Memory: 31.383651733398438 GB (4842.34765625 MB free)
  Uptime: 1.5745301e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.320
Commit 82503cd (2018-09-25 07:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   51489246 s       5000 s    5648065 s  1514531151 s         21 s
       #2  3501 MHz  254063504 s        203 s    3979091 s  1316369284 s         11 s
       #3  3501 MHz   35894515 s       3200 s    3144936 s  1535374698 s         22 s
       #4  3501 MHz   33361399 s          0 s    3867802 s  1536970628 s         11 s
       
  Memory: 31.383651733398438 GB (4324.875 MB free)
  Uptime: 1.575794e7 sec
  Load Avg:  0.97412109375  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
