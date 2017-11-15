# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d5c56f41fb257059ebe31cd139bb7b2f990aa42f](https://github.com/JuliaLang/julia/commit/d5c56f41fb257059ebe31cd139bb7b2f990aa42f) vs [JuliaLang/julia@9b1b1bd76c5363e91ea3ea9f8581230faa4d6747](https://github.com/JuliaLang/julia/commit/9b1b1bd76c5363e91ea3ea9f8581230faa4d6747)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24113#issuecomment-344381739)

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
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 7.04 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 12.21 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 6.90 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.30 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.98 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.77 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.18 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 4.00 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 7.01 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 12.90 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 6.65 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.36 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.83 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.07 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.10 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.09 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.67 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.11 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.95 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.09 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.10 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.12 (50%)  | Inf (1%) :x: |
| `["array", "reductions", "(\"var\", \"Float64\")"]` | 1.00 (15%)  | 0.80 (1%) :white_check_mark: |
| `["array", "reductions", "(\"var\", \"Int64\")"]` | 1.05 (15%)  | 0.82 (1%) :white_check_mark: |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.65 (15%) :x: | 1.02 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.68 (15%) :x: | 1.05 (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 0.99 (15%)  | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 0.96 (15%)  | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 0.96 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 1.00 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 1.00 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 0.96 (15%)  | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup\")"]` | 182.33 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 174.32 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 188.77 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 186.48 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup\")"]` | 189.49 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 189.49 (15%) :x: | Inf (1%) :x: |
| `["dates", "parse", "Date"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 1024)"]` | 82.53 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 163.78 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 1024)"]` | 82.29 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 151.02 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 107.81 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 160.72 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 83.35 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 141.10 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 3.07 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 256)"]` | 3.06 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 104.45 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 168.10 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 117.39 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 194.96 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 3.10 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 75.80 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 151.43 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 112.35 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 217.28 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 86.34 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 158.68 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 3.03 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 256)"]` | 3.13 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 119.26 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 166.95 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 122.37 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 195.60 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 3.09 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 86.30 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 157.85 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 1024)"]` | 34.90 (45%) :x: | 1.17 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 70.43 (45%) :x: | 1.66 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 1024)"]` | 52.87 (45%) :x: | 1.28 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 80.30 (45%) :x: | 2.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 1024)"]` | 49.65 (45%) :x: | 1.28 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 91.38 (45%) :x: | 2.06 (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 1024)"]` | 2.04 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 256)"]` | 1.50 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 1024)"]` | 2.14 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 256)"]` | 1.40 (45%)  | Inf (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 1.15 (45%)  | 1.01 (1%) :x: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 256)"]` | 1.16 (45%)  | 1.01 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 0.99 (15%)  | 0.97 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.02 (15%)  | 0.95 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.01 (15%)  | 1.09 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.01 (15%)  | 1.17 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.02 (15%)  | 1.04 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.01 (15%)  | 1.12 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.03 (15%)  | 1.16 (1%) :x: |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["problem", "json", "parse_json"]` | 1.01 (15%)  | 0.97 (1%) :white_check_mark: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.10 (15%)  | 8.44 (1%) :x: |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.01 (15%)  | 1.14 (1%) :x: |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 110.26 (15%) :x: | 32.72 (1%) :x: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 1.05 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"descending\")"]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ones\")"]` | 1.05 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"random\")"]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 0.88 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 1.02 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 1.00 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.06 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 1.00 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.03 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 0.99 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 1.03 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 1.01 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 0.99 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 1.07 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"ones\")"]` | 1.00 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 1.00 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"ascending\")"]` | 1.02 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"descending\")"]` | 1.03 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"ones\")"]` | 0.99 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"random\")"]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ascending\")"]` | 1.01 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"descending\")"]` | 1.00 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ones\")"]` | 1.00 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"random\")"]` | 1.00 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.01 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"descending\")"]` | 1.01 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.01 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"descending\")"]` | 1.01 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 1.00 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 0.99 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 1.00 (30%)  | 1.11 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 1.00 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 0.98 (30%)  | 1.01 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 1.00 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.00 (30%)  | 1.03 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 1.00 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 1.00 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 1.00 (30%)  | 1.05 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 1.32 (30%) :x: | 20.05 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 1.05 (30%)  | 16.24 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.08 (30%)  | 122.90 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.07 (30%)  | 16.24 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.04 (30%)  | 20.05 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x200, sparse 2000x200 -> dense 20x2000\")"]` | 1.05 (30%)  | 153.38 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 1.05 (30%)  | 1524.81 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 200x2000 -> dense 20x200\")"]` | 1.06 (30%)  | 153.38 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x20, dense 20x20 -> dense 2000x20\")"]` | 1.06 (30%)  | 20.05 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x200, dense 20x200 -> dense 2000x20\")"]` | 1.05 (30%)  | 153.38 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 1.05 (30%)  | 1524.81 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x20, dense 200x20 -> dense 200x200\")"]` | 1.05 (30%)  | 16.24 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.04 (30%)  | 122.90 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x2000, dense 20x2000 -> dense 200x20\")"]` | 1.05 (30%)  | 153.38 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.06 (30%)  | 20.05 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x200, dense 200x200 -> dense 20x200\")"]` | 1.04 (30%)  | 16.24 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.08 (30%)  | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 1.01 (30%)  | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.07 (30%)  | 1.13 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 1.09 (30%)  | 1.10 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 1.19 (30%)  | 1.04 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 1.11 (30%)  | 1.08 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.12 (30%)  | 1.79 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.06 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 1.13 (30%)  | 1.71 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.51 (30%) :x: | 1.04 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.12 (30%)  | 1.07 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.09 (30%)  | 3048.62 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 1.10 (30%)  | 305.76 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 1.09 (30%)  | 305.76 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.09 (30%)  | 244.81 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.10 (30%)  | 31.48 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.07 (30%)  | 39.10 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 1.08 (30%)  | 31.48 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.12 (30%)  | 39.10 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x200, dense 20x2000 -> dense 200x20\")"]` | 1.09 (30%)  | 305.76 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 1.10 (30%)  | 3048.62 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.07 (30%)  | 31.48 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 1.09 (30%)  | 244.81 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x2000, dense 20x200 -> dense 2000x20\")"]` | 1.10 (30%)  | 305.76 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.12 (30%)  | 39.10 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x200, dense 200x20 -> dense 200x200\")"]` | 1.10 (30%)  | 31.48 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.11 (30%)  | 39.10 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.12 (30%)  | 1.27 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.18 (30%)  | 1.19 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.03 (30%)  | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.16 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.01 (30%)  | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.07 (30%)  | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 1.17 (30%)  | 2.42 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 1.24 (30%)  | 2.58 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.38 (30%) :x: | 1.14 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 1.11 (30%)  | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 1.25 (30%)  | 1.16 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.63 (30%) :x: | 1.08 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 1.25 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.64 (30%) :x: | 1.08 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
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
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
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
- `["nullable", "basic"]`
- `["nullable", "nullablearray"]`
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
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "cos"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "tan"]`
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
- `["string", "search"]`
- `["string", "searchindex"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2509
Commit d5c56f4 (2017-11-14 20:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   93319955 s          0 s   14479734 s  4516228996 s        207 s
       #2  3501 MHz  372612713 s          0 s   15788469 s  4237750291 s         72 s
       #3  3501 MHz   76910294 s          0 s    8759070 s  4546792597 s         92 s
       #4  3501 MHz   72099132 s          0 s    8630163 s  4552150464 s         39 s
       
  Memory: 31.383651733398438 GB (11485.20703125 MB free)
  Uptime: 4.634372e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2507
Commit 9b1b1bd (2017-11-14 19:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   93426386 s          0 s   14489814 s  4516825438 s        207 s
       #2  3501 MHz  373255918 s          0 s   15798209 s  4237812412 s         72 s
       #3  3501 MHz   77000757 s          0 s    8766760 s  4547409457 s         93 s
       #4  3501 MHz   72181459 s          0 s    8638000 s  4552775508 s         39 s
       
  Memory: 31.383651733398438 GB (11014.94921875 MB free)
  Uptime: 4.6350879e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
