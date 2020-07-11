# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8320fcc7d90ad2523a8f3a3410e7e2d6ac1aa1bf](https://github.com/JuliaLang/julia/commit/8320fcc7d90ad2523a8f3a3410e7e2d6ac1aa1bf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/8320fcc7d90ad2523a8f3a3410e7e2d6ac1aa1bf#commitcomment-40522226)

*Tag Predicate:* `ALL`

*Daily Job:* 2020-07-11 vs 2020-07-10

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
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 1.41 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"BitArray\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_load!"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "boolarray_bool_load!"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_load!"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 500)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "4467"]` | 0.08 (5%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Vector{Float64}\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Complex{Float64}\", \"Int\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "convert", "(\"Float64\", \"Int\")"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "convert", "(\"Int\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"UnitRange{Int64}\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Float32}\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Float64}\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Int64} == UnitRange{Int64}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Int64} == Vector{Int16}\")"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"UnitRange{Int64}\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Bool}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Float32}\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Float64}\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Int16}\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Int64} isequal UnitRange{Int64}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Int64} isequal Vector{Int16}\")"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Int64} isequal Vector{Int64}\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Int64}\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 2048)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 256)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 8)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reverse", "rev_loadmul_slow!"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 0.99 (5%)  | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 0.99 (5%)  | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 1.00 (5%)  | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"tup_tup\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 0.96 (5%)  | 1.10 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 0.94 (5%) :white_check_mark: | 1.14 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 0.96 (5%)  | 1.13 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "initialization", "(\"Vector\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Set\", \"Int\", \"iterate\")"]` | 2.56 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 3.96 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.54 (25%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["dates", "accessor", "day"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "accessor", "hour"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "accessor", "millisecond"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "accessor", "minute"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "accessor", "month"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "accessor", "second"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "accessor", "year"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Hour\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Millisecond\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Minute\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Month\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Second\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Year\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Year\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "construction", "Date"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "construction", "DateTime"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "conversion", "Date -> DateTime"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "conversion", "DateTime -> Date"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.36 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.01 (5%)  | 1.01 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "Date"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "DateTime"]` | 1.49 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitVector\", \"50-50\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Vector{Bool}\", \"10-90\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"Vector{Bool}\", \"50-50\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"Vector{Bool}\", \"90-10\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Vector{Float64}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"Vector{Bool}\", \"50-50\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Matrix{Float64}(10000, 10000)\")"]` | 0.99 (5%)  | 0.96 (1%) :white_check_mark: |
| `["io", "read", "read"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "read", "readstring"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["io", "skipchars"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["micro", "fib"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "18129"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "23042", "ComplexF32"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "allocation elision view", "conditional"]` | 0.60 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "no conditional"]` | 0.69 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "issue 12165", "Float16"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "issue 12165", "Float32"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "issue 12165", "Float64"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1, 1:1)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000, 1:1000)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.01 (5%)  | 0.99 (1%) :white_check_mark: |
| `["problem", "json", "parse_json"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"'a':'z'\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"'a':'z'\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 1.63 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"one\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"one\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"BigInt\")"]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"BigInt\")"]` | 0.51 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float64\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"negative argument\", \"Float32\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"negative argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"negative argument\", \"Float64\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"medium\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"medium\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"one\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"zero\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"zero\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"positive argument\", Float64)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow127\", \"negative argument\", Float32)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow127\", \"positive argument\", Float32)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"positive argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"one\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"one\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"zero\", \"Float32\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"zero\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float3\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"positive argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"zero\", \"Float32\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"zero\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2.0^-28\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2.0^-28\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"2f-12 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"zero\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float32\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 3.10 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 2.26 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 1000)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 2.99 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 2.30 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 3.34 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 1.94 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 2.98 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 3.02 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 10)"]` | 2.71 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 2.24 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 1.73 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 1.91 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"range\", 10)"]` | 2.57 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x50 -> dense 5x50\")"]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sparse", "sparse solves", "square system (lu), vector rhs"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (2, 2), (2, 2))"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (2, 2), (2,))"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (4, 4), (4,))"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "misc", "11899"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (2, 2))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (2,))"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4,))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (8,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (2, 2))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4,))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, ComplexF64, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.67 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, ComplexF64, (false, false))"]` | 0.66 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, ComplexF64, (true, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.69 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 1.47 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, false)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Float32, false)"]` | 0.66 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Float64, false)"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Int64, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, Float32}, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, Float64}, true)"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, BigFloat}, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 1.36 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, BigInt}, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Int64}, false)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Bool, false)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Bool}, true)"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Float32}, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Float64}, true)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Int64}, true)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Int8}, true)"]` | 1.16 (5%) :x: | 1.00 (1%)  |

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
- `["broadcast"]`
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
- `["io", "array_limit"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["io"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`
- `["micro"]`
- `["misc"]`
- `["misc", "23042"]`
- `["misc", "afoldl"]`
- `["misc", "allocation elision view"]`
- `["misc", "bitshift"]`
- `["misc", "issue 12165"]`
- `["misc", "iterators"]`
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
- `["sparse", "sparse matvec"]`
- `["sparse", "sparse solves"]`
- `["sparse", "transpose"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["string", "repeat"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "misc"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.6.0-DEV.425
Commit 8320fcc (2020-07-10 23:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  149459311 s       5056 s   16857368 s  7045977166 s         37 s
       #2  3501 MHz  1130622606 s        217 s   22692112 s  6069476987 s         28 s
       #3  3501 MHz  134696294 s       3321 s   10026290 s  7077500715 s         38 s
       #4  3501 MHz  126253476 s         43 s   14362235 s  7079967926 s         28 s
       
  Memory: 31.383651733398438 GB (19250.72265625 MB free)
  Uptime: 7.2285007e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
