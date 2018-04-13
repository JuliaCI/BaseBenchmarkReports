# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8ac77cc1731ece63d3fb0192ff77c4438c9c3ddd](https://github.com/JuliaLang/julia/commit/8ac77cc1731ece63d3fb0192ff77c4438c9c3ddd) vs [JuliaLang/julia@3666ffad817cfca8539afc589d4a8daa8c6db7cf](https://github.com/JuliaLang/julia/commit/3666ffad817cfca8539afc589d4a8daa8c6db7cf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26795#issuecomment-380930600)

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
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim2\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_fill!"]` | 1.88 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_fill!"]` | 11.22 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 500)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float32,1}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Int16,1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float32,1}\")"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float64,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int16,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float64,1}\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int16,1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Bool}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3darray\")"]` | 8.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 3.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"100000:-1:1\")"]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"Array{Int32,2}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 2.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"BitArray{2}\")"]` | 7.46 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.56 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 5.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.72 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 5.68 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.17 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"100000:-1:1\")"]` | 50600.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"1:100000\")"]` | 4024.29 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float32,2}\")"]` | 8.33 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Int32,2}\")"]` | 6.46 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 8.46 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 9.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 8.38 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 9.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 8.40 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 9.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"BitArray{2}\")"]` | 8.79 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 16.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 12.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 6.38 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 21.69 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.82 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 3.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 20.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 18.86 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 4.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 8.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 22.02 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 5.12 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"100000:-1:1\")"]` | 23.05 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"1:100000\")"]` | 2.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Float32,2}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Int32,2}\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.85 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.41 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.91 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.35 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.89 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BitArray{2}\")"]` | 3.35 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.03 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"100000:-1:1\")"]` | 3562.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"1:100000\")"]` | 5699.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"Array{Int32,2}\")"]` | 4.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 5.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BitArray{2}\")"]` | 12.67 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 4.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.19 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 12.21 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 75.06 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.68 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.72 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"100000:-1:1\")"]` | 49311.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"1:100000\")"]` | 4526.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 7.87 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 14.07 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 8.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 9.41 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 8.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 9.41 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 1.25 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.91 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 12.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.09 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 7.05 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 3.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 18.15 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 3.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 9.60 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 18.87 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.97 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 7.22 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.69 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 20.93 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 5.40 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"BitArray{2}\")"]` | 11.55 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.02 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.05 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.06 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"BitArray{2}\")"]` | 6.05 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"100000:-1:1\")"]` | 3562.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"1:100000\")"]` | 5343.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 5.08 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BitArray{2}\")"]` | 12.13 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 4.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 12.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 75.77 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"100000:-1:1\")"]` | 48055.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"1:100000\")"]` | 4526.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 7.56 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 13.42 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.12 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.11 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.12 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.11 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 1.24 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.94 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.19 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.29 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 7.66 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.22 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.17 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.19 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.13 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 9.78 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.20 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.82 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 7.81 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.24 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.17 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.19 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"100000:-1:1\")"]` | 4.17 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"1:100000\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 1.40 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 1.38 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.76 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.75 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.37 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.44 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.40 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.39 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 1.13 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.61 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.91 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.74 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.22 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.14 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.63 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.47 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.60 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.99 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.76 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.26 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.17 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.64 (50%) :x: | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.47 (50%)  | 1.05 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Float32,2}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Int32,2}\")"]` | 1.10 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.10 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.14 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.10 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.10 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"BitArray{2}\")"]` | 1.14 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.10 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.38 (50%)  | 1.04 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.06 (50%)  | 1.14 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.08 (50%)  | 1.14 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.37 (50%)  | 1.04 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.16 (50%)  | 1.14 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.07 (50%)  | 1.14 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.09 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.11 (50%)  | 1.03 (1%) :x: |
| `["array", "index", "(\"sumrange\", \"100000:-1:1\")"]` | 23.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"1:100000\")"]` | 3.07 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Float32,2}\")"]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Int32,2}\")"]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.72 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 2.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 4.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.97 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 4.11 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.90 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 3.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 1.14 (50%)  | 1.10 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 1.14 (50%)  | 1.10 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 1.55 (50%) :x: | 1.11 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 1.19 (50%)  | 1.11 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"Array{Float32,2}\")"]` | 1.22 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"Array{Int32,2}\")"]` | 1.28 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.46 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.44 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.22 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.25 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.24 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.26 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"BitArray{2}\")"]` | 1.46 (50%)  | 1.25 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.52 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.85 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.78 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.99 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.97 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.42 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.71 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.44 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.73 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.72 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.96 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.93 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.39 (50%)  | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.75 (50%) :x: | 1.29 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 1.04 (50%)  | 1.13 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1.0:1.0:100000.0\")"]` | 0.98 (50%)  | 1.13 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"100000:-1:1\")"]` | 1.27 (50%)  | 1.13 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1:100000\")"]` | 1.06 (50%)  | 1.14 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"Array{Float32,2}\")"]` | 1.70 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"Array{Int32,2}\")"]` | 1.76 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.30 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.13 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.12 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.31 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.23 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.23 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 2.79 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.03 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.35 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.08 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.04 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.27 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.26 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.19 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.92 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.25 (50%)  | 1.20 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.61 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.12 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.24 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.23 (50%)  | 1.40 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.11 (50%)  | 1.40 (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 4.36 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 4.05 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"maxabs\", \"Int64\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 7.52 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Int64\")"]` | 9.98 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 7.84 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 10.43 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 6.41 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs2\", \"Int64\")"]` | 3.45 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 8.09 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 7.13 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"var\", \"Float64\")"]` | 7.69 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"var\", \"Int64\")"]` | 2.26 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 2.59 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 3.31 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.88 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 2.27 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.94 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 6.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 5.84 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 3.65 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 2.74 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 1.62 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((10000000,), 2)"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 0.98 (15%)  | 0.91 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 1.00 (15%)  | 0.88 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 0.98 (15%)  | 0.89 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.76 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 0.88 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 0.85 (15%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Bool\")"]` | 1.90 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Int8\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Nothing\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Bool\")"]` | 1.84 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Int8\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Nothing\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Bool\")"]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Int8\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Bool\")"]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Int8\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"in\", \"true\")"]` | 2.35 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"specified\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"specified\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 1.63 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 1.63 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"BitSet\")"]` | 3.08 (25%) :x: | 1.11 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Set\")"]` | 1.97 (25%) :x: | 1.11 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"Set\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Vector\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Set\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Vector\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.60 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"BitSet\")"]` | 1.69 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"Vector\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.06 (15%)  | 1.13 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.52 (15%) :x: | 1.20 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 1.46 (15%) :x: | 1.11 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.52 (15%) :x: | 1.20 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.03 (15%)  | 1.11 (1%) :x: |
| `["dates", "string", "DateTime"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.83 (15%) :x: | 1.02 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{Float32,1}\")"]` | 2.32 (15%) :x: | 1.01 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Float64,1}\")"]` | 2.23 (15%) :x: | 1.01 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.59 (15%) :x: | 1.01 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Int8,1}\")"]` | 1.94 (15%) :x: | 1.02 (1%) :x: |
| `["find", "findall", "(\"ispos\", \"Array{UInt64,1}\")"]` | 2.33 (15%) :x: | 1.01 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{UInt8,1}\")"]` | 2.44 (15%) :x: | 1.01 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"90-10\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 1024)"]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 2.06 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 1024)"]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.54 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.81 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.78 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 2.43 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 1024)"]` | 1.77 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 256)"]` | 2.45 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 1.54 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.76 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 2.45 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 1.73 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.72 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.63 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.72 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.77 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 2.43 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 1024)"]` | 1.77 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 256)"]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.75 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 1.74 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.88 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.71 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.85 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.80 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 1024)"]` | 1.84 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 1.76 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 1024)"]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "axpy!"]` | 2.52 (40%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "scal!"]` | 2.32 (40%) :x: | 1.00 (1%)  |
| `["misc", "parse", "Float64"]` | 1.54 (15%) :x: | 3.67 (1%) :x: |
| `["misc", "parse", "Int"]` | 1.56 (15%) :x: | 2.31 (1%) :x: |
| `["misc", "repeat", "(200, 1, 24)"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 5.13 (15%) :x: | 1.13 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 5.24 (15%) :x: | 1.11 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 4.82 (15%) :x: | 1.06 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 5.17 (15%) :x: | 1.12 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 5.24 (15%) :x: | 1.11 (1%) :x: |
| `["problem", "go", "go_game"]` | 1.25 (15%) :x: | 1.94 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 1.32 (15%) :x: | 1.06 (1%) :x: |
| `["problem", "json", "parse_json"]` | 1.87 (15%) :x: | 1.13 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 2.18 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 1.06 (15%)  | 1.34 (1%) :x: |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 5.27 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 2.97 (15%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 1.18 (15%) :x: | 1.10 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.03 (25%)  | 0.75 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 1.01 (25%)  | 0.75 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 1.02 (25%)  | 0.75 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 1.02 (25%)  | 0.75 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 1.06 (25%)  | 0.75 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 1.02 (25%)  | 0.75 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 1.15 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 1.13 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 1.36 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 1.06 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.20 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.09 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 1.30 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.27 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 1.14 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 1.11 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 1.32 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 1.00 (25%)  | Inf (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 1.15 (25%)  | 1.04 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 1.04 (25%)  | 1.01 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:2^10000\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt8\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"ImplicitRNG\", \"Float64\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"ImplicitRNG\", \"Float64\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Int64\")"]` | 1.78 (40%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"negative argument\", \"Float32\")"]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> norm\", \"Float64\")"]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"Int64\", \"-\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"UInt64\", \"+\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"UInt64\", \"-\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["scalar", "iteration", "indexed"]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 1.91 (40%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2.0^-28\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"negative argument\", \"Float32\")"]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["shootout", "pidigits"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout", "regex_dna"]` | 1.35 (15%) :x: | 1.26 (1%) :x: |
| `["shootout", "spectralnorm"]` | 1.00 (15%)  | 4.58 (1%) :x: |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 14.82 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 15.63 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4095)"]` | 5.80 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4096)"]` | 5.78 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4095)"]` | 12.88 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 13.18 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4095)"]` | 2.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4096)"]` | 2.33 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4095)"]` | 6.99 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4096)"]` | 7.06 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4095)"]` | 3.54 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4096)"]` | 3.57 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 7.63 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 7.80 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 3.54 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 3.55 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float32\", 4095)"]` | 13.08 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float32\", 4096)"]` | 15.76 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float64\", 4095)"]` | 6.48 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float64\", 4096)"]` | 6.61 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int32\", 4095)"]` | 11.95 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int32\", 4096)"]` | 12.36 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int64\", 4095)"]` | 1.91 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Int64\", 4096)"]` | 1.91 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 16.18 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 16.91 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 17.17 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 18.25 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 6.51 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 6.71 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 6.69 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 6.98 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 15.97 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 16.04 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 15.57 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 15.85 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.85 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.82 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.82 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.86 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float32\", 4095)"]` | 10.30 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float32\", 4096)"]` | 10.80 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float64\", 4095)"]` | 6.24 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float64\", 4096)"]` | 6.29 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int32\", 4095)"]` | 12.08 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int32\", 4096)"]` | 12.19 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int64\", 4095)"]` | 3.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int64\", 4096)"]` | 3.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float32\", 4095)"]` | 10.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float32\", 4096)"]` | 10.34 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float64\", 4095)"]` | 8.79 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float64\", 4096)"]` | 8.53 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 19.37 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 18.37 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4095)"]` | 11.17 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4096)"]` | 11.92 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float32\", 4095)"]` | 12.87 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float32\", 4096)"]` | 13.54 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float64\", 4095)"]` | 7.37 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float64\", 4096)"]` | 7.52 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int32\", 4095)"]` | 8.46 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int32\", 4096)"]` | 7.71 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int64\", 4095)"]` | 6.78 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int64\", 4096)"]` | 6.84 (20%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"ascending\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"descending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"ones\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort forwards\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort reverse\", \"ascending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort reverse\", \"descending\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort reverse\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"descending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ones\")"]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 2.06 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ascending\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"descending\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ones\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ascending\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"descending\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ones\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort forwards\", \"ascending\")"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort forwards\", \"descending\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort forwards\", \"ones\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort forwards\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort reverse\", \"ascending\")"]` | 2.04 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort reverse\", \"descending\")"]` | 1.76 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort reverse\", \"ones\")"]` | 1.77 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort reverse\", \"random\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! forwards\", \"ascending\")"]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! forwards\", \"descending\")"]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! forwards\", \"ones\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! forwards\", \"random\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! reverse\", \"ascending\")"]` | 2.07 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! reverse\", \"descending\")"]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! reverse\", \"ones\")"]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sort! reverse\", \"random\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ascending\")"]` | 1.76 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"descending\")"]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ones\")"]` | 1.76 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"random\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ascending\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"descending\")"]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ones\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"random\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"descending\")"]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ones\")"]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"random\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"descending\")"]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ones\")"]` | 1.78 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"random\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sort forwards\", \"ones\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sort reverse\", \"ones\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sort! forwards\", \"ones\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sort! reverse\", \"ones\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 1000)"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 1.11 (30%)  | 1.01 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 10)"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 100)"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 1000)"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"logical\", 1000)"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"range\", 10)"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"range\", 100)"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"range\", 1000)"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 100)"]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 1.97 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 1.91 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 100)"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 1.14 (30%)  | 1.23 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 1.03 (30%)  | 1.23 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 1.00 (30%)  | 1.13 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"integer\", 1000)"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"integer\", 10000)"]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"integer\", 100000)"]` | 1.91 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x50 -> dense 5x50\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x200, sparse 2000x200 -> dense 20x2000\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x20, dense 20x20 -> dense 2000x20\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x200, dense 20x200 -> dense 2000x20\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x20, dense 200x20 -> dense 200x200\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x2000, dense 20x2000 -> dense 200x20\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x200, dense 200x200 -> dense 20x200\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x40, sparse 400x40 -> dense 400x400\")"]` | 1.54 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x400, dense 40x400 -> dense 4000x40\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x40, dense 400x40 -> dense 400x400\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x4000, dense 40x4000 -> dense 400x40\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x200, dense 20x2000 -> dense 200x20\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 1.75 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x400, dense 40x4000 -> dense 400x40\")"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 2.28 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 2"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["string", "replace"]` | 2.90 (15%) :x: | 2.20 (1%) :x: |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 4.38 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 1.24 (15%) :x: | 1.16 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 1.25 (15%) :x: | 1.16 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.19 (15%) :x: | 1.21 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 1.21 (15%) :x: | 1.21 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.91 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 2.87 (15%) :x: | 6.09 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 3.14 (15%) :x: | 6.09 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 2.59 (15%) :x: | 6.49 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 2.94 (15%) :x: | 4.05 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 3.06 (15%) :x: | 3.96 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 3.02 (15%) :x: | 9.87 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 3.57 (15%) :x: | 6.73 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 3.52 (15%) :x: | 6.58 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 2.61 (15%) :x: | 5.91 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 3.28 (15%) :x: | 4.21 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 3.30 (15%) :x: | 4.12 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 3.02 (15%) :x: | 5.91 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 3.23 (15%) :x: | 4.21 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 3.37 (15%) :x: | 4.12 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 1.98 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 2.82 (15%) :x: | 4.58 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 3.16 (15%) :x: | 4.58 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 1.44 (15%) :x: | 1.16 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 1.49 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 2.51 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 3.37 (15%) :x: | 6.43 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 2.72 (15%) :x: | 6.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 3.44 (15%) :x: | 4.16 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 3.71 (15%) :x: | 7.17 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 4.80 (15%) :x: | 5.31 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 2.79 (15%) :x: | 4.35 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 3.70 (15%) :x: | 3.39 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 3.56 (15%) :x: | 4.35 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 3.94 (15%) :x: | 3.39 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 2.43 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 3.23 (15%) :x: | 4.75 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 2.66 (15%) :x: | 1.92 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 2.83 (15%) :x: | 1.92 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 2.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 4.34 (15%) :x: | 6.43 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 2.87 (15%) :x: | 4.72 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 3.29 (15%) :x: | 3.14 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 3.40 (15%) :x: | 7.17 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 4.72 (15%) :x: | 5.31 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 2.91 (15%) :x: | 4.35 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 4.22 (15%) :x: | 3.39 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 3.01 (15%) :x: | 4.35 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 3.69 (15%) :x: | 3.39 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 2.71 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 3.69 (15%) :x: | 4.75 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 1.24 (15%) :x: | 1.06 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 1.24 (15%) :x: | 1.06 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 1.22 (15%) :x: | 1.08 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 1.24 (15%) :x: | 1.08 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 1.34 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 1.39 (15%) :x: | 1.44 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 1.31 (15%) :x: | 1.40 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 1.39 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 1.38 (15%) :x: | 1.40 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 1.29 (15%) :x: | 1.47 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 1.37 (15%) :x: | 1.54 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 1.40 (15%) :x: | 1.55 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 1.32 (15%) :x: | 1.36 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 1.35 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 1.35 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 1.31 (15%) :x: | 1.36 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 1.34 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 1.35 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 1.37 (15%) :x: | 1.41 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 1.40 (15%) :x: | 1.44 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 1.43 (15%) :x: | 1.08 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 1.43 (15%) :x: | 1.21 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 3.37 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 3.31 (15%) :x: | 3.36 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 3.09 (15%) :x: | 6.88 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 3.33 (15%) :x: | 3.95 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 5.07 (15%) :x: | 8.63 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 4.20 (15%) :x: | 4.90 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 4.27 (15%) :x: | 4.92 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 3.45 (15%) :x: | 3.12 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 5.95 (15%) :x: | 4.92 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 4.12 (15%) :x: | 3.12 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 3.60 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 4.18 (15%) :x: | 3.36 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 2.97 (15%) :x: | 1.48 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 2.20 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 2.36 (15%) :x: | 1.48 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 3.30 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 3.31 (15%) :x: | 3.36 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 2.06 (15%) :x: | 4.96 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 3.26 (15%) :x: | 2.97 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 4.89 (15%) :x: | 8.63 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 3.98 (15%) :x: | 4.90 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 4.95 (15%) :x: | 4.92 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 3.93 (15%) :x: | 3.12 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 5.04 (15%) :x: | 4.92 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 3.80 (15%) :x: | 3.12 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 4.80 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 3.25 (15%) :x: | 3.36 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 1.28 (15%) :x: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 1.25 (15%) :x: | 1.09 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 1.33 (15%) :x: | 1.09 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 1.11 (15%)  | 1.11 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 1.14 (15%)  | 1.12 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (true, true))"]` | 1.12 (15%)  | 1.12 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, false))"]` | 4.37 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, true))"]` | 4.05 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 3.52 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 3.28 (15%) :x: | 7.07 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 3.51 (15%) :x: | 6.70 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 3.45 (15%) :x: | 6.51 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, false))"]` | 6.40 (15%) :x: | 11.77 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 6.00 (15%) :x: | 11.16 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 5.71 (15%) :x: | 10.85 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 5.37 (15%) :x: | 7.10 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 5.36 (15%) :x: | 6.75 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 5.18 (15%) :x: | 6.58 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 5.46 (15%) :x: | 7.10 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, true))"]` | 4.98 (15%) :x: | 6.75 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 5.07 (15%) :x: | 6.58 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, false))"]` | 3.89 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 3.80 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 4.61 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"BigFloat\")"]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 2.87 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 2.61 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 3.28 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 2.99 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 4.12 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 2.93 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, false)"]` | 3.20 (15%) :x: | 1.96 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 3.05 (15%) :x: | 1.96 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 3.17 (15%) :x: | 1.96 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 3.03 (15%) :x: | 1.96 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 4.42 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 3.89 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 3.36 (15%) :x: | 3.33 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 3.51 (15%) :x: | 3.14 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 5.27 (15%) :x: | 5.60 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 6.03 (15%) :x: | 5.29 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 5.45 (15%) :x: | 3.60 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 4.73 (15%) :x: | 3.43 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int64, false)"]` | 4.48 (15%) :x: | 3.60 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 4.01 (15%) :x: | 3.43 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 5.13 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 5.06 (15%) :x: | 4.60 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 6.56 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 5.36 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, false)"]` | 3.78 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 3.98 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float32, false)"]` | 8.26 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 7.07 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float64, false)"]` | 8.94 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 7.00 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Int64, false)"]` | 8.33 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Int64, true)"]` | 7.70 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 5.74 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 5.00 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.4865
Commit 8ac77cc (2018-04-12 20:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    2051919 s        256 s     316679 s  137803096 s          1 s
       #2  3501 MHz   17494312 s          0 s     278372 s  122595767 s          0 s
       #3  3501 MHz    2044398 s       2368 s     222203 s  137927859 s          1 s
       #4  3501 MHz    1971293 s          0 s     304486 s  138023712 s          1 s
       
  Memory: 31.383651733398438 GB (20417.30859375 MB free)
  Uptime: 1.404618e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4863
Commit 3666ffa (2018-04-12 19:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    2141722 s        256 s     326747 s  138583307 s          1 s
       #2  3501 MHz   18326490 s          0 s     287806 s  122636956 s          0 s
       #3  3501 MHz    2133788 s       2368 s     229980 s  138712699 s          1 s
       #4  3501 MHz    2053110 s          0 s     311974 s  138816989 s          1 s
       
  Memory: 31.383651733398438 GB (19969.0859375 MB free)
  Uptime: 1.413451e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
