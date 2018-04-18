# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@beba563aa2360944cd61aa9ecd68d8fef2658172](https://github.com/JuliaLang/julia/commit/beba563aa2360944cd61aa9ecd68d8fef2658172) vs [JuliaLang/julia@8e7034e5c96d5bb9ffb9d1780f15d25338802ca7](https://github.com/JuliaLang/julia/commit/8e7034e5c96d5bb9ffb9d1780f15d25338802ca7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25261#issuecomment-382477789)

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
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.84 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1} generator\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Vector{Bool}\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.82 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1} generator\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1}\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 1.98 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Vector{Bool}\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_fill!"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_fill!"]` | 8.64 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_load!"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 500)"]` | 34.01 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 52.25 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 46.04 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 102.64 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 39.60 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 90.47 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 37.63 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 89.49 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 7.06 (15%) :x: | 1.17 (1%) :x: |
| `["array", "cat", "(\"vcat\", 500)"]` | 92.51 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 46.16 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 93.47 (15%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Complex{Float64}\", \"Int\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Float64\", \"Int\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Bool}\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 2.83 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcolon\", \"100000:-1:1\")"]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"1:100000\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Float32,2}\")"]` | 2.03 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Int32,2}\")"]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 3.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.69 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.22 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.76 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"100000:-1:1\")"]` | 2380.24 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"1:100000\")"]` | 6410.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"Array{Int32,2}\")"]` | 4.24 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 4.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 5.82 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 9.10 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"1:100000\")"]` | 1710.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"Array{Int32,2}\")"]` | 7.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Int32,2}\")"]` | 6.43 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"100000:-1:1\")"]` | 2479.42 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"1:100000\")"]` | 6838.20 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"Array{Int32,2}\")"]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 5.92 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 9.15 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"100000:-1:1\")"]` | 1.90 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"1:100000\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Float32,2}\")"]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Int32,2}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 3.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.49 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.45 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.46 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.90 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norm1\", \"Int64\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 5.32 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 5.54 (15%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 0.95 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 0.94 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 0.92 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.93 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 0.95 (15%)  | 1.18 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 0.98 (15%)  | 0.88 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 0.94 (15%)  | 0.89 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.76 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 0.92 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 0.93 (15%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter!\")"]` | 1.60 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter\")"]` | 1.43 (25%) :x: | 2.56 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 8.47 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"pop!\")"]` | 42.81 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter!\")"]` | 1.34 (25%) :x: | 2.00 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter\")"]` | 1.20 (25%)  | 1.56 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 32.34 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter!\")"]` | 6.62 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 6.21 (25%) :x: | 3.49 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 40.98 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 50.96 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter!\")"]` | 1.28 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 1.25 (25%)  | 3.34 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 39.76 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 53.75 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter\")"]` | 24.91 (25%) :x: | 7.02 (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter!\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.65 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter\")"]` | 1.38 (25%) :x: | 2.90 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 2.39 (25%) :x: | 1.45 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\")"]` | 2.75 (25%) :x: | 1.49 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 2.97 (25%) :x: | 1.53 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"iterator\")"]` | 1.26 (25%) :x: | 1.34 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\")"]` | 1.26 (25%) :x: | 1.34 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\", \"sizehint!\")"]` | 1.28 (25%) :x: | 1.36 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 3.02 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 2.83 (25%) :x: | 1.63 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 3.02 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"iterator\")"]` | 1.24 (25%)  | 1.68 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\")"]` | 1.23 (25%)  | 1.63 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\", \"sizehint!\")"]` | 1.24 (25%)  | 1.68 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\")"]` | 14.45 (25%) :x: | 3.87 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\", \"sizehint!\")"]` | 15.92 (25%) :x: | 6.56 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\")"]` | 1.46 (25%) :x: | 2.86 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\", \"sizehint!\")"]` | 1.47 (25%) :x: | 4.75 (1%) :x: |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 59.18 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"next\")"]` | 1.29 (25%) :x: | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"start\")"]` | 718.79 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"start\")"]` | 755.36 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"next\")"]` | 1.25 (25%)  | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"start\")"]` | 753.79 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"next\")"]` | 3.56 (25%) :x: | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"start\")"]` | 651.81 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"start\")"]` | 627.25 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"next\")"]` | 1.33 (25%) :x: | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"start\")"]` | 621.13 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"next\")"]` | 3.13 (25%) :x: | 3.50 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"start\")"]` | 283.85 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"start\")"]` | 260.38 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"next\")"]` | 1.39 (25%) :x: | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"start\")"]` | 259.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 1.24 (25%)  | 1.86 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"first\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 2.83 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"first\")"]` | 1.45 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"unspecified\")"]` | 1.68 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"false\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"unspecified\")"]` | 1.02 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 7.86 (25%) :x: | 4.23 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 7.84 (25%) :x: | 3.22 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 4.84 (25%) :x: | 2001.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 4.10 (25%) :x: | 1793.00 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 0.89 (25%)  | 0.78 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.96 (25%)  | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 1.04 (25%)  | 1.55 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 1.06 (25%)  | 1.48 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.08 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.14 (25%)  | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.52 (25%) :x: | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.60 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.68 (25%) :x: | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.85 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Vector\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.08 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.05 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.19 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 1.03 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"BitSet\")"]` | 2.09 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Set\")"]` | 1.63 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.05 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.05 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.01 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.53 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"empty\", \"Int\", \"<\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"empty\", \"Int\", \"⊆\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.47 (15%) :x: | 1.43 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 101.49 (15%) :x: | Inf (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 54.38 (15%) :x: | 15.10 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 37.52 (15%) :x: | 8.30 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 56.71 (15%) :x: | 15.10 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.23 (15%) :x: | 1.42 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 66.41 (15%) :x: | Inf (1%) :x: |
| `["dates", "parse", "Date"]` | 97.03 (15%) :x: | Inf (1%) :x: |
| `["dates", "parse", "DateTime"]` | 129.17 (15%) :x: | Inf (1%) :x: |
| `["dates", "string", "Date"]` | 1.44 (15%) :x: | 2.17 (1%) :x: |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 2.65 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 3.33 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Int8,1}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 0.99 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 0.85 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 0.93 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.02 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 0.84 (45%)  | 1.01 (1%) :x: |
| `["linalg", "blas", "axpy!"]` | 2.09 (40%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "scal!"]` | 1.95 (40%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 1024)"]` | 5.06 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 256)"]` | 13.16 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 1.15 (45%)  | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 1.13 (45%)  | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 1024)"]` | 1.14 (45%)  | 1.08 (1%) :x: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 256)"]` | 1.13 (45%)  | 1.09 (1%) :x: |
| `["micro", "parseint"]` | 1.17 (15%) :x: | 1.12 (1%) :x: |
| `["micro", "randmatstat"]` | 2.16 (15%) :x: | 1.00 (1%)  |
| `["misc", "afoldl", "Complex{Float64}"]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["misc", "afoldl", "Float64"]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["misc", "afoldl", "Int"]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 18.73 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 26.13 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 35.60 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 19.60 (15%) :x: | 1.00 (1%)  |
| `["misc", "parse", "DateTime"]` | 39.96 (15%) :x: | 55.80 (1%) :x: |
| `["misc", "parse", "Float64"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["misc", "parse", "Int"]` | 25.68 (15%) :x: | 47.32 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.10 (15%)  | 1.05 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.11 (15%)  | 1.09 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.08 (15%)  | 1.02 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.09 (15%)  | 1.06 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.09 (15%)  | 1.08 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 3.11 (15%) :x: | 3.94 (1%) :x: |
| `["problem", "json", "parse_json"]` | 1.32 (15%) :x: | 1.18 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 7.17 (15%) :x: | 9.71 (1%) :x: |
| `["problem", "simplex", "simplex"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 2.73 (15%) :x: | 1.96 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:1)\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> norm\", \"Float32\")"]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "iteration", "in"]` | 14171.91 (25%) :x: | 1.00 (1%)  |
| `["scalar", "iteration", "indexed"]` | 56684.28 (25%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float32\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["shootout", "fasta"]` | 1.04 (15%)  | 1.01 (1%) :x: |
| `["shootout", "k_nucleotide"]` | 2.83 (15%) :x: | 2.26 (1%) :x: |
| `["shootout", "mandelbrot"]` | 1.00 (15%)  | 1.05 (1%) :x: |
| `["shootout", "meteor_contest"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["shootout", "nbody"]` | 1.30 (15%) :x: | 358.50 (1%) :x: |
| `["shootout", "nbody_vec"]` | 1.13 (15%)  | 2.41 (1%) :x: |
| `["sort", "issorted", "(\"forwards\", \"ascending\")"]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 2.05 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 1.10 (15%)  | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 1.14 (15%)  | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 1.12 (15%)  | 1.06 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 1.99 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x50 -> dense 5x50\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["string", "join"]` | 1.59 (40%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (8, 8))"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.04 (15%)  | 1.07 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 1.04 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 1.07 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 1.05 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 1.02 (15%)  | 1.03 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 1.03 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 1.05 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.05 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 1.05 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.15 (15%) :x: | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.09 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.10 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 4.49 (15%) :x: | 3.24 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 4.46 (15%) :x: | 3.28 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 4.52 (15%) :x: | 3.31 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 4.48 (15%) :x: | 3.76 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 4.52 (15%) :x: | 3.75 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 4.54 (15%) :x: | 3.79 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 6.90 (15%) :x: | 23.37 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 7.06 (15%) :x: | 20.56 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 7.13 (15%) :x: | 22.03 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 6.41 (15%) :x: | 4.59 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 6.00 (15%) :x: | 4.30 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 6.36 (15%) :x: | 4.35 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 6.89 (15%) :x: | 7.32 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 6.42 (15%) :x: | 7.03 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 6.83 (15%) :x: | 7.22 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 6.61 (15%) :x: | 6.25 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 6.52 (15%) :x: | 5.88 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 6.50 (15%) :x: | 5.98 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 6.25 (15%) :x: | 6.25 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 6.23 (15%) :x: | 5.88 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 6.25 (15%) :x: | 5.98 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 7.04 (15%) :x: | 23.37 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 6.97 (15%) :x: | 20.56 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 7.02 (15%) :x: | 22.03 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 7.93 (15%) :x: | 1.91 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 7.05 (15%) :x: | 1.88 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 10.43 (15%) :x: | 3.75 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 8.75 (15%) :x: | 3.25 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 97.74 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 38.33 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 47.24 (15%) :x: | 23.49 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 28.71 (15%) :x: | 10.86 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 96.84 (15%) :x: | 37.15 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 36.51 (15%) :x: | 16.12 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 76.16 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 35.05 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 100.71 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 36.96 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 97.90 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 36.74 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 66.62 (15%) :x: | 11.73 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 27.42 (15%) :x: | 6.17 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 60.66 (15%) :x: | 11.73 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 26.67 (15%) :x: | 6.17 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 98.87 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 38.34 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 46.90 (15%) :x: | 14.34 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 26.41 (15%) :x: | 7.00 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 85.65 (15%) :x: | 37.15 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 37.36 (15%) :x: | 16.12 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 81.28 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 35.28 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 106.51 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 35.60 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 106.69 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 37.26 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 134.44 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 124.06 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 104.77 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 104.62 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 105.08 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 86.59 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 103.68 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 75.48 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 98.71 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 87.36 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 109.45 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 80.66 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 111.74 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 88.86 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 103.25 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 85.78 (15%) :x: | Inf (1%) :x: |

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
Julia Version 0.7.0-DEV.4898
Commit beba563 (2018-04-18 17:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    3785826 s        259 s     532653 s  186753016 s          2 s
       #2  3501 MHz   29105583 s          0 s     435579 s  161829358 s          0 s
       #3  3501 MHz    3350452 s       2368 s     342476 s  187438892 s          2 s
       #4  3501 MHz    3291463 s          0 s     439700 s  187561872 s          1 s
       
  Memory: 31.383651733398438 GB (16721.0 MB free)
  Uptime: 1.914928e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4895
Commit 8e7034e (2018-04-18 16:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    3901490 s        259 s     542615 s  187518151 s          2 s
       #2  3501 MHz   29923336 s          0 s     445038 s  161895650 s          0 s
       #3  3501 MHz    3436608 s       2368 s     350220 s  188237697 s          2 s
       #4  3501 MHz    3376209 s          0 s     447301 s  188362947 s          1 s
       
  Memory: 31.383651733398438 GB (15684.41015625 MB free)
  Uptime: 1.923868e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
