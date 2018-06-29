# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ba31a93ff1071c8448aed391131f27ad2eb1a61d](https://github.com/JuliaLang/julia/commit/ba31a93ff1071c8448aed391131f27ad2eb1a61d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ba31a93ff1071c8448aed391131f27ad2eb1a61d#commitcomment-29539219)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-06-29 vs 2018-06-28

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"hcat\", 5)"]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"Array{Float32,2}\")"]` | 5.85 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"Array{Int32,2}\")"]` | 6.07 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.44 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.48 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 6.16 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 6.31 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 6.51 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 6.29 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 1.91 (50%) :x: | 1.34 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.52 (50%) :x: | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 5.92 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.49 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 35.84 (50%) :x: | 20.04 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 149.65 (50%) :x: | 48.61 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.40 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 5.58 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.45 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 6.09 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.47 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 36.87 (50%) :x: | 21.43 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 154.35 (50%) :x: | 58.20 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.34 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 5.20 (50%) :x: | 1.85 (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Float64\")"]` | 71.30 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 575.32 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Float64\")"]` | 71.17 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 569.19 (15%) :x: | Inf (1%) :x: |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 26.91 (25%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 26.96 (25%) :x: | 1.00 (1%)  |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"iterator\")"]` | 1.02 (25%)  | 1.04 (1%) :x: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"iterator\")"]` | 1.08 (25%)  | 1.03 (1%) :x: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"next\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"BitSet\", \"Int8\")"]` | 1.00 (25%)  | 1.10 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 18.77 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 22.00 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\")"]` | 1.05 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Set\")"]` | 0.99 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Vector\")"]` | 0.96 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Set\")"]` | 1.01 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Vector\")"]` | 1.01 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"Set\")"]` | 1.02 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"Vector\")"]` | 1.05 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\")"]` | 1.06 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.91 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.01 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.01 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.02 (25%)  | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.03 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.08 (25%)  | 1.17 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Set\")"]` | 1.00 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Vector\")"]` | 1.11 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\")"]` | 1.03 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.03 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\")"]` | 1.01 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.02 (25%)  | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\")"]` | 1.05 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.09 (25%)  | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 1.03 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Set\")"]` | 1.00 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Vector\")"]` | 1.01 (25%)  | Inf (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 2.43 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.44 (45%) :x: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.62 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"zero\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 1.91 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 1.92 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4095)"]` | 0.70 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 0.58 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4096)"]` | 0.60 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "arithmetic", "(\"unary minus\", (20000, 20000))"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 1000)"]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.49 (40%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int8, true)"]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigFloat, true)"]` | 0.98 (15%)  | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", BigInt, true)"]` | 0.88 (15%)  | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Bool, true)"]` | 0.67 (15%) :white_check_mark: | 0.65 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float32, true)"]` | 0.87 (15%)  | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Float64, true)"]` | 0.82 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int64, true)"]` | 0.69 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["union", "array", "(\"sort\", Int8, true)"]` | 0.67 (15%) :white_check_mark: | 0.65 (1%) :white_check_mark: |

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
Julia Version 0.7.0-beta.83
Commit ba31a93 (2018-06-29 01:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   36670556 s        278 s    3828635 s  765559713 s          7 s
       #2  3501 MHz  168056590 s          0 s    2348050 s  637691002 s          4 s
       #3  3501 MHz   23025810 s       2377 s    1903642 s  782830121 s         12 s
       #4  3501 MHz   21525343 s          0 s    2189954 s  784190231 s          8 s
       
  Memory: 31.383651733398438 GB (4867.59375 MB free)
  Uptime: 8.085848e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
