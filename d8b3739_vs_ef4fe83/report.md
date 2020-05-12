# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d8b3739fa5dcfa6be5420fea6a9e20c55f42e61b](https://github.com/JuliaLang/julia/commit/d8b3739fa5dcfa6be5420fea6a9e20c55f42e61b) vs [JuliaLang/julia@ef4fe83698fb0d4cc5cc110164234eaf4b6d675e](https://github.com/JuliaLang/julia/commit/ef4fe83698fb0d4cc5cc110164234eaf4b6d675e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/35846#issuecomment-627136566)

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
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 1.03 (5%)  | 0.30 (1%) :white_check_mark: |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"BitArray\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat\", 5)"]` | 0.84 (5%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 1.00 (5%)  | 0.95 (1%) :white_check_mark: |
| `["array", "cat", "(\"vcat\", 500)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "4467"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"BitArray\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 256)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.09 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.15 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 1.27 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.85 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.77 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.05 (50%)  | 5.50 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.86 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.88 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.80 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.02 (50%)  | 5.50 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcartesian_view\", \"BitArray{2}\")"]` | 0.25 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.69 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.70 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.98 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.94 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.91 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 1.00 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.83 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.83 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.99 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.80 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.71 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.85 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Float32,2}\")"]` | 0.71 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Int32,2}\")"]` | 0.71 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.64 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.64 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.64 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.64 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.65 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.63 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BitArray{2}\")"]` | 0.73 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.70 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.78 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.72 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.47 (50%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.43 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.63 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.66 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.71 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.77 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.72 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.47 (50%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.43 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.64 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.65 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.69 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.67 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 0.89 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 0.91 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 0.94 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 0.95 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"1.0:1.0:100000.0\")"]` | 0.97 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"100000:-1:1\")"]` | 0.91 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"1:100000\")"]` | 0.96 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"Array{Float32,2}\")"]` | 0.17 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"Array{Int32,2}\")"]` | 0.14 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.26 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.26 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.27 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.25 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.25 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.26 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 0.66 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.16 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.72 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.17 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.22 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.36 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.25 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.30 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.15 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.73 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.17 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.23 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.35 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.26 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.28 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 1.08 (5%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"mean\", \"Int64\")"]` | 8.12 (5%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"perf_reduce\", \"Int64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"gramschmidt!\", 100)"]` | 0.94 (5%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"gramschmidt!\", 1000)"]` | 0.99 (5%)  | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"gramschmidt!\", 250)"]` | 0.98 (5%)  | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"gramschmidt!\", 500)"]` | 0.98 (5%)  | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.00 (5%)  | 0.98 (1%) :white_check_mark: |
| `["broadcast", "26942"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"IdDict\", \"Int\", \"filter!\")"]` | 1.00 (25%)  | 1.03 (1%) :x: |
| `["collection", "deletion", "(\"IdDict\", \"String\", \"filter!\")"]` | 0.80 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"IdDict\", \"String\", \"filter\")"]` | 0.85 (25%)  | 0.44 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter!\")"]` | 1.09 (25%)  | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 1.14 (25%)  | 1.29 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 1.41 (25%) :x: | 3.74 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 0.95 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\")"]` | 0.94 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.93 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"iterator\")"]` | 0.89 (25%)  | 1.01 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\")"]` | 0.88 (25%)  | 1.01 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.84 (25%)  | 1.01 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"iterator\")"]` | 1.13 (25%)  | 2.65 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\")"]` | 1.11 (25%)  | 2.65 (1%) :x: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\", \"sizehint!\")"]` | 1.16 (25%)  | 3.07 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 1.00 (25%)  | 1.17 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 1.00 (25%)  | 1.15 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 1.01 (25%)  | 1.17 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate second\")"]` | 0.55 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate\")"]` | 0.72 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate second\")"]` | 0.83 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate\")"]` | 0.81 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"iterate second\")"]` | 0.45 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"iterate\")"]` | 0.53 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate second\")"]` | 0.75 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate\")"]` | 0.74 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"iterate second\")"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Set\", \"Any\", \"iterate\")"]` | 0.41 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"iterate second\")"]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"iterate\")"]` | 0.42 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 0.99 (25%)  | 1.04 (1%) :x: |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Nothing\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Nothing\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"Nothing\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Bool\")"]` | 0.99 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Int8\")"]` | 1.00 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Nothing\")"]` | 0.73 (25%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Bool\")"]` | 0.99 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Int8\")"]` | 1.00 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Nothing\")"]` | 0.75 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"true\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"in\", \"false\")"]` | 0.23 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"new\")"]` | 0.31 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"new\")"]` | 0.31 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"overwrite\")"]` | 1.04 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"in\", \"false\")"]` | 0.57 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"push!\", \"new\")"]` | 0.65 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"setindex!\", \"new\")"]` | 0.68 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"setindex!\", \"overwrite\")"]` | 0.72 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"in\", \"false\")"]` | 0.52 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"push!\", \"new\")"]` | 0.66 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"new\")"]` | 0.66 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"overwrite\")"]` | 0.87 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"false\")"]` | 0.22 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 1.04 (25%)  | 2.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"new\")"]` | 0.26 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"first\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 0.93 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 0.42 (25%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"setindex!\")"]` | 0.85 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 0.03 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 0.83 (25%)  | 0.71 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.84 (25%)  | 0.68 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 0.84 (25%)  | 0.68 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.84 (25%)  | 0.64 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.26 (25%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.01 (25%)  | 1.03 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.91 (25%)  | 1.15 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.97 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.96 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 0.92 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.91 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 0.99 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.98 (25%)  | 0.98 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"DateTime\", \"Hour\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 0.92 (5%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.96 (5%)  | 0.88 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.98 (5%)  | 0.92 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.96 (5%)  | 0.88 (1%) :white_check_mark: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.88 (5%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "Date"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 1.22 (5%) :x: | 1.59 (1%) :x: |
| `["dates", "string", "DateTime"]` | 1.09 (5%) :x: | 1.21 (1%) :x: |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.03 (5%)  | 0.98 (1%) :white_check_mark: |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"50-50\")"]` | 0.92 (5%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.89 (5%) :white_check_mark: | 0.99 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.91 (5%) :white_check_mark: | 0.99 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.04 (5%)  | 0.96 (1%) :white_check_mark: |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.96 (5%)  | 0.96 (1%) :white_check_mark: |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,1}(100000000,)\")"]` | 3.70 (5%) :x: | 1.05 (1%) :x: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 3.13 (5%) :x: | 0.99 (1%) :white_check_mark: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(100000000, 1)\")"]` | 3.55 (5%) :x: | 1.05 (1%) :x: |
| `["io", "serialization", "(\"deserialize\", \"Vector{String}\")"]` | 2.36 (5%) :x: | 2.05 (1%) :x: |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 3.08 (5%) :x: | 2.23 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"Vector\", 1024)"]` | 0.21 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"Vector\", 256)"]` | 0.27 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"Vector\", 1024)"]` | 0.19 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"Vector\", 256)"]` | 0.30 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 1.44 (45%)  | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 1.40 (45%)  | 1.09 (1%) :x: |
| `["linalg", "small exp #29116"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["micro", "parseint"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "18129"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "20517"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Complex{Float32}"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "afoldl", "Complex{Float64}"]` | 0.20 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "afoldl", "Float64"]` | 0.19 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "afoldl", "Int"]` | 0.29 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "conditional"]` | 0.12 (5%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "allocation elision view", "no conditional"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1000)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["misc", "julia", "(\"macroexpand\", \"evalpoly\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 0.98 (5%)  | 1.05 (1%) :x: |
| `["misc", "parse", "Int"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "perf highdim generator"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 0.93 (5%) :white_check_mark: | 1.01 (1%)  |
| `["misc", "splatting", "(3, 3, 3)"]` | 0.66 (5%) :white_check_mark: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 0.85 (5%) :white_check_mark: | 1.03 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 0.84 (5%) :white_check_mark: | 1.01 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 0.84 (5%) :white_check_mark: | 1.03 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 0.85 (5%) :white_check_mark: | 1.03 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 0.89 (5%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["problem", "monte carlo", "euro_option_devec"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 0.79 (5%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["problem", "stockcorr", "stockcorr"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large BitSet\")"]` | 0.98 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 1.28 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.30 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small BitSet\")"]` | 0.81 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 1.31 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 1.31 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large BitSet\")"]` | 1.01 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 1.29 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 1.30 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small BitSet\")"]` | 0.81 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 1.29 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 1.32 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Vector\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large BitSet\")"]` | 0.89 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Dict\")"]` | 12.16 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 11.93 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small BitSet\")"]` | 0.89 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Dict\")"]` | 10.59 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 10.24 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large BitSet\")"]` | 0.82 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large String\")"]` | 0.77 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small BitSet\")"]` | 0.67 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small String\")"]` | 0.75 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large BitSet\")"]` | 0.68 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 0.86 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small BitSet\")"]` | 0.67 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small String\")"]` | 0.86 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"'a':'z'\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large BitSet\")"]` | 0.65 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large String\")"]` | 0.67 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small BitSet\")"]` | 0.66 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small String\")"]` | 0.67 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Vector\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 0.86 (25%)  | 0.54 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 0.97 (25%)  | 0.50 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 0.99 (25%)  | 0.54 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.01 (25%)  | 0.50 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:2^10000\")"]` | 0.90 (25%)  | 0.96 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 0.99 (25%)  | 0.50 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 0.72 (25%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Bool\")"]` | 0.16 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Float64\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"ImplicitRNG\", \"Float64\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float32\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float64\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"ImplicitRNG\", \"Float64\")"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float64\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.85 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.91 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.77 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.95 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.96 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.84 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 0.85 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Int64}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.95 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.83 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.89 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.89 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.83 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.86 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.85 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.96 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.92 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.84 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.98 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 0.82 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.98 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 0.81 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.95 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 0.93 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.88 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.95 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.90 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.87 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.88 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.86 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.85 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.90 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.86 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.93 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.87 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.87 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.86 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.87 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.90 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.87 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.91 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.85 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.87 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.86 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.90 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.83 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.87 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 0.91 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.80 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 0.87 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.86 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.86 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.86 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.90 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.87 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.90 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.88 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.95 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 0.94 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.86 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.87 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 1.05 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.98 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.85 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.86 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.86 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.87 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.91 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.96 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 1.00 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.96 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.92 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.97 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.97 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Int64\")"]` | 0.86 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.96 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.98 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.97 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.99 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigInt\")"]` | 0.95 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.97 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 0.94 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 1.06 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigInt}\")"]` | 1.01 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 1.74 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.92 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.98 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.96 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 0.88 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Int64}\")"]` | 1.01 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.95 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.87 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.84 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.81 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.91 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.85 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.85 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.69 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.83 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.96 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.90 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.91 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 0.97 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.97 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 0.85 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.87 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.92 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.91 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.91 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.89 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.94 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 0.96 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.98 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.96 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.96 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigInt}\")"]` | 0.99 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.99 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float64\")"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 1.70 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 0.84 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 0.79 (40%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 0.85 (40%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.87 (40%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 0.94 (40%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 0.97 (40%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 0.80 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigInt}\")"]` | 0.95 (40%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "revcomp"]` | 0.88 (25%)  | 0.87 (1%) :white_check_mark: |
| `["simd", "(\"auto_axpy!\", \"Float32\", 4095)"]` | 0.59 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Float32\", 4096)"]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Int32\", 4095)"]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"auto_axpy!\", \"Int32\", 4096)"]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int32\", 4095)"]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int32\", 4096)"]` | 0.47 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int64\", 4095)"]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"auto_conditional_loop!\", \"Int64\", 4096)"]` | 0.72 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 0.57 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4095)"]` | 0.46 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4096)"]` | 0.42 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4096)"]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float32\", 4095)"]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"inner\", \"Float32\", 4096)"]` | 0.71 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Float64\", 4095)"]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"inner_aliased\", \"Float64\", 4096)"]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 0.97 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 0.98 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 0.97 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 0.94 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 0.95 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 0.94 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 0.93 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 0.96 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 0.96 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 0.96 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 0.96 (20%)  | 0.00 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 1.01 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 1.04 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 1.04 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 1.01 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 0.96 (5%)  | 0.91 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 0.84 (5%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 0.95 (5%)  | 0.89 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 0.88 (5%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 0.98 (5%)  | 0.80 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 0.85 (5%) :white_check_mark: | 0.83 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 0.91 (5%) :white_check_mark: | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 0.95 (5%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 0.98 (5%)  | 0.99 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 0.94 (5%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.09 (5%) :x: | 0.99 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 10)"]` | 0.94 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 1.12 (30%)  | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 10)"]` | 0.92 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 100)"]` | 0.91 (30%)  | 0.75 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 1000)"]` | 0.97 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 0.88 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 0.90 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 1.04 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 0.98 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 0.94 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 100)"]` | 0.91 (30%)  | 0.75 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 1000)"]` | 0.91 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 0.99 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"logical\", 100)"]` | 0.97 (30%)  | 1.02 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 1000)"]` | 0.99 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"range\", 10)"]` | 0.93 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 10)"]` | 0.94 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 100)"]` | 0.92 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 0.83 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 0.99 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 0.91 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 0.77 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 0.90 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.00 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.84 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 10)"]` | 1.05 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 100)"]` | 0.90 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 0.81 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 2.90 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 97.14 (30%) :x: | 0.77 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 2.88 (30%) :x: | 0.87 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 1.00 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"logical\", 10000)"]` | 1.00 (30%)  | 1.02 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"range\", 1000)"]` | 1.01 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"range\", 10000)"]` | 1.08 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x50 -> dense 5x50\")"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x500, dense 500x5 -> dense 50x5\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "sparse solves", "least squares (default), matrix rhs"]` | 0.97 (5%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "least squares (default), vector rhs"]` | 0.98 (5%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "least squares (qr), matrix rhs"]` | 0.97 (5%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "least squares (qr), vector rhs"]` | 0.98 (5%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "square system (lu), matrix rhs"]` | 2.56 (5%) :x: | 2.38 (1%) :x: |
| `["sparse", "sparse solves", "square system (lu), vector rhs"]` | 1.87 (5%) :x: | 1.71 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 1.01 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint\", (20000, 10000))"]` | 0.82 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint\", (20000, 20000))"]` | 0.78 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint\", (600, 400))"]` | 0.78 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint\", (600, 600))"]` | 0.88 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose\", (20000, 10000))"]` | 0.78 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 0.82 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (600, 400))"]` | 0.78 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (600, 600))"]` | 0.78 (30%)  | 0.00 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 1000"]` | 0.96 (5%)  | 0.80 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 2"]` | 0.98 (5%)  | 0.80 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 50000"]` | 0.96 (5%)  | 0.80 (1%) :white_check_mark: |
| `["tuple", "linear algebra", "(\"matmat\", (16, 16), (16, 16))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (2, 2))"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4,))"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.05 (5%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.05 (5%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 0.60 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.61 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 0.64 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 0.54 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 0.66 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.63 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 0.56 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 0.67 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 0.56 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.63 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 0.64 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 0.61 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.77 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 0.64 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 0.63 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 0.59 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.52 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, false)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, false)"]` | 1.67 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.36 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, false)"]` | 0.39 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 0.39 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.04 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 0.02 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, true)"]` | 1.60 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, false)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, BigFloat}, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, BigInt}, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, BigFloat}, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Float32}, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Float64}, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Int64}, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 0.44 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 1.31 (5%) :x: | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Complex{Float64}}, true)"]` | 1.22 (5%) :x: | 1.14 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float32}, true)"]` | 0.89 (5%) :white_check_mark: | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 1.29 (5%) :x: | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Int64}, true)"]` | 0.91 (5%) :white_check_mark: | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Int8}, true)"]` | 1.00 (5%)  | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Bool}, false)"]` | 1.90 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Complex{Float64}}, false)"]` | 1.51 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Float32}, false)"]` | 1.51 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Float64}, false)"]` | 1.51 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Int8}, false)"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Bool, false)"]` | 0.50 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Bool}, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Float32}, false)"]` | 1.40 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.6.0-DEV.22
Commit d8b3739 (2020-05-12 06:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   57938947 s       2449 s   20360912 s  6610720561 s         19 s
       #2  3501 MHz  362724949 s         62 s    7630988 s  6336751082 s         27 s
       #3  3501 MHz   49040064 s       3236 s    5796378 s  6650311783 s         40 s
       #4  3501 MHz   47247272 s         19 s    4477035 s  6657467663 s         37 s
       
  Memory: 31.383651733398438 GB (18936.91796875 MB free)
  Uptime: 6.7110456e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.2-pre.0
Commit ef4fe83 (2020-04-15 16:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   58066558 s       2449 s   20370744 s  6611974732 s         19 s
       #2  3501 MHz  364022682 s         62 s    7656924 s  6336823971 s         27 s
       #3  3501 MHz   49167148 s       3236 s    5801757 s  6651574965 s         40 s
       #4  3501 MHz   47377165 s         19 s    4482331 s  6658728950 s         37 s
       
  Memory: 31.383651733398438 GB (18732.0703125 MB free)
  Uptime: 6.7124425e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-8.0.1 (ORCJIT, haswell)

```
