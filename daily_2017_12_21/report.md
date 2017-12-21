# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b57a59256fbe646e63153cb35fc09dd6bc3d9ae9](https://github.com/JuliaLang/julia/commit/b57a59256fbe646e63153cb35fc09dd6bc3d9ae9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b57a59256fbe646e63153cb35fc09dd6bc3d9ae9#commitcomment-26406409)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-12-21 vs 2017-12-19

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
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"iterator\")"]` | 0.80 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\")"]` | 0.85 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\", \"sizehint!\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"iterator\")"]` | 0.79 (25%)  | 1.29 (1%) :x: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\")"]` | 0.85 (25%)  | 1.29 (1%) :x: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\", \"sizehint!\")"]` | 0.89 (25%)  | 2.00 (1%) :x: |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"BitSet\", \"Int8\")"]` | 0.80 (25%)  | 0.91 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 0.70 (25%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"true\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"<\", \"BitSet\")"]` | 0.88 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"big\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\")"]` | 0.79 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.86 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.49 (25%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 0.94 (25%)  | 1.28 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.07 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 0.87 (25%)  | 0.65 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.03 (25%) :white_check_mark: | 1.40 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Vector\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"big\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"BitSet\")"]` | 0.82 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Set\")"]` | 0.80 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.75 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"big\")"]` | 50.79 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\")"]` | 6.93 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.88 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.61 (25%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 0.88 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.80 (25%)  | 0.37 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.82 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.11 (25%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Vector\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 50.62 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\")"]` | 0.78 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\")"]` | 0.84 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.59 (25%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\")"]` | 0.81 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.00 (25%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\")"]` | 0.72 (25%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.00 (25%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"BitSet\")"]` | 0.89 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"self\")"]` | 0.85 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.21 (25%) :white_check_mark: | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.25 (25%) :white_check_mark: | 1.04 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 0.15 (25%) :white_check_mark: | 1.01 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.17 (25%) :white_check_mark: | 1.04 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 0.05 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.16 (25%) :white_check_mark: | 2.76 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"BitSet\")"]` | 0.07 (25%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Set\")"]` | 0.06 (25%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.05 (25%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\")"]` | 254.79 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.54 (25%) :white_check_mark: | 0.52 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.53 (25%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 0.54 (25%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.55 (25%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.50 (25%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.53 (25%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 10.97 (25%) :x: | 4.79 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\")"]` | 26.17 (25%) :x: | 51.73 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 26.82 (25%) :x: | 51.79 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\")"]` | 12.78 (25%) :x: | 51.73 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 12.84 (25%) :x: | 51.79 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\")"]` | 5.51 (25%) :x: | 53.66 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 5.79 (25%) :x: | 55.62 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"BitSet\")"]` | 1.15 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 1.18 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 1.14 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 5170.57 (25%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.38 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.39 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 0.37 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.39 (25%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.29 (25%) :white_check_mark: | 0.11 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.29 (25%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 0.48 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\")"]` | 0.47 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.49 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 0.47 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.50 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 0.49 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.51 (25%) :white_check_mark: | 0.69 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"empty\", \"Int\", \"<\", \"BitSet\")"]` | 0.90 (25%)  | 0.91 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"empty\", \"Int\", \"⊆\", \"BitSet\")"]` | 0.90 (25%)  | 0.91 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 1024)"]` | 37.49 (45%) :x: | 13.67 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 256)"]` | 4.23 (45%) :x: | 3.45 (1%) :x: |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 0.54 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.54 (45%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small BitSet\")"]` | 0.05 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small BitSet\")"]` | 0.05 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small BitSet\")"]` | 0.00 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large BitSet\")"]` | 1.31 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small BitSet\")"]` | 1.16 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large BitSet\")"]` | 1.26 (25%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small BitSet\")"]` | 1.14 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large BitSet\")"]` | 1.21 (25%)  | Inf (1%) :x: |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small BitSet\")"]` | 1.03 (25%)  | Inf (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 1.93 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isequal\", \"Int64\")"]` | 1.57 (25%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["find"]`
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
- `["scalar", "cos"]`
- `["scalar", "cosh"]`
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
Julia Version 0.7.0-DEV.3138
Commit b57a592 (2017-12-21 03:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109671726 s          0 s   19296955 s  4805194174 s        100 s
       #2  3501 MHz  462890771 s          0 s   12272302 s  4470568536 s         23 s
       #3  3501 MHz   91736681 s          0 s   10479249 s  4844005257 s         84 s
       #4  3501 MHz   87764320 s          0 s   10670552 s  4847778951 s         21 s
       
  Memory: 31.383651733398438 GB (2185.71875 MB free)
  Uptime: 4.9485829e7 sec
  Load Avg:  1.0830078125  1.03125  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
