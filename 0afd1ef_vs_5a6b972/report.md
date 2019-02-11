# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0afd1ef1473f3503b15e17fbc40323fe840961c4](https://github.com/JuliaLang/julia/commit/0afd1ef1473f3503b15e17fbc40323fe840961c4) vs [JuliaLang/julia@5a6b972282a91ceea422c479433e7d1413fea2b4](https://github.com/JuliaLang/julia/commit/5a6b972282a91ceea422c479433e7d1413fea2b4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/31011#issuecomment-462180912)

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
| `["array", "accumulate", "(\"accumulate!\", \"Float64\")"]` | 1.34 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 1.70 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"accumulate\", \"Float64\")"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"accumulate\", \"Int\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 1.71 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Float64\")"]` | 1.21 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.96 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.98 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1} generator\")"]` | 1.61 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int64,1} generator\")"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 2.10 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 2.03 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1} generator\")"]` | 1.66 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int64,1} generator\")"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"BitArray\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 5)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 500)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Float64,1}\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int16,1}\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 2048)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 256)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"BitArray{2}\")"]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.39 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 5.25 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumelt\", \"Array{Int32,2}\")"]` | 4.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 5.26 (50%) :x: | 1.40 (1%) :x: |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 2.22 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 2.20 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.22 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.05 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.27 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.28 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.26 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.30 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.53 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"perf_reduce\", \"Int64\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "reverse", "rev_load_slow!"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"false\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"big\")"]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.03 (25%)  | 1.06 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.02 (25%)  | 1.06 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.93 (25%)  | 1.06 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.98 (25%)  | 1.06 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Vector\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 0.91 (5%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.80 (5%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.96 (5%)  | 0.92 (1%) :white_check_mark: |
| `["dates", "string", "Date"]` | 0.55 (5%) :white_check_mark: | 0.65 (1%) :white_check_mark: |
| `["dates", "string", "DateTime"]` | 0.41 (5%) :white_check_mark: | 0.53 (1%) :white_check_mark: |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["io", "array_limit", "(\"display\", \"Array{Float64,1}(100000000,)\")"]` | 0.74 (5%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(10000, 10000)\")"]` | 0.69 (5%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["io", "array_limit", "(\"display\", \"Array{Float64,2}(100000000, 1)\")"]` | 0.74 (5%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["io", "skipchars"]` | 1.09 (5%) :x: | 0.94 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 1024)"]` | 1.50 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 256)"]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 1024)"]` | 1.69 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 256)"]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.39 (45%) :x: | 1.00 (1%)  |
| `["linalg", "small exp #29116"]` | 1.25 (5%) :x: | 1.02 (1%) :x: |
| `["micro", "fib"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["micro", "printfd"]` | 0.99 (5%)  | 0.84 (1%) :white_check_mark: |
| `["misc", "18129"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["misc", "23042", "Float64"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "afoldl", "Int"]` | 0.56 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "conditional"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "no conditional"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "fastmath many args"]` | 0.74 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1, 1:1)"]` | 4.99 (5%) :x: | 1.71 (1%) :x: |
| `["misc", "iterators", "zip(1:1000)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.00 (5%)  | 0.99 (1%) :white_check_mark: |
| `["misc", "repeat", "(200, 24, 1)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 0.97 (5%)  | 0.98 (1%) :white_check_mark: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int32\", \"RangeGenerator(1:1)\")"]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.47 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"BigInt\")"]` | 1.59 (40%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float32\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 0.83 (5%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "mandelbrot"]` | 1.01 (5%)  | 0.96 (1%) :white_check_mark: |
| `["shootout", "pidigits"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int32\", 4095)"]` | 1.44 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions\", \"Int32\", 4096)"]` | 1.44 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int32\", 4095)"]` | 1.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"two_reductions_aliased\", \"Int32\", 4096)"]` | 1.47 (20%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string", "readuntil", "no backtracking"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 1.65 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (2, 2))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (2,))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4,))"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 0.79 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 2.57 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 2.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 2.55 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 2.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 2.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 2.59 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 2.58 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 2.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 2.55 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 2.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 2.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 2.58 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 1.52 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 1.49 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, false)"]` | 1.44 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.54 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, false)"]` | 1.67 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 1.73 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, false)"]` | 1.67 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.79 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 1.66 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, true)"]` | 1.53 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 2.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 1.60 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 1.33 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Float32, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Int64, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, Float32}, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, Int64}, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Missing, Int8}, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, BigInt}, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Float32}, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Float64}, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, Int8}, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Bool}, false)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Int8}, false)"]` | 1.16 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.2.0-DEV.307
Commit 0afd1ef (2019-02-10 22:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   44539122 s       2428 s    8796257 s  2706065884 s         12 s
       #2  3501 MHz  252494869 s         14 s    4512539 s  2508862738 s         18 s
       #3  3501 MHz   35553484 s       3148 s    4152208 s  2725958606 s         27 s
       #4  3501 MHz   34257296 s         14 s    3203622 s  2729427852 s         23 s
       
  Memory: 31.383651733398438 GB (3044.24609375 MB free)
  Uptime: 2.7680021e7 sec
  Load Avg:  0.9228515625  1.0  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.2.0-DEV.298
Commit 5a6b972 (2019-02-09 17:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   44657326 s       2428 s    8807164 s  2707145534 s         12 s
       #2  3501 MHz  253618072 s         14 s    4528857 s  2508935794 s         18 s
       #3  3501 MHz   35670615 s       3148 s    4159493 s  2727046612 s         27 s
       #4  3501 MHz   34386319 s         14 s    3210662 s  2730504497 s         23 s
       
  Memory: 31.383651733398438 GB (4241.21875 MB free)
  Uptime: 2.7692154e7 sec
  Load Avg:  1.01806640625  1.0224609375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
