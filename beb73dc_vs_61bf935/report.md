# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@beb73dc968059daf74d37e2439d9b010d36fc093](https://github.com/JuliaLang/julia/commit/beb73dc968059daf74d37e2439d9b010d36fc093) vs [JuliaLang/julia@61bf9359e9d1dcc52ccdd77c3f502045d0b92c0c](https://github.com/JuliaLang/julia/commit/61bf9359e9d1dcc52ccdd77c3f502045d0b92c0c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25261#issuecomment-372147115)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1} generator\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1}\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Vector{Bool}\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1} generator\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1}\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Vector{Bool}\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_fill!"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_fill!"]` | 7.29 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_load!"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 500)"]` | 34.08 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 51.16 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 13.46 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 98.07 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 13.57 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 87.23 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 13.57 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 86.69 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 5.34 (15%) :x: | 1.17 (1%) :x: |
| `["array", "cat", "(\"vcat\", 500)"]` | 86.21 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 13.46 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 87.17 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "convert", "(\"Complex{Float64}\", \"Int\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Float64\", \"Int\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float32,1}\")"]` | 5.60 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 4.94 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 5.03 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float64,1}\")"]` | 4.00 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Int16,1}\")"]` | 7.82 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 4.85 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 8.58 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float32,1}\")"]` | 4.65 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float64,1}\")"]` | 4.44 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int16,1}\")"]` | 7.65 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 2.79 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float64,1}\")"]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int16,1}\")"]` | 8.31 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 4.85 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 5.21 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"BitArray\")"]` | 5.55 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Bool}\")"]` | 8.68 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 2.33 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcolon\", \"100000:-1:1\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Float32,2}\")"]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Int32,2}\")"]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 2.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.26 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.24 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.46 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.93 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.45 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.22 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.56 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.23 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"100000:-1:1\")"]` | 119.22 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"1:100000\")"]` | 211.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"Array{Int32,2}\")"]` | 4.09 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 4.11 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 5.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"1:100000\")"]` | 64.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"Array{Int32,2}\")"]` | 7.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Int32,2}\")"]` | 6.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"100000:-1:1\")"]` | 123.23 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"1:100000\")"]` | 211.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"Array{Int32,2}\")"]` | 4.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 4.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 5.77 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"100000:-1:1\")"]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"1:100000\")"]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Float32,2}\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Int32,2}\")"]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 2.62 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.41 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.49 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.49 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.35 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.56 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "sub2ind"]` | 19.51 (50%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Int64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_fast!"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 0.89 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 0.94 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 0.90 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.90 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 0.95 (15%)  | 1.18 (1%) :x: |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.61 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter!\")"]` | 1.61 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter\")"]` | 1.27 (25%) :x: | 2.56 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 7.24 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"pop!\")"]` | 47.37 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter!\")"]` | 1.36 (25%) :x: | 2.00 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter\")"]` | 1.28 (25%) :x: | 1.56 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 29.81 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter!\")"]` | 6.67 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 5.58 (25%) :x: | 3.49 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 39.26 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 47.99 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter!\")"]` | 1.52 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 1.12 (25%)  | 3.34 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 38.45 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 56.24 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter\")"]` | 23.13 (25%) :x: | 7.02 (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.56 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter\")"]` | 1.81 (25%) :x: | 2.90 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 2.38 (25%) :x: | 1.45 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\")"]` | 2.72 (25%) :x: | 1.49 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 2.95 (25%) :x: | 1.53 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["collection", "initialization", "(\"Dict\", \"String\", \"iterator\")"]` | 1.14 (25%)  | 1.34 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\")"]` | 1.16 (25%)  | 1.34 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\", \"sizehint!\")"]` | 1.09 (25%)  | 1.36 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 2.99 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 2.65 (25%) :x: | 1.63 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 2.95 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"iterator\")"]` | 1.17 (25%)  | 1.68 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\")"]` | 1.25 (25%)  | 1.63 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\", \"sizehint!\")"]` | 1.23 (25%)  | 1.68 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\")"]` | 19.27 (25%) :x: | 4.07 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\", \"sizehint!\")"]` | 19.96 (25%) :x: | 7.35 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\")"]` | 1.53 (25%) :x: | 2.90 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\", \"sizehint!\")"]` | 1.61 (25%) :x: | 4.93 (1%) :x: |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 3.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"next\")"]` | 1.00 (25%)  | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"start\")"]` | 20.61 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"start\")"]` | 23.84 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"next\")"]` | 1.00 (25%)  | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"start\")"]` | 20.47 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"next\")"]` | 1.67 (25%) :x: | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"start\")"]` | 21.75 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"start\")"]` | 20.18 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"next\")"]` | 1.00 (25%)  | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"start\")"]` | 23.84 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"next\")"]` | 1.67 (25%) :x: | 3.50 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"start\")"]` | 8.83 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"start\")"]` | 7.67 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"next\")"]` | 1.00 (25%)  | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"start\")"]` | 7.67 (25%) :x: | Inf (1%) :x: |
| `["collection", "optimizations", "(\"BitSet\", \"Int8\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 1.24 (25%)  | 1.86 (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 1.13 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"unspecified\")"]` | 1.00 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 7.22 (25%) :x: | 4.23 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 7.14 (25%) :x: | 3.22 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 4.10 (25%) :x: | 2001.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 3.50 (25%) :x: | 1793.00 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 0.91 (25%)  | 0.78 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 1.00 (25%)  | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 1.00 (25%)  | 1.55 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 1.00 (25%)  | 1.48 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.00 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.00 (25%)  | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.23 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.35 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.27 (25%) :x: | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.43 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.00 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.00 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.10 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 1.00 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.05 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.07 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.98 (25%)  | 1.01 (1%) :x: |
| `["dates", "arithmetic", "(\"DateTime\", \"Millisecond\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Second\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.26 (15%) :x: | 1.25 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 13.94 (15%) :x: | 11.88 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 8.66 (15%) :x: | 4.12 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 7.87 (15%) :x: | 3.59 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 7.04 (15%) :x: | 4.12 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.06 (15%)  | 1.22 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 4.72 (15%) :x: | 3.85 (1%) :x: |
| `["dates", "parse", "Date"]` | 6.01 (15%) :x: | 3.85 (1%) :x: |
| `["dates", "parse", "DateTime"]` | 28.59 (15%) :x: | 11.88 (1%) :x: |
| `["dates", "string", "Date"]` | 1.28 (15%) :x: | 2.17 (1%) :x: |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.82 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 2.39 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 1.05 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.17 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 0.95 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.96 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.53 (45%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "axpy!"]` | 2.09 (40%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "scal!"]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 1024)"]` | 5.04 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 256)"]` | 12.32 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 1.14 (45%)  | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 1.14 (45%)  | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 1024)"]` | 1.14 (45%)  | 1.08 (1%) :x: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 256)"]` | 1.14 (45%)  | 1.09 (1%) :x: |
| `["micro", "mandel"]` | 5.62 (15%) :x: | 65.19 (1%) :x: |
| `["micro", "parseint"]` | 1.19 (15%) :x: | 1.13 (1%) :x: |
| `["micro", "randmatstat"]` | 2.14 (15%) :x: | 1.00 (1%)  |
| `["misc", "afoldl", "Complex{Float64}"]` | 0.87 (15%)  | 1.03 (1%) :x: |
| `["misc", "afoldl", "Float64"]` | 0.88 (15%)  | 1.03 (1%) :x: |
| `["misc", "afoldl", "Int"]` | 0.96 (15%)  | 1.03 (1%) :x: |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["misc", "parse", "DateTime"]` | 17.56 (15%) :x: | 10.34 (1%) :x: |
| `["misc", "parse", "Float64"]` | 1.02 (15%)  | 1.03 (1%) :x: |
| `["misc", "parse", "Int"]` | 25.18 (15%) :x: | 48.21 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 0.99 (15%)  | 1.04 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.03 (15%)  | 1.07 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.07 (15%)  | 1.02 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.03 (15%)  | 1.05 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.05 (15%)  | 1.07 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 2.08 (15%) :x: | 3.32 (1%) :x: |
| `["problem", "json", "parse_json"]` | 1.30 (15%) :x: | 1.18 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 6.26 (15%) :x: | 9.71 (1%) :x: |
| `["problem", "simplex", "simplex"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 3.01 (15%) :x: | 2.14 (1%) :x: |
| `["scalar", "iteration", "in"]` | 11626.04 (25%) :x: | 1.00 (1%)  |
| `["scalar", "iteration", "indexed"]` | 46039.13 (25%) :x: | 1.00 (1%)  |
| `["shootout", "fasta"]` | 1.07 (15%)  | 1.01 (1%) :x: |
| `["shootout", "k_nucleotide"]` | 1.47 (15%) :x: | 1.42 (1%) :x: |
| `["shootout", "mandelbrot"]` | 1.01 (15%)  | 1.05 (1%) :x: |
| `["shootout", "meteor_contest"]` | 0.96 (15%)  | 1.01 (1%) :x: |
| `["shootout", "nbody"]` | 1.34 (15%) :x: | 358.50 (1%) :x: |
| `["shootout", "nbody_vec"]` | 1.17 (15%) :x: | 2.41 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ascending\")"]` | 2.36 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ones\")"]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"descending\")"]` | 2.80 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ones\")"]` | 1.99 (30%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"forwards\", \"ascending\")"]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 2.20 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ascending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"descending\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 1.00 (15%)  | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 1.06 (15%)  | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 1.06 (15%)  | 1.06 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 1.72 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 1.78 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 1.70 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x40, sparse 400x40 -> dense 400x400\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 1.58 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.74 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["string", "replace"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.02 (15%)  | 1.07 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 0.80 (15%) :white_check_mark: | 1.01 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 0.81 (15%) :white_check_mark: | 1.01 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.94 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 0.98 (15%)  | 1.03 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 1.07 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.00 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 0.91 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 0.99 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.03 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 2.99 (15%) :x: | 2.62 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 2.99 (15%) :x: | 2.63 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 3.11 (15%) :x: | 2.64 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 3.08 (15%) :x: | 2.99 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 3.03 (15%) :x: | 2.97 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 3.12 (15%) :x: | 2.99 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 4.51 (15%) :x: | 13.12 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 4.47 (15%) :x: | 11.65 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 4.51 (15%) :x: | 12.50 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 3.89 (15%) :x: | 2.80 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 3.74 (15%) :x: | 2.65 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 3.83 (15%) :x: | 2.70 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 4.42 (15%) :x: | 4.28 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 4.06 (15%) :x: | 4.14 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 3.93 (15%) :x: | 4.26 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 4.12 (15%) :x: | 3.72 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 3.83 (15%) :x: | 3.54 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 4.01 (15%) :x: | 3.61 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 4.25 (15%) :x: | 3.72 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 3.79 (15%) :x: | 3.54 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 3.77 (15%) :x: | 3.61 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 4.16 (15%) :x: | 13.12 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 4.12 (15%) :x: | 11.65 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 4.22 (15%) :x: | 12.50 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 7.13 (15%) :x: | 1.91 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 6.71 (15%) :x: | 1.88 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 8.70 (15%) :x: | 3.75 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 7.74 (15%) :x: | 3.25 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 89.11 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 37.53 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 45.45 (15%) :x: | 23.49 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 27.64 (15%) :x: | 10.86 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 82.18 (15%) :x: | 37.15 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 34.89 (15%) :x: | 16.12 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 80.84 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 34.82 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 81.14 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 35.18 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 87.03 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 37.08 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 57.79 (15%) :x: | 11.73 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 26.47 (15%) :x: | 6.17 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 57.71 (15%) :x: | 11.73 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 25.96 (15%) :x: | 6.17 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 90.30 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 37.90 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 39.26 (15%) :x: | 14.34 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 27.07 (15%) :x: | 7.00 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 84.22 (15%) :x: | 37.15 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 35.41 (15%) :x: | 16.12 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 82.53 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 34.95 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 96.41 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 33.23 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 94.55 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 37.46 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 87.82 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 99.26 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 97.12 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 102.56 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 87.16 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 68.32 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 84.87 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 74.94 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 87.70 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 66.15 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 89.75 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 76.21 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 90.06 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 71.29 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 86.50 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 75.00 (15%) :x: | Inf (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

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
Julia Version 0.7.0-DEV.4540
Commit beb73dc (2018-03-11 20:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110604648 s          0 s   17263602 s  5504621468 s        288 s
       #2  3501 MHz  451595357 s          0 s   18356933 s  5165978264 s         89 s
       #3  3501 MHz   87773116 s          0 s    9988608 s  5545668444 s        131 s
       #4  3501 MHz   82935060 s          0 s   10001066 s  5550885255 s         54 s
       
  Memory: 31.383651733398438 GB (6887.8046875 MB free)
  Uptime: 5.64564e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4537
Commit 61bf935 (2018-03-11 19:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110696138 s          0 s   17274718 s  5505445660 s        288 s
       #2  3501 MHz  452466462 s          0 s   18367630 s  5166025521 s         89 s
       #3  3501 MHz   87864957 s          0 s    9996725 s  5546498168 s        132 s
       #4  3501 MHz   83022530 s          0 s   10008974 s  5551719791 s         54 s
       
  Memory: 31.383651733398438 GB (5842.046875 MB free)
  Uptime: 5.6465705e7 sec
  Load Avg:  1.02783203125  1.02490234375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
