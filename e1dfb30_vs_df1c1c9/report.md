# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e1dfb30139621811de4fad24ba8e0af2e7bd6c30](https://github.com/JuliaLang/julia/commit/e1dfb30139621811de4fad24ba8e0af2e7bd6c30) vs [JuliaLang/julia@df1c1c939bf1c582cf040b5ad235933242aeacfb](https://github.com/JuliaLang/julia/commit/df1c1c939bf1c582cf040b5ad235933242aeacfb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27030#issuecomment-402542021)

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
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 0.95 (15%)  | 0.00 (1%) :white_check_mark: |
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1} generator\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1}\")"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int64,1} generator\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int64,1}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Vector{Bool}\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1} generator\")"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1}\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int64,1} generator\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Vector{Bool}\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "boolarray_bool_load!"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.50 (15%) :x: | 2.39 (1%) :x: |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 1.22 (15%) :x: | 2.59 (1%) :x: |
| `["array", "cat", "(\"hcat\", 5)"]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 1.04 (15%)  | 0.82 (1%) :white_check_mark: |
| `["array", "cat", "(\"hvcat\", 5)"]` | 0.99 (15%)  | 0.78 (1%) :white_check_mark: |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 0.94 (15%)  | 0.78 (1%) :white_check_mark: |
| `["array", "cat", "(\"vcat\", 5)"]` | 0.27 (15%) :white_check_mark: | 0.83 (1%) :white_check_mark: |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 0.99 (15%)  | 0.82 (1%) :white_check_mark: |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float32,1}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float64,1}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Int16,1}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 357.83 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float32,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float64,1}\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float64,1}\")"]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int16,1}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 357.83 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"BitArray\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"UnitRange{Int64}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 2048)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 256)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 1.62 (15%) :x: | 1.33 (1%) :x: |
| `["array", "growth", "(\"push_single!\", 256)"]` | 1.72 (15%) :x: | 2.18 (1%) :x: |
| `["array", "growth", "(\"push_single!\", 8)"]` | 1.87 (15%) :x: | 2.83 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.40 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.39 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 0.30 (50%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.42 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.39 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.43 (50%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.50 (50%) :x: | 1.47 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.39 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.40 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.43 (50%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.49 (50%)  | 1.62 (1%) :x: |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 1.42 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian\", \"BitArray{2}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float64,3}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Int32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BitArray{2}\")"]` | 0.22 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.28 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.28 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon\", \"BitArray{2}\")"]` | 0.24 (50%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.82 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.75 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.81 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.74 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"Array{Float32,2}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"Array{Int32,2}\")"]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"BitArray{2}\")"]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BitArray{2}\")"]` | 0.07 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"Array{Float32,2}\")"]` | 0.36 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"Array{Float64,3}\")"]` | 0.85 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"Array{Int32,2}\")"]` | 0.36 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.02 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 0.37 (50%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.45 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.07 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.46 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumelt\", \"BitArray{2}\")"]` | 0.07 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Int32,2}\")"]` | 4.79 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"BitArray{2}\")"]` | 0.07 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.50 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BitArray{2}\")"]` | 0.07 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"100000:-1:1\")"]` | 1272.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"1:100000\")"]` | 566.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"Array{Float32,2}\")"]` | 0.36 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"Array{Float64,3}\")"]` | 0.89 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"Array{Int32,2}\")"]` | 0.36 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.02 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.33 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.33 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.33 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.34 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 0.37 (50%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.34 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.59 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.34 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.31 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.78 (50%)  | 0.56 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.03 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.33 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.58 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.34 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.31 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 0.66 (50%)  | 0.91 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.43 (50%)  | 0.97 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.26 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 3.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.42 (50%)  | 0.97 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Float32,2}\")"]` | 1.12 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"Array{Int32,2}\")"]` | 1.11 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.17 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.08 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.11 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.11 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.14 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.29 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"BitArray{2}\")"]` | 0.24 (50%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.63 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.19 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.70 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.78 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.70 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.14 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.98 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.63 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.08 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.70 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.73 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.68 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.12 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.98 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"Array{Float32,2}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"Array{Int32,2}\")"]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.14 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.17 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.12 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.17 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.18 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 0.66 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 0.65 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 0.66 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 0.67 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"BitArray{2}\")"]` | 0.25 (50%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.62 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 3.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 3.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.01 (50%)  | 0.87 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 3.45 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.91 (50%)  | 0.87 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 3.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "ind2sub"]` | 0.28 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "sub2ind"]` | 0.03 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Int64\")"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"maxabs\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 0.63 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 0.59 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 0.64 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.61 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 0.69 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.62 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.59 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 2.16 (15%) :x: | 1.14 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.75 (15%) :x: | 1.01 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.93 (15%) :x: | 1.05 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.75 (15%) :x: | 1.02 (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 0.16 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 0.95 (15%)  | 0.67 (1%) :white_check_mark: |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "sparse", "((10000000,), 2)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 0.59 (25%) :white_check_mark: | 0.72 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 186.04 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter!\")"]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 0.91 (25%)  | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"pop!\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"pop!\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"String\", \"pop!\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"iterator\")"]` | 0.90 (25%)  | 0.52 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\")"]` | 0.93 (25%)  | 0.52 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\", \"sizehint!\")"]` | 0.97 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"iterator\")"]` | 0.84 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\")"]` | 0.84 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\", \"sizehint!\")"]` | 0.86 (25%)  | 2.00 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 0.68 (25%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\")"]` | 0.57 (25%) :white_check_mark: | 0.74 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.58 (25%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"iterator\")"]` | 0.47 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\")"]` | 0.47 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.43 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 0.62 (25%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 0.60 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.62 (25%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"iterator\")"]` | 0.48 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\")"]` | 0.52 (25%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.49 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"iterator\")"]` | 5.20 (25%) :x: | Inf (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\")"]` | 1.54 (25%) :x: | 1.07 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\", \"sizehint!\")"]` | 1.59 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Int\", \"iterator\")"]` | 4.57 (25%) :x: | Inf (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Int\", \"loop\")"]` | 1.59 (25%) :x: | 1.05 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Int\", \"loop\", \"sizehint!\")"]` | 1.72 (25%) :x: | 1.09 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"iterator\")"]` | 5.03 (25%) :x: | Inf (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\")"]` | 1.29 (25%) :x: | 1.02 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\", \"sizehint!\")"]` | 1.29 (25%) :x: | 1.05 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"next\")"]` | 1.73 (25%) :x: | 1.50 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"start\")"]` | 622.32 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"next\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"start\")"]` | 689.11 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"next\")"]` | 1.54 (25%) :x: | 1.50 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"start\")"]` | 653.11 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"next\")"]` | 2.03 (25%) :x: | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"start\")"]` | 641.47 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"start\")"]` | 665.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"next\")"]` | 1.29 (25%) :x: | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"start\")"]` | 599.65 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"next\")"]` | 2.48 (25%) :x: | 2.50 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"start\")"]` | 409.85 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"start\")"]` | 399.31 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"next\")"]` | 1.22 (25%)  | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"start\")"]` | 397.69 (25%) :x: | Inf (1%) :x: |
| `["collection", "optimizations", "(\"BitSet\", \"Int8\")"]` | 0.89 (25%)  | 0.91 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Bool\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Int8\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"UInt16\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Bool\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Int8\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"UInt16\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Bool\")"]` | 0.57 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Int8\")"]` | 0.96 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"UInt16\")"]` | 0.95 (25%)  | 2.50 (1%) :x: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Bool\")"]` | 0.57 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Int8\")"]` | 0.96 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"UInt16\")"]` | 0.95 (25%)  | 2.50 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"in\", \"false\")"]` | 4.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"in\", \"true\")"]` | 1.13 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"specified\")"]` | 1.06 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"new\")"]` | 2.72 (25%) :x: | 2.50 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"overwrite\")"]` | 1.20 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"new\")"]` | 2.73 (25%) :x: | 2.50 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"overwrite\")"]` | 1.09 (25%)  | 2.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"first\")"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"in\", \"true\")"]` | 0.48 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"specified\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"push!\", \"new\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"false\")"]` | 3.91 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"specified\")"]` | 0.84 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 47.06 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"new\")"]` | 2.48 (25%) :x: | 4.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 1.06 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"first\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"specified\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"unspecified\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"push!\", \"new\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"push!\", \"overwrite\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"false\")"]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"unspecified\")"]` | 0.55 (25%) :white_check_mark: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 1.80 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"in\", \"false\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 0.49 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 3.16 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"big\")"]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"small\")"]` | 0.00 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"big\")"]` | 0.00 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"small\")"]` | 0.00 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"big\")"]` | 0.26 (25%) :white_check_mark: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"small\")"]` | 0.22 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 0.25 (25%) :white_check_mark: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"small\")"]` | 0.21 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\")"]` | 0.04 (25%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 0.05 (25%) :white_check_mark: | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.05 (25%) :white_check_mark: | 1.04 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 0.02 (25%) :white_check_mark: | 3.91 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.06 (25%) :white_check_mark: | 10.70 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Set\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Vector\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Set\")"]` | 0.04 (25%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.03 (25%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\")"]` | 55.93 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 0.27 (25%) :white_check_mark: | 0.48 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.29 (25%) :white_check_mark: | 0.47 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.09 (25%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.10 (25%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Set\")"]` | 0.45 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Vector\")"]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\")"]` | 0.04 (25%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\")"]` | 0.40 (25%) :white_check_mark: | 0.72 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.38 (25%) :white_check_mark: | 0.72 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\")"]` | 0.08 (25%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.08 (25%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Set\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Vector\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 3.76 (25%) :x: | 1.81 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\")"]` | 4.07 (25%) :x: | 8.32 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 4.08 (25%) :x: | 8.37 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\")"]` | 2.58 (25%) :x: | 10.25 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 2.61 (25%) :x: | 12.18 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 0.75 (25%)  | 0.39 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.82 (25%)  | 0.38 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 3174.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 0.20 (25%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.22 (25%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.20 (25%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.21 (25%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 0.13 (25%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 0.11 (25%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.11 (25%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 0.13 (25%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.13 (25%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"empty\", \"Int\", \"⊆\", \"Set\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["dates", "accessor", "millisecond"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Month\")"]` | 0.80 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"DateTime\", \"Year\")"]` | 0.85 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 0.88 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"Date\", \"Year\")"]` | 0.83 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "construction", "Date"]` | 0.31 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "construction", "DateTime"]` | 0.26 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 0.66 (15%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.31 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.10 (15%)  | 1.14 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.97 (15%)  | 1.07 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.06 (15%)  | 1.14 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.73 (15%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 0.65 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "parse", "Date"]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "parse", "DateTime"]` | 1.47 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["dates", "string", "DateTime"]` | 1.17 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.08 (15%)  | 0.69 (1%) :white_check_mark: |
| `["find", "findall", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.01 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "findall", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.04 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "findall", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.11 (15%)  | 0.80 (1%) :white_check_mark: |
| `["find", "findall", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.99 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "findall", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.03 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "findall", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.03 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.01 (15%)  | 0.00 (1%) :white_check_mark: |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.62 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.29 (15%) :x: | 1.90 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 11.48 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.75 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 13.71 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"10-90\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"BitArray{1}\", \"90-10\")"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.87 (15%)  | 0.00 (1%) :white_check_mark: |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.65 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.51 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.11 (15%)  | 1.90 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 8.52 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.60 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 9.39 (15%) :x: | 1.00 (1%)  |
| `["io", "serialization", "(\"deserialize\", \"Vector{String}\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 0.94 (15%)  | 0.95 (1%) :white_check_mark: |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 0.51 (45%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 0.46 (45%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 0.84 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.79 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 0.50 (45%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 0.47 (45%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 0.78 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.85 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 1024)"]` | 1.00 (45%)  | 0.60 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 256)"]` | 0.96 (45%)  | 0.60 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 1024)"]` | 0.64 (45%)  | 0.72 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 256)"]` | 0.58 (45%)  | 0.73 (1%) :white_check_mark: |
| `["linalg", "blas", "dotc"]` | 0.96 (40%)  | 0.00 (1%) :white_check_mark: |
| `["linalg", "blas", "dotu"]` | 0.96 (40%)  | 0.00 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"chol\", \"Matrix\", 256)"]` | 1.15 (45%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"cholfact\", \"Matrix\", 256)"]` | 1.14 (45%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"eig\", \"Bidiagonal\", 256)"]` | 1.16 (45%)  | 1.03 (1%) :x: |
| `["linalg", "factorization", "(\"eig\", \"Diagonal\", 256)"]` | 2.15 (45%) :x: | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"eig\", \"SymTridiagonal\", 256)"]` | 1.01 (45%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"eigfact\", \"Bidiagonal\", 256)"]` | 1.19 (45%)  | 1.03 (1%) :x: |
| `["linalg", "factorization", "(\"eigfact\", \"Diagonal\", 256)"]` | 2.47 (45%) :x: | 1.03 (1%) :x: |
| `["linalg", "factorization", "(\"eigfact\", \"SymTridiagonal\", 256)"]` | 1.01 (45%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 1024)"]` | 0.64 (45%)  | 0.33 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 256)"]` | 0.83 (45%)  | 0.33 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 1024)"]` | 0.00 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 256)"]` | 0.01 (45%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"lufact\", \"Matrix\", 256)"]` | 1.10 (45%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 1024)"]` | 4.66 (45%) :x: | 1.30 (1%) :x: |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 256)"]` | 12.88 (45%) :x: | 2.15 (1%) :x: |
| `["linalg", "factorization", "(\"qr\", \"Matrix\", 1024)"]` | 0.37 (45%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"qr\", \"Matrix\", 256)"]` | 0.46 (45%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"qrfact\", \"Matrix\", 256)"]` | 0.97 (45%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"schurfact\", \"Matrix\", 256)"]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Bidiagonal\", 1024)"]` | 0.97 (45%)  | 0.83 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"Bidiagonal\", 256)"]` | 0.98 (45%)  | 0.83 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 0.48 (45%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 1.00 (45%)  | 0.09 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"LowerTriangular\", 1024)"]` | 1.00 (45%)  | 0.88 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"LowerTriangular\", 256)"]` | 0.99 (45%)  | 0.88 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"Matrix\", 1024)"]` | 1.00 (45%)  | 0.86 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"Matrix\", 256)"]` | 0.99 (45%)  | 0.86 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"UpperTriangular\", 1024)"]` | 1.00 (45%)  | 0.88 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"UpperTriangular\", 256)"]` | 0.98 (45%)  | 0.88 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 1024)"]` | 0.39 (45%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 256)"]` | 0.94 (45%)  | 0.07 (1%) :white_check_mark: |
| `["micro", "parseint"]` | 1.70 (15%) :x: | 1.17 (1%) :x: |
| `["micro", "randmatstat"]` | 0.90 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "afoldl", "Complex{Float64}"]` | 0.07 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "afoldl", "Float64"]` | 0.05 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "afoldl", "Int"]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.15 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 0.17 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 0.05 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 0.16 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "julia", "(\"macroexpand\", \"evalpoly\")"]` | 0.01 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.23 (15%) :x: | 0.85 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["misc", "parse", "DateTime"]` | 1.51 (15%) :x: | 0.00 (1%) :white_check_mark: |
| `["misc", "parse", "Float64"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 1.23 (15%) :x: | 2.03 (1%) :x: |
| `["misc", "repeat", "(200, 24, 1)"]` | 1.00 (15%)  | 1.12 (1%) :x: |
| `["misc", "splatting", "(3, 3, 3)"]` | 0.69 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 0.85 (15%)  | 1.06 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 0.20 (15%) :white_check_mark: | 1.11 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 0.78 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 0.32 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 0.46 (15%) :white_check_mark: | 1.11 (1%) :x: |
| `["problem", "chaosgame", "chaosgame"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 0.77 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 2.10 (15%) :x: | 1.76 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 1.16 (15%) :x: | 1.32 (1%) :x: |
| `["problem", "json", "parse_json"]` | 1.85 (15%) :x: | 2.63 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 4.78 (15%) :x: | 3829.61 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 0.53 (15%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem", "simplex", "simplex"]` | 0.72 (15%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["problem", "spellcheck", "spellcheck"]` | 2.15 (15%) :x: | 2.20 (1%) :x: |
| `["problem", "ziggurat", "ziggurat"]` | 2.64 (15%) :x: | 2.83 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"'a':'z'\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Vector\")"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Vector\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"'a':'z'\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Vector\")"]` | 0.45 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Vector\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Vector\")"]` | 0.49 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Vector\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Vector\")"]` | 0.49 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Vector\")"]` | 0.48 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\")"]` | 0.44 (25%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", 100)"]` | 0.33 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 1.27 (25%) :x: | 0.87 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 1.29 (25%) :x: | 0.86 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 1.29 (25%) :x: | 0.87 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.39 (25%) :x: | 0.86 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:2^10000\")"]` | 1.00 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 1.28 (25%) :x: | 0.86 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 1.29 (25%) :x: | 0.86 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551615\")"]` | 0.45 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551616\")"]` | 0.37 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int32\", \"1:1\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:1\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967295\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967297\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int8\", \"1:1\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551615\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551616\")"]` | 0.37 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt16\", \"1:1\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt32\", \"1:1\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt32\", \"1:4294967295\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:18446744073709551615\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:1\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967295\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967297\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt8\", \"1:1\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 0.31 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 0.31 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 0.77 (25%)  | 0.16 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 0.80 (25%)  | 0.18 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.90 (25%)  | 0.16 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.77 (25%)  | 0.16 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.84 (25%)  | 0.84 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 0.97 (25%)  | 0.16 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967297)\")"]` | 0.91 (25%)  | 0.16 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:1)\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967295)\")"]` | 0.38 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967297)\")"]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:4294967297)\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:1)\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967295)\")"]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967297)\")"]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967297)\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"ImplicitRNG\", \"Int64\")"]` | 1.03 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Bool\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int16}\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int32}\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int8}\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt8}\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float16\")"]` | 1.47 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 0.95 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int128\")"]` | 1.03 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int16\")"]` | 1.02 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int32\")"]` | 1.03 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int64\")"]` | 1.04 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int8\")"]` | 0.93 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt128\")"]` | 1.04 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt16\")"]` | 1.01 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt32\")"]` | 0.99 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt64\")"]` | 1.04 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt8\")"]` | 0.93 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt128\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"ImplicitRNG\", \"Float64\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float32\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float64\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"ImplicitRNG\", \"Float64\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float32\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float64\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"Float64\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"1 <= abs(x) < 2\", \"positive argument\", \"Float32\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"1 <= abs(x) < 2\", \"positive argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"one\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"one\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigFloat\")"]` | 0.72 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 0.53 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.57 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.59 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.60 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 0.57 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 0.58 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Int64\")"]` | 0.83 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"UInt64\")"]` | 0.82 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 0.57 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigInt\")"]` | 1.35 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.56 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.37 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 0.62 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Int64}\")"]` | 1.14 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{UInt64}\")"]` | 1.18 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float32\")"]` | 0.64 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float64\")"]` | 0.64 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Int64\")"]` | 0.95 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"UInt64\")"]` | 1.36 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.55 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.60 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.51 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.51 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.74 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.70 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.59 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.59 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.86 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.84 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.56 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.36 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.13 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.59 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 1.12 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 1.15 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 0.63 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 0.62 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 1.33 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.37 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.59 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.51 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.59 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.51 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.48 (50%) :white_check_mark: | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.72 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 1.23 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.74 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 1.11 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.70 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 1.08 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 1.16 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 0.58 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigInt\")"]` | 0.64 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.59 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 0.58 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigInt\")"]` | 0.63 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigFloat\")"]` | 0.83 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigInt\")"]` | 1.37 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.85 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigInt}\")"]` | 1.35 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 0.82 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 1.37 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.83 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 1.37 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigFloat\")"]` | 0.90 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 0.24 (50%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.03 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.04 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.62 (50%)  | 1.04 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.70 (50%)  | 1.04 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.64 (50%)  | 1.04 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.63 (50%)  | 1.04 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 0.44 (50%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 0.44 (50%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Int64\")"]` | 0.70 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"UInt64\")"]` | 0.67 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigFloat\")"]` | 0.82 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigInt\")"]` | 0.76 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.53 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.51 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.51 (50%)  | 0.99 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.53 (50%)  | 0.99 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.64 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.61 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float32\")"]` | 0.74 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float64\")"]` | 0.74 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 0.64 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"UInt64\")"]` | 0.66 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.78 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.26 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.57 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.57 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.59 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.58 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.57 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.46 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.45 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.59 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.72 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.66 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.58 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.35 (50%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.52 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.53 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 0.66 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 0.66 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.63 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 0.66 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.57 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.63 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 0.67 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.58 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.81 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 0.72 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.57 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.49 (50%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.81 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.70 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.58 (50%)  | 1.05 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.54 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 0.70 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigInt\")"]` | 0.76 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.61 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.59 (50%)  | 0.99 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 0.70 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigInt\")"]` | 0.73 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.61 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.60 (50%)  | 0.99 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigFloat\")"]` | 0.85 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigInt\")"]` | 0.83 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 1.03 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.01 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigFloat\")"]` | 0.88 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigInt\")"]` | 0.81 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.03 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.01 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigFloat\")"]` | 0.80 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 0.29 (50%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 1.07 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.31 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.52 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.49 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.56 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.55 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 0.56 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 0.56 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Int64\")"]` | 0.67 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"UInt64\")"]` | 0.67 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 0.29 (50%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigInt\")"]` | 1.36 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.30 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.14 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 1.17 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 1.14 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float32\")"]` | 0.63 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float64\")"]` | 0.67 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Int64\")"]` | 1.39 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"UInt64\")"]` | 1.36 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.29 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.32 (50%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.47 (50%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.48 (50%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.59 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.54 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.61 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.44 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.55 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.59 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.31 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.19 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.33 (50%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.97 (50%) :x: | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.54 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.53 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 2.03 (50%) :x: | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.00 (50%) :x: | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 0.60 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 0.60 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Int64\")"]` | 1.13 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.15 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.50 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.47 (50%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.54 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.50 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.48 (50%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.54 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.56 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigInt\")"]` | 1.47 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.55 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 2.07 (50%) :x: | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.55 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigInt\")"]` | 1.16 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.54 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.04 (50%) :x: | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 0.56 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 0.66 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.54 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 0.60 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 0.55 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigInt\")"]` | 0.67 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.55 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 0.59 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigFloat\")"]` | 0.66 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 0.84 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.55 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 1.18 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigFloat\")"]` | 0.68 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 1.39 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.59 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigInt}\")"]` | 1.17 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"Bool\")"]` | 0.39 (40%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"Int64\")"]` | 2.95 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 1.16 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Bool\")"]` | 0.22 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Int64\")"]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"UInt64\")"]` | 0.13 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"BigInt\")"]` | 1.40 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"BigInt\")"]` | 0.96 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Bool\")"]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Int64\")"]` | 0.12 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"UInt64\")"]` | 0.13 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"BigInt\")"]` | 0.87 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Bool\")"]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Int64\")"]` | 0.18 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"UInt64\")"]` | 0.12 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigFloat\")"]` | 0.71 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 0.46 (50%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.49 (50%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.53 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.53 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.59 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.60 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 0.53 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 0.56 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Int64\")"]` | 0.70 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"UInt64\")"]` | 0.69 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 0.46 (50%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigInt\")"]` | 1.36 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.49 (50%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.13 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Int64}\")"]` | 1.26 (50%)  | 0.77 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{UInt64}\")"]` | 1.12 (50%)  | 0.77 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float32\")"]` | 0.62 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float64\")"]` | 0.62 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Int64\")"]` | 0.91 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"UInt64\")"]` | 1.39 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.60 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.61 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.83 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.49 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.48 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.68 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.67 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.55 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.86 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.74 (50%)  | 1.06 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.49 (50%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.20 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.53 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.16 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.56 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 1.11 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 1.16 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 1.17 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.14 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.54 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.48 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.55 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.51 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 0.58 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.48 (50%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.56 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.65 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 0.87 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.65 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 1.00 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 1.10 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 0.54 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigInt\")"]` | 0.61 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.53 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 0.54 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigInt\")"]` | 0.62 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.53 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 0.57 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigFloat\")"]` | 0.69 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 0.91 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigInt}\")"]` | 0.98 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigFloat\")"]` | 0.69 (50%)  | 1.08 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 0.97 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.66 (50%)  | 1.07 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.99 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"negative argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float64\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float64\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigFloat\")"]` | 0.70 (40%)  | 1.08 (1%) :x: |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 1.38 (40%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 0.68 (40%)  | 1.07 (1%) :x: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 1.28 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"div\", \"BigFloat\")"]` | 0.89 (40%)  | 1.08 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigInt\")"]` | 0.77 (40%)  | 1.08 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 0.60 (40%) :white_check_mark: | 1.07 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.36 (40%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"mul\", \"BigFloat\")"]` | 0.81 (40%)  | 1.08 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 1.37 (40%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 0.61 (40%)  | 1.07 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 1.99 (40%) :x: | 0.75 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"sub\", \"BigFloat\")"]` | 0.71 (40%)  | 1.08 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 0.72 (40%)  | 0.75 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 0.60 (40%) :white_check_mark: | 1.07 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigInt}\")"]` | 1.11 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float64\")"]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float32\")"]` | 0.27 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float64\")"]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float32\")"]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float64\")"]` | 0.19 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float32\")"]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float64\")"]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"normal path -> small, k = -150\", \"Float32\")"]` | 0.21 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"overflow\", \"Float32\")"]` | 0.21 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"overflow\", \"Float64\")"]` | 0.22 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"taylor expansion\", \"Float32\")"]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"underflow\", \"Float32\")"]` | 0.21 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"underflow\", \"Float64\")"]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp\", \"no agument reduction, k = 9\", \"Float64\")"]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"+\")"]` | 1.24 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"-\")"]` | 1.24 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar", "intfuncs", "(\"nextpow2\", \"Int64\", \"+\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"Int64\", \"-\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"UInt64\", \"+\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"UInt64\", \"-\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"+\")"]` | 1.34 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"-\")"]` | 1.32 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "intfuncs", "(\"prevpow2\", \"Int64\", \"+\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"UInt64\", \"+\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "iteration", "indexed"]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.40 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.42 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.40 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.38 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.34 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.45 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.46 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 1.01 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 1.02 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.38 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.35 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.35 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.35 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.35 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.38 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.33 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.42 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.39 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.39 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.32 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.32 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"negative argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2f0^-12\", \"negative argument\", \"Float32\")"]` | 2.56 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2f0^-12\", \"positive argument\", \"Float32\")"]` | 2.56 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "binary_trees"]` | 0.82 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["shootout", "mandelbrot"]` | 0.97 (15%)  | 1.04 (1%) :x: |
| `["shootout", "meteor_contest"]` | 0.72 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["shootout", "nbody"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "pidigits"]` | 1.23 (15%) :x: | 0.99 (1%)  |
| `["shootout", "regex_dna"]` | 60.75 (15%) :x: | 1.00 (1%)  |
| `["shootout", "revcomp"]` | 0.81 (25%)  | 0.91 (1%) :white_check_mark: |
| `["shootout", "spectralnorm"]` | 1.00 (15%)  | 0.22 (1%) :white_check_mark: |
| `["simd", "(\"auto_conditional_loop!\", \"Float32\", 4095)"]` | 4.12 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Float32\", 4096)"]` | 4.14 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Float64\", 4095)"]` | 3.58 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Float64\", 4096)"]` | 3.59 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4095)"]` | 0.05 (20%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4096)"]` | 0.05 (20%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["simd", "(\"auto_local_arrays\", \"Float64\", 4095)"]` | 0.07 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd", "(\"auto_local_arrays\", \"Float64\", 4096)"]` | 0.07 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd", "(\"auto_local_arrays\", \"Int32\", 4095)"]` | 0.06 (20%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["simd", "(\"auto_local_arrays\", \"Int32\", 4096)"]` | 0.06 (20%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["simd", "(\"auto_local_arrays\", \"Int64\", 4095)"]` | 0.08 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd", "(\"auto_local_arrays\", \"Int64\", 4096)"]` | 0.07 (20%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["simd", "(\"auto_two_reductions\", \"Int32\", 4095)"]` | 0.05 (20%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"auto_two_reductions\", \"Int32\", 4096)"]` | 0.05 (20%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4095)"]` | 8.23 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4096)"]` | 8.71 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4095)"]` | 3.25 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4096)"]` | 3.43 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4095)"]` | 6.99 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4096)"]` | 7.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4095)"]` | 1.36 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4096)"]` | 1.35 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4095)"]` | 27.87 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4096)"]` | 29.37 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4095)"]` | 11.76 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4096)"]` | 11.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 3.44 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 4.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 2.34 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 2.35 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Float32\", 4095)"]` | 7.52 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Float32\", 4096)"]` | 7.52 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Float64\", 4095)"]` | 6.37 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Float64\", 4096)"]` | 6.35 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4095)"]` | 3.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4096)"]` | 3.42 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 2.35 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4096)"]` | 1.77 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 0.06 (20%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 0.06 (20%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["simd", "(\"local_arrays\", \"Float64\", 4095)"]` | 0.09 (20%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["simd", "(\"local_arrays\", \"Float64\", 4096)"]` | 0.09 (20%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["simd", "(\"local_arrays\", \"Int32\", 4095)"]` | 0.07 (20%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["simd", "(\"local_arrays\", \"Int32\", 4096)"]` | 0.07 (20%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["simd", "(\"local_arrays\", \"Int64\", 4095)"]` | 0.09 (20%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["simd", "(\"local_arrays\", \"Int64\", 4096)"]` | 0.08 (20%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 11.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 12.19 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 12.32 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 12.70 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 5.13 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 5.14 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 5.27 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 5.33 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 11.44 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 11.52 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 10.63 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 10.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.22 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float32\", 4095)"]` | 7.50 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float32\", 4096)"]` | 7.50 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float64\", 4095)"]` | 3.67 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Float64\", 4096)"]` | 3.63 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int32\", 4095)"]` | 5.60 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int32\", 4096)"]` | 5.60 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int64\", 4095)"]` | 2.71 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!\", \"Int64\", 4096)"]` | 2.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Float32\", 4095)"]` | 14.54 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Float32\", 4096)"]` | 15.08 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Float64\", 4095)"]` | 6.54 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Float64\", 4096)"]` | 6.51 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int32\", 4095)"]` | 9.81 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int32\", 4096)"]` | 9.86 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int64\", 4095)"]` | 2.94 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"manual_example!_aliased\", \"Int64\", 4096)"]` | 2.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float32\", 4095)"]` | 8.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float32\", 4096)"]` | 8.75 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float64\", 4095)"]` | 7.33 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Float64\", 4096)"]` | 7.20 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 8.34 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 8.38 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4095)"]` | 4.51 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4096)"]` | 4.49 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float32\", 4095)"]` | 9.83 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float32\", 4096)"]` | 10.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float64\", 4095)"]` | 5.06 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Float64\", 4096)"]` | 5.11 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int32\", 4095)"]` | 0.18 (20%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"two_reductions\", \"Int32\", 4096)"]` | 0.19 (20%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"two_reductions\", \"Int64\", 4095)"]` | 4.48 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int64\", 4096)"]` | 4.64 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float32\", 4095)"]` | 9.89 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float32\", 4096)"]` | 10.28 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float64\", 4095)"]` | 5.10 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Float64\", 4096)"]` | 5.16 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int32\", 4095)"]` | 0.30 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int32\", 4096)"]` | 0.30 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int64\", 4095)"]` | 6.00 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int64\", 4096)"]` | 5.95 (20%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 0.62 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"descending\")"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ones\")"]` | 1.03 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"random\")"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 1.08 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 1.01 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ascending\")"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 0.88 (30%)  | 0.14 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 0.70 (30%)  | 0.14 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.05 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 0.71 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 0.70 (30%)  | 0.13 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 0.90 (30%)  | 0.13 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 1.03 (30%)  | 0.30 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 0.71 (30%)  | 0.30 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"forwards\", \"descending\")"]` | 0.37 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort", "issorted", "(\"forwards\", \"random\")"]` | 0.41 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 0.64 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 1.20 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"ones\")"]` | 0.88 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 0.66 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"ascending\")"]` | 0.87 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"descending\")"]` | 0.87 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"ones\")"]` | 1.02 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"random\")"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"descending\")"]` | 1.01 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ones\")"]` | 0.98 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"random\")"]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ascending\")"]` | 0.78 (30%)  | 0.14 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"descending\")"]` | 0.79 (30%)  | 0.14 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 0.89 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 0.87 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ascending\")"]` | 0.79 (30%)  | 0.13 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"descending\")"]` | 0.77 (30%)  | 0.13 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 0.89 (30%)  | 0.30 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 0.87 (30%)  | 0.30 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 1.05 (15%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 0.20 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 0.01 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 0.00 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 0.61 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 0.84 (15%) :white_check_mark: | 0.99 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 0.98 (15%)  | 0.94 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 1.00 (15%)  | 0.94 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 1.13 (30%)  | 1.22 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 0.96 (30%)  | 1.07 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 10)"]` | 1.00 (30%)  | 1.10 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 100)"]` | 0.97 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 1000)"]` | 0.95 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 0.88 (30%)  | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 0.83 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 0.85 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 0.80 (30%)  | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 0.75 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 0.98 (30%)  | 1.10 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 100)"]` | 0.98 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 1000)"]` | 0.93 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 100)"]` | 0.85 (30%)  | 1.64 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 0.99 (30%)  | 1.77 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 0.82 (30%)  | 1.76 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 0.84 (30%)  | 1.19 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.74 (30%)  | 1.14 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 100)"]` | 0.78 (30%)  | 1.64 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.14 (30%)  | 1.77 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 0.33 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 0.21 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 0.94 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.02 (30%)  | 1.12 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 1.76 (30%) :x: | 0.75 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.41 (30%) :x: | 0.72 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.03 (30%)  | 1.10 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 8.95 (30%) :x: | 1.21 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 3.84 (30%) :x: | 1.17 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.25 (30%)  | 1.19 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.81 (30%)  | 2.40 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.05 (30%)  | 1.12 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 1.96 (30%) :x: | 1.52 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.31 (30%) :x: | 1.45 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.84 (30%)  | 0.56 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 6.34 (30%) :x: | 1.68 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 2.74 (30%) :x: | 1.62 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.92 (30%)  | 1.64 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.60 (30%) :white_check_mark: | 2.32 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 0.48 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 0.48 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 0.51 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 0.44 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 0.47 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 0.90 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x2000, dense 2000x20 -> dense 2000x20\")"]` | 0.84 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 0.89 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 0.83 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 0.77 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 0.82 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x200, dense 20x200 -> dense 200x200\")"]` | 0.72 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 0.67 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.37 (30%) :white_check_mark: | 1.27 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.46 (30%) :white_check_mark: | 1.19 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.07 (30%)  | 1.17 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.45 (30%) :white_check_mark: | 1.10 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.60 (30%) :white_check_mark: | 0.72 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 2.33 (30%) :x: | 1.21 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 0.96 (30%)  | 0.75 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.85 (30%)  | 1.12 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.25 (30%)  | 1.19 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.83 (30%)  | 2.40 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 3.79 (30%) :x: | 1.17 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.40 (30%) :x: | 0.72 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.00 (30%)  | 1.10 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 8.71 (30%) :x: | 1.21 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 1.75 (30%) :x: | 0.75 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.01 (30%)  | 1.12 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 0.49 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 0.49 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 0.51 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 0.51 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.51 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.48 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 0.91 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 0.86 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 0.91 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 0.83 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 0.74 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 0.84 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 0.73 (30%)  | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 0.68 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.39 (30%) :white_check_mark: | 1.26 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.47 (30%) :white_check_mark: | 1.65 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.04 (30%)  | 1.62 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.48 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.61 (30%) :white_check_mark: | 0.72 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 2.14 (30%) :x: | 1.68 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 0.98 (30%)  | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.84 (30%)  | 1.12 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.92 (30%)  | 1.64 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.59 (30%) :white_check_mark: | 2.32 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 2.74 (30%) :x: | 1.62 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.30 (30%) :x: | 1.45 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.80 (30%)  | 0.56 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 6.35 (30%) :x: | 1.68 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 1.96 (30%) :x: | 1.52 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.04 (30%)  | 1.12 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose\", (20000, 10000))"]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (600, 400))"]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (600, 600))"]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["string", "join"]` | 1.12 (40%)  | 1.22 (1%) :x: |
| `["string", "readuntil", "backtracking"]` | 0.00 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["string", "readuntil", "barbarian backtrack"]` | 0.01 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["string", "readuntil", "no backtracking"]` | 0.01 (15%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 1"]` | 0.27 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 1000"]` | 0.07 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 2"]` | 0.22 (15%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 50000"]` | 0.10 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["string", "replace"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (4, 4), (4,))"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (16, 16))"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (8, 8))"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.15 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 0.61 (15%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 1.01 (15%)  | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 1.01 (15%)  | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 0.72 (15%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.04 (15%)  | 0.70 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 1.06 (15%)  | 0.70 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 0.36 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 1.91 (15%) :x: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 1.88 (15%) :x: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 0.20 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 1.06 (15%)  | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 1.07 (15%)  | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 0.18 (15%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 1.03 (15%)  | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.01 (15%)  | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.20 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 1.21 (15%) :x: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 1.21 (15%) :x: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 0.18 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 1.09 (15%)  | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 1.06 (15%)  | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 0.29 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 1.58 (15%) :x: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 1.59 (15%) :x: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 0.48 (15%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 1.10 (15%)  | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 0.38 (15%) :white_check_mark: | 0.36 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 0.87 (15%)  | 0.41 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 0.31 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 2.23 (15%) :x: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 0.26 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 1.29 (15%) :x: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 0.18 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 1.34 (15%) :x: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 0.20 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 1.53 (15%) :x: | 0.23 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 0.18 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 1.30 (15%) :x: | 0.23 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 0.25 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.72 (15%) :x: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 0.34 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 2.19 (15%) :x: | 0.49 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 0.33 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 2.10 (15%) :x: | 0.49 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 0.31 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 2.22 (15%) :x: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 0.17 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.18 (15%) :x: | 0.26 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 0.17 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 1.30 (15%) :x: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 0.20 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 1.48 (15%) :x: | 0.23 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 0.18 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 1.30 (15%) :x: | 0.23 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 0.25 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 1.82 (15%) :x: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 0.27 (15%) :white_check_mark: | 0.83 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 0.24 (15%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 0.24 (15%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 0.37 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 0.32 (15%) :white_check_mark: | 0.58 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 0.32 (15%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 0.02 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.02 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 0.02 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 0.02 (15%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 0.03 (15%) :white_check_mark: | 0.24 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 0.04 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 0.02 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 0.02 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.02 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 0.02 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 0.02 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.02 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 0.02 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 0.02 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 0.02 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 0.02 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.02 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 0.02 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 0.54 (15%) :white_check_mark: | 1.07 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 0.40 (15%) :white_check_mark: | 0.99 (1%)  |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 0.38 (15%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 0.34 (15%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 0.11 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 0.37 (15%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 0.16 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 0.09 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 0.10 (15%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 0.07 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 0.11 (15%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 0.06 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 0.13 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 0.06 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 0.16 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 0.15 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 0.11 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 0.10 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.10 (15%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 0.09 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 0.09 (15%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 0.06 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 0.09 (15%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 0.06 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.11 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.05 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 0.61 (15%) :white_check_mark: | 0.99 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 0.61 (15%) :white_check_mark: | 0.99 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 0.74 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 0.72 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (true, true))"]` | 0.74 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, false))"]` | 0.10 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, true))"]` | 0.11 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 0.11 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 0.11 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 0.13 (15%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 0.14 (15%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, false))"]` | 0.06 (15%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 0.07 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 0.07 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 0.09 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 0.10 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 0.10 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 0.08 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, true))"]` | 0.09 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 0.08 (15%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, false))"]` | 0.09 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 0.11 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 0.11 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 0.18 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, false)"]` | 0.17 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 0.19 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 0.17 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 0.19 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 0.08 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 0.09 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 0.14 (15%) :white_check_mark: | 0.36 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 0.15 (15%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 0.06 (15%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.08 (15%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 0.08 (15%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.08 (15%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int64, false)"]` | 0.08 (15%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 0.08 (15%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 0.07 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 0.07 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 0.55 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 0.54 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 1.02 (15%)  | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", BigInt, true)"]` | 1.09 (15%)  | 0.78 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Bool, false)"]` | 0.04 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.04 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, false)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Float32, false)"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Float64, false)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Int64, false)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, false)"]` | 0.55 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum3\", BigFloat, true)"]` | 0.55 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 1.00 (15%)  | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", BigInt, true)"]` | 1.08 (15%)  | 0.78 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 0.07 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 0.10 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, false)"]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Float32, false)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.05 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Float64, false)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Int64, true)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.10 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 0.53 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 0.52 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 0.91 (15%)  | 0.76 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", BigInt, true)"]` | 0.93 (15%)  | 0.75 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Bool, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Bool, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, false)"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Float32, false)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Float32, true)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Float64, false)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Float64, true)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Int64, false)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Int64, true)"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 0.00 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 0.00 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.61 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 0.59 (15%) :white_check_mark: | 1.08 (1%) :x: |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 1.13 (15%)  | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 1.22 (15%) :x: | 0.78 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, false)"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Float32, false)"]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Float64, false)"]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Int64, false)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Int64, true)"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |

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
- `["string"]`
- `["string", "readuntil"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta-Wut.150
Commit e1dfb30 (2018-07-04 17:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   38529142 s        278 s    4016968 s  811895230 s          8 s
       #2  3501 MHz  175347190 s          0 s    2469312 s  678738403 s          4 s
       #3  3501 MHz   24065421 s       2379 s    1992502 s  830109446 s         12 s
       #4  3501 MHz   22455499 s          0 s    2306688 s  831584604 s          8 s
       
  Memory: 31.383651733398438 GB (5049.5078125 MB free)
  Uptime: 8.570762e6 sec
  Load Avg:  1.0166015625  1.02197265625  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.4-pre.7
Commit df1c1c9 (2018-06-19 17:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5393.50390625 MB free)
Uptime: 8.579829e6 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   38622045 s        278 s    4028609 s  812693981 s          8 s
#2  3501 MHz  176201021 s          0 s    2479356 s  678780679 s          4 s
#3  3501 MHz   24154276 s       2379 s    2001634 s  830916718 s         12 s
#4  3501 MHz   22543105 s          0 s    2315484 s  832394277 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell MAX_THREADS=16)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
