# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6a0089f8cfefe8c99613d39882a1c5c280fa1017](https://github.com/JuliaLang/julia/commit/6a0089f8cfefe8c99613d39882a1c5c280fa1017) vs [JuliaLang/julia@c7e4b9929b3b6ee89d47ce1320ef2de14c4ecf85](https://github.com/JuliaLang/julia/commit/c7e4b9929b3b6ee89d47ce1320ef2de14c4ecf85)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33753#issuecomment-549095501)

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
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 1.43 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 1.43 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"BitArray\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["array", "bool", "bitarray_bool_load!"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_fill!"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_fill!"]` | 10.24 (5%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_load!"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 500)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 500)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.56 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 8)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 8)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 256)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3darray\")"]` | 7.51 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"100000:-1:1\")"]` | 2245.05 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"1:100000\")"]` | 2566.07 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"Array{Float64,3}\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.24 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"1:100000\")"]` | 5.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float32,2}\")"]` | 8.10 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Int32,2}\")"]` | 5.23 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 9.95 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 9.97 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 7.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 5.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 7.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 5.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 13.15 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.60 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 8.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 5.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 14.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.62 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 5.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.91 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"100000:-1:1\")"]` | 13.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.38 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.24 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 4.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.91 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"100000:-1:1\")"]` | 2138.10 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"1:100000\")"]` | 3018.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"Array{Int32,2}\")"]` | 4.75 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 5.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 36.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.11 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.23 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"100000:-1:1\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"1:100000\")"]` | 5.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 64.77 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 70.76 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 7.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 5.38 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 7.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 5.35 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 1.22 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 13.14 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 8.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 14.38 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.90 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 4.47 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"100000:-1:1\")"]` | 2138.05 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"1:100000\")"]` | 3017.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"Array{Int32,2}\")"]` | 4.75 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 5.10 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 36.79 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"100000:-1:1\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"1:100000\")"]` | 5.14 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 66.76 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 72.20 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.11 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.12 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.11 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.12 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 1.22 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.07 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"100000:-1:1\")"]` | 5.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"1:100000\")"]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 1.53 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 1.51 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.71 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.59 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.41 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.39 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.41 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.44 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 1.00 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.73 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.03 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.46 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.24 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.18 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.76 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.84 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.84 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.04 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.47 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.24 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.14 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.61 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.86 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Float32,2}\")"]` | 1.21 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Int32,2}\")"]` | 1.20 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.17 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.15 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.16 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.16 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.17 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.17 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BitArray{2}\")"]` | 1.20 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.22 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.38 (50%)  | 1.04 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.19 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.07 (50%)  | 1.18 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.49 (50%)  | 1.14 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.17 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.17 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.21 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.37 (50%)  | 1.04 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.23 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.08 (50%)  | 1.18 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.11 (50%)  | 1.14 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.17 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.18 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumrange\", \"100000:-1:1\")"]` | 14.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"1:100000\")"]` | 2.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.90 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.16 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.89 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.19 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.12 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.05 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.92 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 1.11 (50%)  | 1.13 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 1.09 (50%)  | 1.13 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 1.50 (50%) :x: | 1.13 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 1.18 (50%)  | 1.13 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"Array{Float32,2}\")"]` | 1.31 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"Array{Int32,2}\")"]` | 1.35 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.32 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.34 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.20 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.22 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.35 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.36 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BitArray{2}\")"]` | 1.24 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.34 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.50 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.67 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.74 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.58 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.35 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.76 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.35 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.56 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.81 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.71 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.66 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.47 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.81 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 1.08 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1.0:1.0:100000.0\")"]` | 1.16 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"100000:-1:1\")"]` | 0.94 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1:100000\")"]` | 1.08 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"Array{Float32,2}\")"]` | 1.74 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"Array{Int32,2}\")"]` | 2.17 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.29 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.14 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.21 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.23 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.27 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.17 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 1.87 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.24 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.28 (50%)  | 1.30 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.25 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.54 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.24 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.26 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.21 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.42 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.35 (50%)  | 1.30 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.93 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.62 (50%) :x: | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.22 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.14 (50%)  | 1.99 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.21 (50%)  | 1.99 (1%) :x: |
| `["array", "reductions", "(\"maxabs\", \"Float64\")"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"maxabs\", \"Int64\")"]` | 1.80 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 6.87 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Int64\")"]` | 6.91 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"norminf\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"perf_mapreduce\", \"Int64\")"]` | 3.64 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"perf_reduce\", \"Int64\")"]` | 3.67 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 7.23 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 7.21 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 9.00 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs2\", \"Int64\")"]` | 2.75 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 6.89 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 5.59 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"gramschmidt!\", 100)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"gramschmidt!\", 1000)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"gramschmidt!\", 250)"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"gramschmidt!\", 500)"]` | 1.51 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.30 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.30 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.30 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "26942"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 10.25 (5%) :x: | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 1.98 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 2.27 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 1.79 (5%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.81 (5%) :x: | 3.50 (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 1.81 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 1.80 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((10000000,), 2)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.69 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"BitSet\", \"Int\", \"pop!\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"pop!\")"]` | 1.70 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 2.20 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter!\")"]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 1.75 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter!\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Bool\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Int8\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Nothing\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Bool\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Int8\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Nothing\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Bool\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Bool\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"pop!\", \"specified\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"specified\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"unspecified\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"unspecified\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"push!\", \"new\")"]` | 1.83 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Set\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"Set\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"Vector\")"]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Set\")"]` | 1.53 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Vector\")"]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.57 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.60 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"BitSet\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Set\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Vector\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.86 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Year\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["dates", "construction", "Date"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"50-50\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,1}(100000000,)\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 1.17 (5%) :x: | 1.14 (1%) :x: |
| `["io", "read", "read"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 4.72 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 2.67 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 1024)"]` | 1.73 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 1.49 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 5.10 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 2.82 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 5.08 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 2.85 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.67 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.75 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.97 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 2.70 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 1024)"]` | 1.98 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 256)"]` | 2.74 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.72 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.95 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 2.68 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.54 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.66 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.66 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.95 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 2.68 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 1024)"]` | 2.00 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 1.63 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.97 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 2.67 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 1.66 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.88 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.71 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.86 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.69 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 1024)"]` | 1.85 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 1.70 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"mul!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 1024)"]` | 1.74 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"mul!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 256)"]` | 1.77 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "axpy!"]` | 2.23 (40%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "scal!"]` | 2.03 (40%) :x: | 1.00 (1%)  |
| `["linalg", "small exp #29116"]` | 1.44 (5%) :x: | 2.06 (1%) :x: |
| `["micro", "parseint"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Complex{Float32}"]` | 1.66 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Complex{Float64}"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Float32"]` | 4.01 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Float64"]` | 1.91 (5%) :x: | 1.00 (1%)  |
| `["misc", "allocation elision view", "no conditional"]` | 7.77 (5%) :x: | Inf (1%) :x: |
| `["misc", "fastmath many args"]` | 1.48 (5%) :x: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000, 1:1000, 1:1000)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "perf highdim generator"]` | 1.40 (5%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 24, 1)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 3.36 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 2.07 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 2.61 (5%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 2.05 (5%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967295\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967297)\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float32\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float64\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"zero\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"1 <= abs(x) < 2\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"BigInt\")"]` | 1.43 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 2.04 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 3.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 3.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow127\", \"negative argument\", Float32)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 1.52 (40%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.85 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 2.00 (5%) :x: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 3.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 2.46 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 3.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 3.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 3.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 3.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 3.15 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 3.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"negative argument\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 3.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 2.31 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "k_nucleotide"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["shootout", "regex_dna"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Float32\", 4095)"]` | 5.57 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Float32\", 4096)"]` | 5.31 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Float64\", 4095)"]` | 2.87 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Float64\", 4096)"]` | 2.52 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Int32\", 4095)"]` | 6.07 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Int32\", 4096)"]` | 6.62 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Int64\", 4095)"]` | 1.85 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Int64\", 4096)"]` | 1.79 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Float32\", 4095)"]` | 6.97 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Float32\", 4096)"]` | 7.03 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Float64\", 4095)"]` | 3.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Float64\", 4096)"]` | 3.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int32\", 4095)"]` | 5.63 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int32\", 4096)"]` | 5.85 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int64\", 4095)"]` | 3.03 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int64\", 4096)"]` | 3.06 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_inner\", \"Int32\", 4095)"]` | 6.92 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_inner\", \"Int32\", 4096)"]` | 7.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_inner\", \"Int64\", 4095)"]` | 1.65 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_inner\", \"Int64\", 4096)"]` | 1.64 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4095)"]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4096)"]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_manual_example!\", \"Int32\", 4095)"]` | 5.55 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_manual_example!\", \"Int32\", 4096)"]` | 5.71 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_manual_example!\", \"Int64\", 4095)"]` | 2.63 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_manual_example!\", \"Int64\", 4096)"]` | 2.55 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_sum_reduce\", \"Int32\", 4095)"]` | 7.45 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_sum_reduce\", \"Int32\", 4096)"]` | 7.60 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_sum_reduce\", \"Int64\", 4095)"]` | 4.53 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_sum_reduce\", \"Int64\", 4096)"]` | 4.57 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_two_reductions\", \"Int64\", 4095)"]` | 3.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_two_reductions\", \"Int64\", 4096)"]` | 3.56 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 6.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 6.90 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4095)"]` | 3.07 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4096)"]` | 2.90 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4095)"]` | 7.00 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 7.48 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4095)"]` | 2.01 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4096)"]` | 1.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4095)"]` | 1.48 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4096)"]` | 1.48 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4095)"]` | 1.36 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4096)"]` | 1.36 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4095)"]` | 1.46 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4096)"]` | 1.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4095)"]` | 1.35 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4096)"]` | 1.34 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4095)"]` | 6.97 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4096)"]` | 7.03 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4095)"]` | 3.23 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4096)"]` | 3.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 5.67 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 5.72 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 3.06 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 3.04 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4095)"]` | 5.84 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4096)"]` | 5.84 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 3.03 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4096)"]` | 3.06 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float32\", 4095)"]` | 13.09 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float32\", 4096)"]` | 14.04 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float64\", 4095)"]` | 6.79 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float64\", 4096)"]` | 6.93 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int32\", 4095)"]` | 7.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int32\", 4096)"]` | 7.55 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int64\", 4095)"]` | 1.70 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int64\", 4096)"]` | 1.70 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Float32\", 4095)"]` | 20.23 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Float32\", 4096)"]` | 24.25 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Float64\", 4095)"]` | 8.33 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Float64\", 4096)"]` | 8.66 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Int32\", 4095)"]` | 8.19 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Int32\", 4096)"]` | 8.50 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Int64\", 4095)"]` | 1.66 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Int64\", 4096)"]` | 1.66 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.39 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.39 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.38 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.37 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.20 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.30 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.23 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.23 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float32\", 4095)"]` | 7.27 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float32\", 4096)"]` | 8.04 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float64\", 4095)"]` | 3.65 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float64\", 4096)"]` | 3.71 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int32\", 4095)"]` | 5.63 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int32\", 4096)"]` | 5.90 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int64\", 4095)"]` | 2.43 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int64\", 4096)"]` | 2.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int32\", 4095)"]` | 1.39 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int32\", 4096)"]` | 1.40 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int64\", 4095)"]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int64\", 4096)"]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float32\", 4095)"]` | 11.19 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float32\", 4096)"]` | 11.04 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float64\", 4095)"]` | 6.95 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float64\", 4096)"]` | 7.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 11.68 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 11.65 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4095)"]` | 7.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4096)"]` | 7.18 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float32\", 4095)"]` | 11.25 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float32\", 4096)"]` | 11.82 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float64\", 4095)"]` | 5.42 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float64\", 4096)"]` | 5.56 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int64\", 4095)"]` | 3.18 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int64\", 4096)"]` | 3.53 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float32\", 4095)"]` | 12.93 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float32\", 4096)"]` | 13.68 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float64\", 4095)"]` | 7.27 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float64\", 4096)"]` | 7.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int64\", 4095)"]` | 4.26 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int64\", 4096)"]` | 4.34 (20%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"ascending\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"descending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"ones\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort reverse\", \"ascending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort reverse\", \"descending\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort reverse\", \"ones\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort reverse\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 2.42 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"descending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ones\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 1.54 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ascending\")"]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"descending\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ones\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"random\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ascending\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"descending\")"]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ones\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"random\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.93 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 1.93 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort forwards\", \"ascending\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort forwards\", \"descending\")"]` | 1.74 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort forwards\", \"ones\")"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort reverse\", \"ascending\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort reverse\", \"descending\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort reverse\", \"ones\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! forwards\", \"ascending\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! forwards\", \"descending\")"]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! forwards\", \"ones\")"]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! reverse\", \"ascending\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! reverse\", \"descending\")"]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! reverse\", \"ones\")"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ascending\")"]` | 1.73 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"descending\")"]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ones\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ascending\")"]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"descending\")"]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ones\")"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.73 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"descending\")"]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ones\")"]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"random\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"descending\")"]` | 1.71 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ones\")"]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm forwards\", \"ascending\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm forwards\", \"descending\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm reverse\", \"ascending\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"descending\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"descending\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.67 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.49 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 1.30 (30%) :x: | 1.01 (1%)  |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"array\", 1000)"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 1.15 (30%)  | 1.01 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 1000)"]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.93 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x4000, dense 4000x40 -> dense 400x40\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x50 -> dense 5x50\")"]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x200, dense 200x200 -> dense 20x200\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x40, dense 400x40 -> dense 400x400\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 1.77 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 1.78 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x2000, dense 2000x20 -> dense 2000x20\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x200, dense 20x200 -> dense 200x200\")"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 2.00 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 2.14 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 2.03 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.90 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 2.21 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 2.22 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x2000, dense 20x200 -> dense 2000x20\")"]` | 1.54 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x200, dense 200x20 -> dense 200x200\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.77 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 2.05 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 2.00 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 2.05 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 2.02 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 1.73 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.76 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 1.76 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.78 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.76 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 1.73 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x4000, dense 40x400 -> dense 4000x40\")"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x400, dense 400x40 -> dense 400x400\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.71 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 1.71 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.74 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "sparse matvec", "adjoint"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["sparse", "sparse matvec", "non-adjoint"]` | 1.43 (5%) :x: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (default), matrix rhs"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (default), vector rhs"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (qr), matrix rhs"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 1.70 (5%) :x: | 1.00 (1%)  |
| `["string", "repeat", "repeat str len 16"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (16, 16), (16, 16))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (8, 8), (8, 8))"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4,))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.96 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 2.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 2.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 1.62 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 2.88 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 2.02 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 2.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 2.78 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 2.04 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 2.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 2.74 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 2.03 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 2.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 2.78 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 2.03 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 2.03 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.70 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 1.97 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 2.53 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 2.34 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 2.60 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 1.79 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 2.50 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 1.94 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 2.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 2.34 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.70 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 1.93 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.52 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 3.01 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 1.77 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 2.48 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 1.55 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 2.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 1.65 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 2.61 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 1.79 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 1.36 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 1.67 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 1.53 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 1.36 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.53 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 1.72 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 1.70 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 1.59 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 1.42 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 1.64 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, false))"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, true))"]` | 1.17 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 1.28 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, false))"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, false))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 1.99 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 2.02 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 2.02 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 1.99 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 2.01 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 1.98 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 1.96 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 1.97 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 1.99 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 2.02 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 1.97 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 2.02 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, false)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 1.48 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.36 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 1.30 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 1.47 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, false)"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, false)"]` | 1.51 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 3.59 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, false)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Bool, false)"]` | 2.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Bool, true)"]` | 2.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, false)"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float32, false)"]` | 4.67 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float32, true)"]` | 6.52 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float64, false)"]` | 3.91 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float64, true)"]` | 5.55 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int64, false)"]` | 3.01 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int64, true)"]` | 5.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 23.62 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 60.00 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int64, false)"]` | 3.02 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int64, true)"]` | 7.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 23.51 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 61.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, false)"]` | 3.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 10.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 6.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 6.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 6.46 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 1.48 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Complex{Float64}}, true)"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float32}, true)"]` | 1.45 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 1.48 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Int64}, true)"]` | 5.65 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Int8}, true)"]` | 4.26 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Bool}, false)"]` | 1.59 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Complex{Float64}}, false)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Float32}, false)"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Float64}, false)"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Int64}, false)"]` | 1.81 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Int8}, false)"]` | 1.58 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Bool, false)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Float32, false)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Float64, false)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Int64, false)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Int8, false)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Bool}, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Int64}, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Missing, Int8}, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Bool}, false)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Float32}, false)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Float64}, false)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Int64}, false)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Int8}, false)"]` | 1.31 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.4.0-DEV.430
Commit 6a0089f (2019-11-03 01:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  106581601 s       5044 s   12444093 s  4928358144 s         30 s
       #2  3501 MHz  753354894 s        214 s   13560688 s  4288207925 s         24 s
       #3  3501 MHz   90382122 s       3255 s    7385104 s  4957543463 s         34 s
       #4  3501 MHz   84730007 s         32 s   10540529 s  4957983211 s         23 s
       
  Memory: 31.383651733398438 GB (15065.9609375 MB free)
  Uptime: 5.0589449e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.427
Commit c7e4b99 (2019-11-02 09:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  106678431 s       5044 s   12452509 s  4929628431 s         30 s
       #2  3501 MHz  754659559 s        214 s   13585165 s  4288258848 s         24 s
       #3  3501 MHz   90487686 s       3255 s    7389716 s  4958812762 s         34 s
       #4  3501 MHz   84829776 s         32 s   10544977 s  4959258973 s         23 s
       
  Memory: 31.383651733398438 GB (15051.76953125 MB free)
  Uptime: 5.0603253e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
