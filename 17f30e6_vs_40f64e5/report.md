# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@17f30e6f6dfb6b62bae4dfb3e5bd89d6ab3ce823](https://github.com/JuliaLang/julia/commit/17f30e6f6dfb6b62bae4dfb3e5bd89d6ab3ce823) vs [JuliaLang/julia@40f64e590ffd3f03836a7a2b13c53b86be4a7856](https://github.com/JuliaLang/julia/commit/40f64e590ffd3f03836a7a2b13c53b86be4a7856)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25261#issuecomment-372077184)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1} generator\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1}\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Vector{Bool}\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1} generator\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1}\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Vector{Bool}\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_fill!"]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_fill!"]` | 8.23 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_load!"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 500)"]` | 32.80 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 50.97 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 13.35 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 97.64 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 13.68 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 88.96 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 13.57 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 89.71 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 5.37 (15%) :x: | 1.17 (1%) :x: |
| `["array", "cat", "(\"vcat\", 500)"]` | 86.46 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 13.46 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 87.50 (15%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Complex{Float64}\", \"Int\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Float64\", \"Int\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float32,1}\")"]` | 5.57 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 4.89 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 4.91 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float64,1}\")"]` | 3.97 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Int16,1}\")"]` | 7.82 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 4.85 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 9.06 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float32,1}\")"]` | 4.70 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float64,1}\")"]` | 4.22 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int16,1}\")"]` | 8.14 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 2.80 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float64,1}\")"]` | 2.27 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int16,1}\")"]` | 7.82 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 5.35 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 5.63 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"BitArray\")"]` | 5.55 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Vector{Bool}\")"]` | 8.63 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 2.46 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcolon\", \"1.0:0.00010001000100010001:2.0\")"]` | 31.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"1.0:1.0:100000.0\")"]` | 32.20 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"100000:-1:1\")"]` | 105.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"1:100000\")"]` | 106.11 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Float32,2}\")"]` | 98.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"Array{Int32,2}\")"]` | 100.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 111.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 99.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 93.29 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 95.62 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 98.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 98.12 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 94.49 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 92.95 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 71.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.46 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 5.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 97.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 73.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 98.21 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 97.40 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 71.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 5.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 100.32 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 73.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"100000:-1:1\")"]` | 123.22 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"1:100000\")"]` | 212.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"Array{Int32,2}\")"]` | 3.49 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 4.15 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 5.60 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"1:100000\")"]` | 54.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"Array{Int32,2}\")"]` | 6.68 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Int32,2}\")"]` | 6.26 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"100000:-1:1\")"]` | 123.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"1:100000\")"]` | 211.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"Array{Int32,2}\")"]` | 4.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 4.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 4.91 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"1.0:0.00010001000100010001:2.0\")"]` | 15.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"1.0:1.0:100000.0\")"]` | 15.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"100000:-1:1\")"]` | 18.03 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"1:100000\")"]` | 21.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 24.00 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 24.22 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 22.47 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 22.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 24.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 24.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 24.12 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 24.40 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 17.75 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 18.02 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 18.92 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 24.19 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 18.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 18.02 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 17.95 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 19.02 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 23.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 18.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 21.10 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 21.43 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"1.0:0.00010001000100010001:2.0\")"]` | 30.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"1.0:1.0:100000.0\")"]` | 32.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"100000:-1:1\")"]` | 106.20 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"1:100000\")"]` | 105.43 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Float32,2}\")"]` | 99.07 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"Array{Int32,2}\")"]` | 97.06 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 99.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 93.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 92.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 91.93 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 98.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 99.23 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 109.25 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 94.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 70.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.75 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 102.14 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 72.64 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 94.18 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 99.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 71.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.87 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 100.07 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 72.48 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"Array{Float32,2}\")"]` | 8.49 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"Array{Int32,2}\")"]` | 7.86 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 9.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 7.93 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 8.66 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 8.03 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 7.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 9.39 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 9.49 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 8.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 6.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.41 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.17 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.51 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 7.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 9.60 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 9.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.62 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 8.06 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.90 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 5.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 5.99 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "7d"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "sub2ind"]` | 19.82 (50%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norm1\", \"Int64\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_fast!"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 1.00 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 0.94 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 0.95 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.95 (15%)  | 1.18 (1%) :x: |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 0.95 (15%)  | 1.18 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 19.98 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 5.69 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 6.66 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 5.89 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.61 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter!\")"]` | 1.57 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter\")"]` | 1.35 (25%) :x: | 2.56 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 7.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"pop!\")"]` | 45.92 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter!\")"]` | 1.35 (25%) :x: | 2.00 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter\")"]` | 1.19 (25%)  | 1.56 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 29.65 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter!\")"]` | 7.10 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 5.52 (25%) :x: | 3.49 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 41.01 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 47.99 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter!\")"]` | 1.37 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 1.08 (25%)  | 3.34 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 38.14 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 56.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter\")"]` | 23.60 (25%) :x: | 7.02 (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.86 (25%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter\")"]` | 1.65 (25%) :x: | 2.90 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 2.35 (25%) :x: | 1.45 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\")"]` | 2.57 (25%) :x: | 1.49 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 2.84 (25%) :x: | 1.53 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"iterator\")"]` | 1.10 (25%)  | 1.34 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\")"]` | 1.12 (25%)  | 1.34 (1%) :x: |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\", \"sizehint!\")"]` | 1.13 (25%)  | 1.36 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 3.05 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 2.66 (25%) :x: | 1.63 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 2.95 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"iterator\")"]` | 1.17 (25%)  | 1.68 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\")"]` | 1.16 (25%)  | 1.63 (1%) :x: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\", \"sizehint!\")"]` | 1.18 (25%)  | 1.68 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\")"]` | 19.99 (25%) :x: | 4.07 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\", \"sizehint!\")"]` | 20.23 (25%) :x: | 7.35 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\")"]` | 1.57 (25%) :x: | 2.90 (1%) :x: |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\", \"sizehint!\")"]` | 1.65 (25%) :x: | 4.93 (1%) :x: |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 3.15 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"next\")"]` | 1.00 (25%)  | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"start\")"]` | 20.61 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"start\")"]` | 24.33 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"next\")"]` | 1.00 (25%)  | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"start\")"]` | 20.75 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"next\")"]` | 1.78 (25%) :x: | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"start\")"]` | 21.61 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"start\")"]` | 20.75 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"next\")"]` | 1.00 (25%)  | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Set\", \"String\", \"start\")"]` | 24.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"next\")"]` | 1.78 (25%) :x: | 3.50 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"start\")"]` | 9.00 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"start\")"]` | 7.83 (25%) :x: | Inf (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"next\")"]` | 1.00 (25%)  | 3.00 (1%) :x: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"start\")"]` | 7.83 (25%) :x: | Inf (1%) :x: |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 1.24 (25%)  | 1.86 (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 1.13 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"unspecified\")"]` | 1.00 (25%)  | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 6.97 (25%) :x: | 4.23 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 7.91 (25%) :x: | 3.22 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 4.14 (25%) :x: | 2001.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 3.54 (25%) :x: | 1793.00 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 0.91 (25%)  | 0.78 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 1.00 (25%)  | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 1.00 (25%)  | 1.55 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 1.15 (25%)  | 1.48 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.12 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.00 (25%)  | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.23 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.44 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.36 (25%) :x: | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.61 (25%) :x: | 1.14 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.00 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.00 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.10 (25%)  | 1.10 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 1.00 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.08 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.03 (25%)  | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.07 (25%)  | 1.01 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.02 (15%)  | 1.25 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 14.17 (15%) :x: | 11.88 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 6.78 (15%) :x: | 4.12 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 8.15 (15%) :x: | 3.59 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 8.23 (15%) :x: | 4.12 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.97 (15%)  | 1.22 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 4.80 (15%) :x: | 3.85 (1%) :x: |
| `["dates", "parse", "Date"]` | 5.97 (15%) :x: | 3.85 (1%) :x: |
| `["dates", "parse", "DateTime"]` | 28.15 (15%) :x: | 11.88 (1%) :x: |
| `["dates", "string", "Date"]` | 1.26 (15%) :x: | 2.17 (1%) :x: |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 2.06 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 2.70 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io", "read", "read"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 0.72 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 0.86 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 1.09 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.96 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg", "blas", "axpy!"]` | 2.11 (40%) :x: | 1.00 (1%)  |
| `["linalg", "blas", "scal!"]` | 3.10 (40%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eig\", \"LowerTriangular\", 1024)"]` | 1.90 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eig\", \"LowerTriangular\", 256)"]` | 3.26 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eig\", \"UpperTriangular\", 1024)"]` | 2.13 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eig\", \"UpperTriangular\", 256)"]` | 3.64 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eigfact\", \"LowerTriangular\", 1024)"]` | 1.96 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eigfact\", \"LowerTriangular\", 256)"]` | 3.30 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eigfact\", \"UpperTriangular\", 1024)"]` | 2.13 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"eigfact\", \"UpperTriangular\", 256)"]` | 3.63 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 1024)"]` | 4.89 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 256)"]` | 13.62 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 1024)"]` | 7.36 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 256)"]` | 24.57 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"qr\", \"Matrix\", 256)"]` | 2.33 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 15.20 (45%) :x: | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 14.05 (45%) :x: | 1.09 (1%) :x: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 1024)"]` | 15.20 (45%) :x: | 1.08 (1%) :x: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 256)"]` | 14.00 (45%) :x: | 1.09 (1%) :x: |
| `["micro", "mandel"]` | 5.63 (15%) :x: | 65.19 (1%) :x: |
| `["micro", "parseint"]` | 1.25 (15%) :x: | 1.13 (1%) :x: |
| `["micro", "randmatstat"]` | 2.12 (15%) :x: | 1.00 (1%)  |
| `["misc", "afoldl", "Complex{Float64}"]` | 1.05 (15%)  | 1.03 (1%) :x: |
| `["misc", "afoldl", "Float64"]` | 1.13 (15%)  | 1.03 (1%) :x: |
| `["misc", "afoldl", "Int"]` | 1.15 (15%)  | 1.03 (1%) :x: |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["misc", "parse", "DateTime"]` | 17.88 (15%) :x: | 10.34 (1%) :x: |
| `["misc", "parse", "Float64"]` | 0.98 (15%)  | 1.03 (1%) :x: |
| `["misc", "parse", "Int"]` | 26.12 (15%) :x: | 48.21 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.05 (15%)  | 1.04 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.00 (15%)  | 1.07 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.11 (15%)  | 1.02 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.02 (15%)  | 1.05 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.03 (15%)  | 1.07 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 2.30 (15%) :x: | 3.32 (1%) :x: |
| `["problem", "json", "parse_json"]` | 1.30 (15%) :x: | 1.18 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 12.62 (15%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 7.76 (15%) :x: | 9.71 (1%) :x: |
| `["problem", "simplex", "simplex"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 3.39 (15%) :x: | 2.14 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large BitSet\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Bool\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["scalar", "iteration", "in"]` | 11673.69 (25%) :x: | 1.00 (1%)  |
| `["scalar", "iteration", "indexed"]` | 46042.79 (25%) :x: | 1.00 (1%)  |
| `["shootout", "fasta"]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["shootout", "k_nucleotide"]` | 1.53 (15%) :x: | 1.42 (1%) :x: |
| `["shootout", "mandelbrot"]` | 1.01 (15%)  | 1.05 (1%) :x: |
| `["shootout", "meteor_contest"]` | 0.96 (15%)  | 1.01 (1%) :x: |
| `["shootout", "nbody"]` | 1.35 (15%) :x: | 358.50 (1%) :x: |
| `["shootout", "nbody_vec"]` | 1.20 (15%) :x: | 2.41 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ascending\")"]` | 2.42 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ones\")"]` | 2.16 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"descending\")"]` | 2.88 (30%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ones\")"]` | 2.00 (30%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"forwards\", \"ascending\")"]` | 2.26 (30%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 2.00 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ascending\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort", "mergesort", "(\"sortperm reverse\", \"descending\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 1.00 (15%)  | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 1.06 (15%)  | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 1.06 (15%)  | 1.06 (1%) :x: |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.20 (15%) :x: | 1.01 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 3.74 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 1000)"]` | 3.51 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 1.71 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 3.08 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"array\", 10000)"]` | 2.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"array\", 100000)"]` | 2.05 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x40, sparse 400x40 -> dense 400x400\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.83 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.05 (15%)  | 1.07 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 1.03 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 1.08 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 1.06 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 1.05 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 1.03 (15%)  | 1.03 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 0.89 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 0.99 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.01 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 1.07 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.03 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 0.97 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 1.06 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.08 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 3.06 (15%) :x: | 2.62 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 3.02 (15%) :x: | 2.63 (1%) :x: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 3.16 (15%) :x: | 2.64 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 3.11 (15%) :x: | 2.99 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 3.18 (15%) :x: | 2.97 (1%) :x: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 3.08 (15%) :x: | 2.99 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 4.65 (15%) :x: | 13.12 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 4.56 (15%) :x: | 11.65 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 4.38 (15%) :x: | 12.50 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 3.94 (15%) :x: | 2.80 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 3.90 (15%) :x: | 2.65 (1%) :x: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 3.79 (15%) :x: | 2.70 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 4.25 (15%) :x: | 4.28 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 3.92 (15%) :x: | 4.14 (1%) :x: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 4.15 (15%) :x: | 4.26 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 4.26 (15%) :x: | 3.72 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 4.03 (15%) :x: | 3.54 (1%) :x: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 4.07 (15%) :x: | 3.61 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 4.39 (15%) :x: | 3.72 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 4.11 (15%) :x: | 3.54 (1%) :x: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 4.01 (15%) :x: | 3.61 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 4.21 (15%) :x: | 13.12 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 4.17 (15%) :x: | 11.65 (1%) :x: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 4.49 (15%) :x: | 12.50 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 7.44 (15%) :x: | 1.91 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 6.94 (15%) :x: | 1.88 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 9.70 (15%) :x: | 3.75 (1%) :x: |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 7.83 (15%) :x: | 3.25 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 91.53 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 37.15 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 47.60 (15%) :x: | 23.49 (1%) :x: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 29.20 (15%) :x: | 10.86 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 84.72 (15%) :x: | 37.15 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 36.94 (15%) :x: | 16.12 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 83.13 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 35.36 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 89.50 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 36.32 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 95.63 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 38.46 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 65.16 (15%) :x: | 11.73 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 28.22 (15%) :x: | 6.17 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 58.99 (15%) :x: | 11.73 (1%) :x: |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 27.16 (15%) :x: | 6.17 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 93.73 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 37.82 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 40.79 (15%) :x: | 14.34 (1%) :x: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 27.80 (15%) :x: | 7.00 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 92.71 (15%) :x: | 37.15 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 36.18 (15%) :x: | 16.12 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 96.62 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 35.69 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 86.56 (15%) :x: | 19.57 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 35.64 (15%) :x: | 9.20 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 101.18 (15%) :x: | 79.14 (1%) :x: |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 38.04 (15%) :x: | 26.47 (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 100.43 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 91.69 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 90.51 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 98.99 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 89.07 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 79.48 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 89.45 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 80.87 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 97.41 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 78.44 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 95.50 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 82.39 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 79.15 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 73.25 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 92.19 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 76.63 (15%) :x: | Inf (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.23 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.4537
Commit 17f30e6 (2018-03-10 23:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110393602 s          0 s   17234905 s  5497528236 s        288 s
       #2  3501 MHz  449884649 s          0 s   18330634 s  5160362308 s         88 s
       #3  3501 MHz   87565466 s          0 s    9970983 s  5538534886 s        131 s
       #4  3501 MHz   82765308 s          0 s    9978592 s  5543721372 s         54 s
       
  Memory: 31.383651733398438 GB (5552.765625 MB free)
  Uptime: 5.6382786e7 sec
  Load Avg:  1.0068359375  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4535
Commit 40f64e5 (2018-03-10 22:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110511456 s          0 s   17245941 s  5498344485 s        288 s
       #2  3501 MHz  450745809 s          0 s   18340680 s  5160438288 s         89 s
       #3  3501 MHz   87654148 s          0 s    9979342 s  5539385714 s        131 s
       #4  3501 MHz   82851396 s          0 s    9986783 s  5544575145 s         54 s
       
  Memory: 31.383651733398438 GB (5092.61328125 MB free)
  Uptime: 5.6392273e7 sec
  Load Avg:  1.1630859375  1.0478515625  1.05615234375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
