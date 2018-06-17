# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5e3259e98ecc60e169e0cc3025afb3001a3c3786](https://github.com/JuliaLang/julia/commit/5e3259e98ecc60e169e0cc3025afb3001a3c3786)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/5e3259e98ecc60e169e0cc3025afb3001a3c3786#commitcomment-29390818)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-06-17 vs 2018-06-16

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
| `["array", "cat", "(\"catnd\", 5)"]` | 1.02 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.93 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_indexing\", \"Array{Float64,1}\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter!\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"last\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"length\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"getindex\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"in\", \"false\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"unspecified\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"false\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"true\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"Vector\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 2.44 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.43 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 1024)"]` | 0.94 (45%)  | 0.98 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 256)"]` | 0.93 (45%)  | 0.95 (1%) :white_check_mark: |
| `["micro", "parseint"]` | 0.94 (15%)  | 0.99 (1%) :white_check_mark: |
| `["misc", "afoldl", "Complex{Float64}"]` | 0.89 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "afoldl", "Float64"]` | 0.92 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "afoldl", "Int"]` | 0.92 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["misc", "parse", "DateTime"]` | 0.94 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "parse", "Float64"]` | 0.95 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "parse", "Int"]` | 0.95 (15%)  | 0.98 (1%) :white_check_mark: |
| `["problem", "fem", "sparse_fem"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"'a':'z'\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"Float64\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Int64\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.85 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.96 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.96 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.97 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.91 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.95 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.94 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.92 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.93 (15%)  | 0.91 (1%) :white_check_mark: |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "arithmetic", "(\"unary minus\", (20000, 20000))"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 0.91 (15%)  | 0.91 (1%) :white_check_mark: |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 3, Float32)"]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.20 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-alpha.147
Commit 5e3259e (2018-06-16 18:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   29540841 s        276 s    3178894 s  670085576 s          6 s
       #2  3501 MHz  128260175 s          0 s    1785764 s  574620133 s          3 s
       #3  3501 MHz   16863724 s       2373 s    1436351 s  686036412 s          9 s
       #4  3501 MHz   15846452 s          0 s    1684914 s  686952818 s          6 s
       
  Memory: 31.383651733398438 GB (4841.09375 MB free)
  Uptime: 7.050475e6 sec
  Load Avg:  0.97412109375  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
