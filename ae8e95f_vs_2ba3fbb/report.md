# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ae8e95f249732ce4555584e8d0d8e469c4119edb](https://github.com/JuliaLang/julia/commit/ae8e95f249732ce4555584e8d0d8e469c4119edb) vs [JuliaLang/julia@2ba3fbbd4ffb03eda89c942ce9bc422e265e3c86](https://github.com/JuliaLang/julia/commit/2ba3fbbd4ffb03eda89c942ce9bc422e265e3c86)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ae8e95f249732ce4555584e8d0d8e469c4119edb#commitcomment-29626671)

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
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 1.07 (15%)  | 3.33 (1%) :x: |
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1} generator\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int16,1}\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int64,1} generator\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Int64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Vector{Bool}\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1} generator\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int16,1}\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int64,1} generator\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Int64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Vector{Bool}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat\", 5)"]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 0.13 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float32,1}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"Array{Float32,2}\")"]` | 4.70 (50%) :x: | 1.81 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"Array{Int32,2}\")"]` | 5.13 (50%) :x: | 1.82 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.28 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.30 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 4.94 (50%) :x: | 1.81 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 4.72 (50%) :x: | 1.82 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 4.91 (50%) :x: | 1.81 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 4.65 (50%) :x: | 1.82 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 1.63 (50%) :x: | 1.33 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.28 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.84 (50%) :x: | 1.81 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.30 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 20.80 (50%) :x: | 16.35 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 38.78 (50%) :x: | 31.70 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 4.92 (50%) :x: | 1.81 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 4.32 (50%) :x: | 1.81 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.29 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 5.00 (50%) :x: | 1.82 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.28 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 20.53 (50%) :x: | 18.35 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 40.85 (50%) :x: | 40.67 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 5.10 (50%) :x: | 1.82 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 4.47 (50%) :x: | 1.82 (1%) :x: |
| `["array", "index", "(\"sumelt\", \"Array{Int32,2}\")"]` | 0.17 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norm1\", \"Int64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Int64\")"]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Float64\")"]` | 51.81 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 74.82 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Float64\")"]` | 52.05 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 74.48 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"LinearAlgebra.norm\", \"Int64\")"]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"maxabs\", \"Float64\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 1.07 (15%)  | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 1.02 (15%)  | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 1.01 (15%)  | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.98 (15%)  | 0.95 (1%) :white_check_mark: |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 1.01 (15%)  | 0.95 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"BitSet\", \"Int\", \"pop!\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter\")"]` | 0.92 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 42.83 (25%) :x: | 1.21 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"filter!\")"]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"filter\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"pop!\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"IdDict\", \"Int\", \"filter!\")"]` | 0.74 (25%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 0.82 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 46.00 (25%) :x: | 1.16 (1%) :x: |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter!\")"]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"pop!\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter!\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"iterator\")"]` | 0.92 (25%)  | 0.78 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\")"]` | 0.98 (25%)  | 0.78 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 1.01 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.95 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"iterator\")"]` | 0.70 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\")"]` | 0.70 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.66 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"iterator\")"]` | 1.04 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\")"]` | 1.05 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\", \"sizehint!\")"]` | 1.10 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"iterator\")"]` | 0.75 (25%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\")"]` | 0.74 (25%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.71 (25%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 0.95 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 1.01 (25%)  | 0.99 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"iterator\")"]` | 0.73 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\")"]` | 0.76 (25%)  | 0.27 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.75 (25%)  | 0.21 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 0.66 (25%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"next\")"]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"start\")"]` | 0.97 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"start\")"]` | 0.97 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"start\")"]` | 0.96 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"start\")"]` | 0.95 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"Int\", \"next\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"IdDict\", \"Int\", \"start\")"]` | 0.95 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"start\")"]` | 0.97 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"start\")"]` | 0.97 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"start\")"]` | 0.97 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"String\", \"start\")"]` | 0.95 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"start\")"]` | 0.93 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"start\")"]` | 0.93 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"start\")"]` | 0.92 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 0.94 (25%)  | 0.77 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"in\", \"false\")"]` | 3.60 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 33.83 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"new\")"]` | 2.86 (25%) :x: | 2.50 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"new\")"]` | 2.79 (25%) :x: | 2.50 (1%) :x: |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"in\", \"false\")"]` | 2.07 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"false\")"]` | 4.18 (25%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 32.97 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"new\")"]` | 3.57 (25%) :x: | 4.00 (1%) :x: |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"first\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"in\", \"false\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"false\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 1.45 (25%) :x: | 1.93 (1%) :x: |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"in\", \"false\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"in\", \"true\")"]` | 6.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 0.96 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 0.34 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 1.13 (25%)  | 1.44 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 1.04 (25%)  | 1.41 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 1.12 (25%)  | 1.32 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 1.11 (25%)  | 1.29 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.94 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 3.69 (25%) :x: | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.75 (25%) :x: | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.96 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.97 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.97 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.92 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\")"]` | 0.24 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"BitSet\")"]` | 0.34 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Set\")"]` | 0.33 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.33 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\")"]` | 0.26 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.59 (25%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.62 (25%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 0.58 (25%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.59 (25%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.57 (25%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.61 (25%) :white_check_mark: | 0.27 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\")"]` | 0.26 (25%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\")"]` | 0.50 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.51 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\")"]` | 0.50 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.50 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\")"]` | 0.50 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.50 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"BitSet\")"]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Set\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 0.78 (25%)  | 0.45 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\")"]` | 1.01 (25%)  | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.99 (25%)  | 0.22 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\")"]` | 1.00 (25%)  | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.96 (25%)  | 0.22 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\")"]` | 0.98 (25%)  | 0.25 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.95 (25%)  | 0.29 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"BitSet\")"]` | 0.96 (25%)  | 0.42 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 0.96 (25%)  | 0.42 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.98 (25%)  | 0.42 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 0.77 (25%)  | 0.45 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\")"]` | 0.79 (25%)  | 0.45 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.79 (25%)  | 0.45 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 0.78 (25%)  | 0.45 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.78 (25%)  | 0.45 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 0.78 (25%)  | 0.45 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.79 (25%)  | 0.45 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 0.92 (15%)  | 0.98 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 0.14 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.23 (15%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 0.15 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.94 (15%)  | 0.98 (1%) :white_check_mark: |
| `["dates", "string", "Date"]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "string", "DateTime"]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "parse", "Float64"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 0.56 (15%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["problem", "json", "parse_json"]` | 0.73 (15%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["problem", "laplacian", "laplace_iter_devec"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 2.04 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 0.46 (15%) :white_check_mark: | 0.64 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large BitSet\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 0.47 (25%) :white_check_mark: | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large String\")"]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Vector\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small BitSet\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 0.46 (25%) :white_check_mark: | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small String\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Vector\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large BitSet\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 0.54 (25%) :white_check_mark: | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large String\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Vector\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small BitSet\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 0.46 (25%) :white_check_mark: | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small String\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Vector\")"]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 0.96 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 0.95 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large BitSet\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 0.50 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 0.52 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large String\")"]` | 0.58 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small BitSet\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.49 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 0.42 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small String\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large BitSet\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 0.51 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 0.43 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small BitSet\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 0.40 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 0.52 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small String\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 0.76 (25%)  | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 0.67 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 0.72 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 0.65 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", 100)"]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 0.78 (25%)  | 0.96 (1%) :white_check_mark: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 0.74 (25%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\", 100)"]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551615\")"]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551616\")"]` | 0.35 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:1\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967295\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967297\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:170141183460469231731687303715884105728\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551615\")"]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551616\")"]` | 0.40 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:18446744073709551615\")"]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:1\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967295\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967297\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 0.38 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 0.38 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Bool\", \"RangeGenerator(true:true)\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:1)\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.49 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.45 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967295)\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967297)\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:1)\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:4294967297)\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:1)\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 0.45 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967295)\")"]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967297)\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967295)\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967297)\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float16\")"]` | 2.07 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float16\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float32\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float64\")"]` | 1.49 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"RandomDevice\", \"Float64\")"]` | 1.45 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 1.44 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float32\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float64\")"]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"RandomDevice\", \"Float64\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigFloat\")"]` | 0.70 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Int64\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"UInt64\")"]` | 0.90 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float32\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float64\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.80 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.71 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.81 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.82 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.82 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.47 (50%) :white_check_mark: | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 0.65 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigInt\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 0.67 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigInt\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.80 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{Int64}\")"]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.84 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.84 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigFloat\")"]` | 0.90 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.57 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.59 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Int64\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"UInt64\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigFloat\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigInt\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 0.68 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 0.74 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float32\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float64\")"]` | 0.78 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"UInt64\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.61 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.55 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.73 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 0.72 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.61 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.61 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 0.79 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 0.75 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 0.61 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 0.59 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.83 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.80 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 0.70 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.82 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 0.76 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 0.80 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 0.72 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 0.81 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 0.86 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigInt\")"]` | 0.77 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 0.89 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigInt\")"]` | 0.80 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 0.66 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigFloat\")"]` | 0.91 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigInt\")"]` | 0.79 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigFloat\")"]` | 0.91 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigInt\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigFloat\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 0.91 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.56 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 1.01 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 0.78 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Int64\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"UInt64\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 0.74 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.78 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float32\")"]` | 0.64 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float64\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.57 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.80 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 2.19 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.58 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.61 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 2.35 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 0.65 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 0.60 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.59 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.77 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.59 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 2.38 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.60 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.56 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.41 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 0.91 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 0.64 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.79 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 0.79 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigInt\")"]` | 0.67 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.80 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 0.63 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigFloat\")"]` | 0.49 (50%) :white_check_mark: | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.61 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Bool\")"]` | 0.20 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Int64\")"]` | 0.13 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"UInt64\")"]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Bool\")"]` | 0.11 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Int64\")"]` | 0.19 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"UInt64\")"]` | 0.14 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Bool\")"]` | 0.10 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Int64\")"]` | 0.19 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"UInt64\")"]` | 0.15 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigFloat\")"]` | 0.73 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 0.63 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 0.66 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 0.68 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 0.62 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 0.62 (50%)  | 1.24 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Int64\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"UInt64\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 0.66 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 0.71 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float32\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float64\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 0.76 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 0.77 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 0.64 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 0.68 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 0.85 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 0.83 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 0.73 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 0.72 (50%)  | 1.20 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 0.64 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 0.63 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 0.75 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 0.64 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 0.76 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 0.61 (50%)  | 1.26 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 0.70 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 0.66 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 0.69 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigInt\")"]` | 0.68 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 0.73 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigInt\")"]` | 0.69 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 0.72 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 0.62 (50%)  | 1.25 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigFloat\")"]` | 0.71 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 0.65 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigFloat\")"]` | 0.72 (50%)  | 1.27 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 0.67 (50%)  | 1.23 (1%) :x: |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Float64\")"]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigFloat\")"]` | 0.71 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 0.69 (40%)  | 1.23 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigFloat\")"]` | 0.91 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"BigInt\")"]` | 0.77 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 0.63 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 0.75 (40%)  | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"BigFloat\")"]` | 0.65 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 0.58 (40%) :white_check_mark: | 1.26 (1%) :x: |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 2.17 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigFloat\")"]` | 0.73 (40%)  | 1.27 (1%) :x: |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 0.61 (40%)  | 1.23 (1%) :x: |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float64\")"]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp\", \"no agument reduction, k = 9\", \"Float64\")"]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"+\")"]` | 1.49 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"-\")"]` | 1.53 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"+\")"]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"-\")"]` | 1.63 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isodd\", \"Int64\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"negative argument\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"positive argument\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2f0^-12\", \"negative argument\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2f0^-12\", \"positive argument\", \"Float32\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"1f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"1f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2f0^-12 <= abs(x) < 1f0\", \"negative argument\", \"Float32\")"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float32\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "k_nucleotide"]` | 0.53 (15%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4095)"]` | 7.93 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4096)"]` | 8.46 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4095)"]` | 3.28 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4096)"]` | 3.34 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4095)"]` | 6.96 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4096)"]` | 7.19 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4095)"]` | 1.66 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4096)"]` | 1.55 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 1.71 (20%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 0.30 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 0.31 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 1.51 (15%) :x: | 2.29 (1%) :x: |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 0.98 (15%)  | 0.94 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 0.95 (15%)  | 0.94 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 0.60 (30%) :white_check_mark: | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 0.79 (30%)  | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"array\", 1000)"]` | 0.86 (30%)  | 1.02 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 0.64 (30%) :white_check_mark: | 1.05 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 0.75 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 1000)"]` | 0.83 (30%)  | 1.01 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 1.02 (30%)  | 1.60 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 0.83 (30%)  | 1.02 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.00 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.00 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 0.98 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 0.99 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 1.00 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.00 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 0.97 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 1.00 (30%)  | 0.50 (1%) :white_check_mark: |
| `["tuple", "linear algebra", "(\"matvec\", (4, 4), (4,))"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 0.07 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 0.08 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 0.09 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 0.07 (15%) :white_check_mark: | 0.24 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 0.09 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 0.10 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 0.08 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 0.10 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 0.10 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 0.08 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 0.09 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 0.09 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 0.08 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 0.07 (15%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 0.10 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 0.08 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 0.10 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 0.08 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 0.10 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 0.07 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 0.07 (15%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 0.10 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 0.08 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 0.10 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 0.08 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 0.10 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 0.02 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 0.02 (15%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 0.02 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 0.03 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 0.03 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 0.03 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 0.00 (15%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 0.06 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 0.03 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 0.07 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 0.06 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 0.06 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 0.06 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 0.03 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.07 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.03 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 0.07 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 0.07 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 0.08 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (true, true))"]` | 0.09 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, true))"]` | 0.03 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 0.03 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 0.03 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 0.03 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, true))"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, false))"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 0.03 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_countequals\", \"BigFloat\")"]` | 0.10 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 0.04 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 0.04 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 0.06 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 0.05 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.03 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int64, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 0.03 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 0.03 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 0.07 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", BigInt, true)"]` | 0.12 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum2\", Bool, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", BigFloat, true)"]` | 0.07 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", BigInt, true)"]` | 0.12 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 0.04 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 0.05 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, true)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", BigInt, true)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum4\", Bool, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Bool, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float32, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float32, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float64, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Float64, true)"]` | 0.00 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int64, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int64, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 0.00 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 0.00 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 0.07 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 0.12 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int64, false)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int64, true)"]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 0.00 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 0.00 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, BigFloat, false)"]` | 0.10 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, BigFloat, true)"]` | 0.09 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, BigInt, false)"]` | 0.10 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, BigInt, true)"]` | 0.09 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Bool, false)"]` | 0.10 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Bool, true)"]` | 0.06 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 0.09 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, true)"]` | 0.07 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Float32, false)"]` | 0.10 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Float32, true)"]` | 0.07 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Float64, false)"]` | 0.10 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Float64, true)"]` | 0.07 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Int64, false)"]` | 0.10 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Int64, true)"]` | 0.07 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Int8, false)"]` | 0.10 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", collect, Int8, true)"]` | 0.06 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 0.06 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, true)"]` | 0.07 (15%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 0.10 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, BigInt, true)"]` | 0.12 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Bool, false)"]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 0.03 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 0.10 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, true)"]` | 0.03 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 0.10 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 0.02 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 0.10 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 0.03 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 0.03 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 0.02 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int8, true)"]` | 0.03 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", BigFloat, false)"]` | 0.08 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", BigFloat, true)"]` | 0.06 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", BigInt, false)"]` | 0.07 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", BigInt, true)"]` | 0.04 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Bool, false)"]` | 0.04 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Bool, true)"]` | 0.02 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float32, false)"]` | 0.03 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float32, true)"]` | 0.03 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float64, false)"]` | 0.04 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float64, true)"]` | 0.03 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int64, false)"]` | 0.03 (15%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int64, true)"]` | 0.02 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int8, false)"]` | 0.04 (15%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int8, true)"]` | 0.02 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |

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
Julia Version 0.7.0-beta.187
Commit ae8e95f (2018-07-06 16:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   23096403 s        259 s    3252090 s  846479317 s          6 s
       #2  3501 MHz  113763937 s          0 s    1806288 s  758947228 s          6 s
       #3  3501 MHz   17185570 s       2392 s    1882100 s  855619104 s         13 s
       #4  3501 MHz   16486211 s          4 s    1481612 s  857129850 s          7 s
       
  Memory: 31.383651733398438 GB (4882.77734375 MB free)
  Uptime: 8.754895e6 sec
  Load Avg:  1.03271484375  1.02587890625  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.65
Commit 2ba3fbb (2018-06-10 21:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   23215936 s        259 s    3264278 s  847412443 s          6 s
       #2  3501 MHz  114748981 s          0 s    1817081 s  759019072 s          6 s
       #3  3501 MHz   17314172 s       2392 s    1891068 s  856549253 s         13 s
       #4  3501 MHz   16602930 s          4 s    1490578 s  858072202 s          7 s
       
  Memory: 31.383651733398438 GB (4954.296875 MB free)
  Uptime: 8.765583e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
