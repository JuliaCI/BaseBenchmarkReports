# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0bab06f8a7f70d4518ad30e19a4c0a1968c875ad](https://github.com/JuliaLang/julia/commit/0bab06f8a7f70d4518ad30e19a4c0a1968c875ad)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/0bab06f8a7f70d4518ad30e19a4c0a1968c875ad#commitcomment-38788175)

*Tag Predicate:* `ALL`

*Daily Job:* 2020-04-28 vs 2020-04-27

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
| `["array", "cat", "(\"hcat\", 5)"]` | 0.95 (5%)  | 0.95 (1%) :white_check_mark: |
| `["array", "cat", "(\"vcat\", 5)"]` | 0.99 (5%)  | 0.95 (1%) :white_check_mark: |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.66 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.09 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.15 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 1.27 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.81 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.93 (50%)  | 5.50 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.86 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.93 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.05 (50%)  | 5.50 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.62 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.76 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.97 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 1.02 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.95 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.94 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.92 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 0.97 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.79 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.82 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.92 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.94 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.84 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.89 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.00 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Float32,2}\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"Array{Int32,2}\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.85 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"BitArray{2}\")"]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.89 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.72 (50%)  | 0.55 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.72 (50%)  | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.89 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.88 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.73 (50%)  | 0.55 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.79 (50%)  | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.58 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.71 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 0.88 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 0.94 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 0.92 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 0.91 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"1.0:1.0:100000.0\")"]` | 0.88 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"100000:-1:1\")"]` | 0.96 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"1:100000\")"]` | 0.93 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"Array{Float32,2}\")"]` | 0.15 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"Array{Int32,2}\")"]` | 0.15 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.61 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.59 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 0.65 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 0.59 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 0.62 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 0.59 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 0.65 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.16 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.68 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.15 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.21 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.64 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.59 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.62 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.14 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 0.66 (50%)  | 0.80 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.15 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.21 (50%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.69 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.61 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.60 (50%)  | 0.01 (1%) :white_check_mark: |
| `["array", "reductions", "(\"perf_mapreduce\", \"Int64\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"gramschmidt!\", 100)"]` | 0.94 (5%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"gramschmidt!\", 1000)"]` | 0.99 (5%)  | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"gramschmidt!\", 250)"]` | 0.99 (5%)  | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"gramschmidt!\", 500)"]` | 0.98 (5%)  | 0.00 (1%) :white_check_mark: |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.04 (5%)  | 0.98 (1%) :white_check_mark: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"IdDict\", \"String\", \"filter!\")"]` | 0.84 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"IdDict\", \"String\", \"filter\")"]` | 0.90 (25%)  | 0.44 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter!\")"]` | 0.99 (25%)  | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 1.14 (25%)  | 1.29 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 1.09 (25%)  | 1.22 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 1.08 (25%)  | 1.20 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 1.09 (25%)  | 1.22 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate second\")"]` | 0.78 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate\")"]` | 0.92 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate second\")"]` | 0.89 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate\")"]` | 0.88 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"iterate second\")"]` | 0.88 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"iterate\")"]` | 0.88 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate second\")"]` | 0.86 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate\")"]` | 0.81 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Bool\")"]` | 0.99 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Int8\")"]` | 1.02 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Nothing\")"]` | 0.94 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Bool\")"]` | 0.99 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Int8\")"]` | 1.02 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Nothing\")"]` | 0.93 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"in\", \"true\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 1.06 (25%)  | 2.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"specified\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"new\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"overwrite\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 1.00 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.98 (25%)  | 0.93 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 0.98 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.06 (25%)  | 1.03 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.06 (25%)  | 1.15 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.96 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.98 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 0.94 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.92 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 0.97 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.97 (25%)  | 0.98 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.02 (5%)  | 0.87 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.95 (5%)  | 0.88 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.86 (5%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.98 (5%)  | 0.88 (1%) :white_check_mark: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.98 (5%)  | 0.89 (1%) :white_check_mark: |
| `["dates", "query", "(\"daysofweekinmonth\", \"Date\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"50-50\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.94 (5%) :white_check_mark: | 0.99 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.93 (5%) :white_check_mark: | 0.99 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,1}(100000000,)\")"]` | 1.02 (5%)  | 1.02 (1%) :x: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 1.04 (5%)  | 1.01 (1%) :x: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(100000000, 1)\")"]` | 1.03 (5%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 1.41 (45%)  | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 1.36 (45%)  | 1.09 (1%) :x: |
| `["micro", "parseint"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "printfd"]` | 1.00 (5%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "allocation elision view", "conditional"]` | 0.19 (5%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc", "allocation elision view", "no conditional"]` | 1.30 (5%) :x: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.01 (5%)  | 1.04 (1%) :x: |
| `["misc", "repeat", "(200, 1, 24)"]` | 1.07 (5%) :x: | 1.01 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 0.98 (5%)  | 0.98 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.01 (5%)  | 0.99 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 0.99 (5%)  | 0.98 (1%) :white_check_mark: |
| `["problem", "imdb", "centrality"]` | 0.88 (5%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 0.79 (5%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large BitSet\")"]` | 1.11 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 1.06 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.02 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small BitSet\")"]` | 1.08 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 1.06 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 0.94 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large BitSet\")"]` | 1.06 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 1.03 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 1.03 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small BitSet\")"]` | 1.04 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 1.03 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 0.94 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large BitSet\")"]` | 1.04 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Dict\")"]` | 0.99 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small BitSet\")"]` | 1.05 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Dict\")"]` | 0.99 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 0.97 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large BitSet\")"]` | 0.96 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large String\")"]` | 0.93 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small BitSet\")"]` | 0.89 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small String\")"]` | 0.87 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large BitSet\")"]` | 1.02 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 0.92 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small BitSet\")"]` | 0.95 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small String\")"]` | 0.92 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large BitSet\")"]` | 1.04 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large String\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small BitSet\")"]` | 0.99 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small String\")"]` | 0.99 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 1.01 (25%)  | 0.54 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 0.99 (25%)  | 0.50 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 1.02 (25%)  | 0.54 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.01 (25%)  | 0.50 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:2^10000\")"]` | 1.07 (25%)  | 0.96 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 1.01 (25%)  | 0.50 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 1.03 (25%)  | 0.50 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt8\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"Float64\")"]` | 1.64 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 1.06 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 1.17 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 1.08 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 1.03 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 1.09 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 1.11 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 1.06 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.88 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 1.07 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 1.14 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Int64}\")"]` | 0.96 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.95 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 1.06 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 1.10 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 1.04 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 1.10 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 1.06 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 1.08 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.86 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 1.09 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 1.08 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 1.08 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 1.17 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.14 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 1.09 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 1.07 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 1.05 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.97 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.97 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 1.12 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 1.11 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 0.98 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.96 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 1.06 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 1.33 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 1.07 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 1.06 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 1.14 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 1.11 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 1.07 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 1.10 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 0.93 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 1.07 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 1.04 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.96 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 1.10 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 1.05 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 1.07 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigInt}\")"]` | 0.99 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 1.06 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.98 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 1.02 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.93 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.96 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 1.02 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 1.02 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.90 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.94 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.95 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.96 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.94 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 1.02 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 1.00 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.96 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 1.00 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 1.03 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 1.06 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 1.10 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 1.13 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 1.19 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 1.18 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 1.25 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.03 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 1.00 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.99 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 1.02 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 1.17 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 1.10 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.24 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 1.00 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.94 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 1.05 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 1.11 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 0.99 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.98 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 1.13 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 1.07 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.99 (50%)  | 0.96 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.98 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 1.07 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.94 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 1.07 (50%)  | 0.90 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 1.06 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 1.15 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 1.10 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 1.24 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 1.18 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 1.13 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 1.07 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 0.98 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 1.06 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 1.06 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 1.09 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 1.00 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 1.06 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 1.07 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 1.10 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 1.16 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 1.21 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 1.07 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.98 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 1.29 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.91 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 1.12 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 1.03 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.95 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.96 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 1.06 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 1.08 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Int64\")"]` | 0.97 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.82 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 1.08 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 1.09 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.92 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 1.11 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 1.17 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigInt\")"]` | 0.82 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.97 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 1.21 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.97 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 1.05 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 1.10 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 1.06 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 1.05 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 1.06 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 1.24 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 1.09 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 1.19 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.93 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 1.15 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 1.14 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 1.10 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 1.01 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 1.09 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 1.07 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 1.12 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.99 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 1.08 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 1.08 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Int64}\")"]` | 0.94 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.86 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 1.08 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.95 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 1.09 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 1.13 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 1.21 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.96 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 1.08 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 1.06 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 1.06 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 1.09 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 1.07 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 1.07 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 1.15 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.96 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 1.15 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 1.05 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 1.10 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.94 (50%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 0.97 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 1.16 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 0.96 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.96 (50%)  | 0.60 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 1.02 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 1.14 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 1.03 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 1.17 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 1.04 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 1.19 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 1.18 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 1.13 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 1.00 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 0.98 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 1.07 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 1.00 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 1.09 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.96 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.99 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 1.22 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 1.11 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 1.04 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 1.06 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 1.93 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 1.13 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigInt}\")"]` | 0.96 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.98 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"negative argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float32\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float32\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float32\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float32\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 1.69 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.48 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.56 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.63 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float64\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"one\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 1.04 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 0.92 (40%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 0.99 (40%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.96 (40%)  | 0.97 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 1.08 (40%)  | 0.95 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 0.95 (40%)  | 0.89 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 1.06 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigInt}\")"]` | 0.94 (40%)  | 0.73 (1%) :white_check_mark: |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2.0^-28\", \"negative argument\", \"Float64\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"2.0^-28 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "revcomp"]` | 0.97 (25%)  | 0.87 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 0.98 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 1.00 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 0.99 (20%)  | 0.00 (1%) :white_check_mark: |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 1.67 (20%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 0.99 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 1.00 (30%)  | 0.33 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 0.98 (5%)  | 0.91 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 0.94 (5%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 0.95 (5%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 0.98 (5%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 1.00 (5%)  | 0.80 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 1.02 (5%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 1.09 (5%) :x: | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 0.99 (5%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.03 (5%)  | 0.99 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 0.98 (5%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.00 (5%)  | 0.99 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 10)"]` | 1.03 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 1.00 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 10)"]` | 0.94 (30%)  | 0.70 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 100)"]` | 0.93 (30%)  | 0.75 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 1000)"]` | 0.88 (30%)  | 0.84 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 1.00 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 1.06 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 0.99 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 1.00 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 0.98 (30%)  | 0.70 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 100)"]` | 0.94 (30%)  | 0.75 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 1000)"]` | 0.92 (30%)  | 0.84 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 1.04 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"range\", 10)"]` | 1.03 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 10)"]` | 0.94 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 100)"]` | 0.94 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 1.03 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 0.97 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 1.00 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 0.99 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 0.96 (30%)  | 0.86 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.00 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.98 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 10)"]` | 0.98 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 100)"]` | 1.03 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 0.94 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 0.90 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 0.92 (30%)  | 0.77 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 1.00 (30%)  | 0.87 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 0.95 (30%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"range\", 1000)"]` | 1.01 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"range\", 10000)"]` | 1.00 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "least squares (default), matrix rhs"]` | 0.99 (5%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "least squares (default), vector rhs"]` | 0.99 (5%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "least squares (qr), matrix rhs"]` | 0.98 (5%)  | 0.93 (1%) :white_check_mark: |
| `["sparse", "sparse solves", "least squares (qr), vector rhs"]` | 0.99 (5%)  | 0.95 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 0.99 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 0.99 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint\", (20000, 10000))"]` | 0.83 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint\", (20000, 20000))"]` | 0.88 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint\", (600, 400))"]` | 0.82 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint\", (600, 600))"]` | 0.83 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 1.00 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 0.99 (30%)  | 4.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose\", (20000, 10000))"]` | 0.83 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 0.88 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (600, 400))"]` | 0.83 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (600, 600))"]` | 0.88 (30%)  | 0.00 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 1000"]` | 0.99 (5%)  | 0.80 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 2"]` | 0.88 (5%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 50000"]` | 1.00 (5%)  | 0.80 (1%) :white_check_mark: |
| `["string", "repeat", "repeat char 2"]` | 0.58 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (8, 8), (8, 8))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (16, 16), (16,))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.00 (5%)  | 0.96 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.00 (5%)  | 0.98 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.00 (5%)  | 0.98 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 0.72 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 0.77 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 0.62 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 0.60 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 0.67 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 0.57 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 1.32 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.48 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 1.41 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.41 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, BigFloat, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, Complex{Float64}}, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Bool}, true)"]` | 1.00 (5%)  | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Complex{Float64}}, true)"]` | 1.00 (5%)  | 1.14 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float32}, true)"]` | 0.74 (5%) :white_check_mark: | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 0.99 (5%)  | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Int64}, true)"]` | 1.02 (5%)  | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Int8}, true)"]` | 0.99 (5%)  | 1.20 (1%) :x: |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, BigInt}, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 1.5.0-DEV.696
Commit 0bab06f (2020-04-27 22:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  136135581 s       5056 s   15552492 s  6423044459 s         35 s
       #2  3501 MHz  1024963482 s        217 s   20097204 s  5539723838 s         26 s
       #3  3501 MHz  120926352 s       3296 s    9216570 s  6453851952 s         38 s
       #4  3501 MHz  113556245 s         43 s   13254781 s  6455497036 s         27 s
       
  Memory: 31.383651733398438 GB (19144.40234375 MB free)
  Uptime: 6.5896071e7 sec
  Load Avg:  1.224609375  1.06298828125  1.06005859375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
