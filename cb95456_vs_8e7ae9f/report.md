# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@cb95456acfd6ee137e798fdb12dbd680786ad9e4](https://github.com/JuliaLang/julia/commit/cb95456acfd6ee137e798fdb12dbd680786ad9e4) vs [JuliaLang/julia@8e7ae9f96fa2eee7316a7a4a205cede4d22ae917](https://github.com/JuliaLang/julia/commit/8e7ae9f96fa2eee7316a7a4a205cede4d22ae917)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25377#issuecomment-356342023)

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
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.16 (15%) :x: | 1.01 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 691.70 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 192.22 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 179.22 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 1.00 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.64 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 0.96 (15%)  | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 0.99 (15%)  | Inf (1%) :x: |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.15 (15%)  | 1.02 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 2.43 (15%) :x: | 2.80 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 1.57 (15%) :x: | 2.57 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 1.86 (15%) :x: | 2.63 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 2.58 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.72 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 2.00 (15%) :x: | Inf (1%) :x: |
| `["dates", "arithmetic", "(\"DateTime\", \"Hour\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["find", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.04 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.08 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 1024)"]` | 1.04 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 1.08 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.03 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 1.14 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.08 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.09 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 1.05 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 1.08 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.00 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 1.04 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.33 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.08 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 1.24 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.17 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.21 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 1.14 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 1.06 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.04 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 1.25 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.03 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.12 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 1024)"]` | 1.03 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.24 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 1024)"]` | 1.03 (45%)  | 1.01 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 1.12 (45%)  | 1.05 (1%) :x: |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.43 (45%) :x: | 1.00 (1%)  |
| `["micro", "randmatstat"]` | 0.97 (15%)  | 1.11 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 43.70 (15%) :x: | 11730.87 (1%) :x: |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.18 (15%) :x: | 1.22 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Vector\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small BitSet\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small String\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Vector\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 4.89 (15%) :x: | 32.01 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 1.14 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 52.73 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x400, dense 40x400 -> dense 4000x40\")"]` | 155.68 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 189.52 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x40, dense 400x40 -> dense 400x400\")"]` | 17.89 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 20.53 (30%) :x: | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x4000, dense 40x4000 -> dense 400x40\")"]` | 20.05 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 2.51 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 2.26 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 5.52 (30%) :x: | 4.97 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 4.94 (30%) :x: | 6.64 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 6.15 (30%) :x: | 6.34 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.44 (30%) :x: | 1.54 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 15.87 (30%) :x: | 7.47 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 18.06 (30%) :x: | 7.22 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 39.59 (30%) :x: | 7.32 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 4.09 (30%) :x: | 2.42 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 1.80 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 5.78 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 33.24 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 1.49 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 2.88 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 4.13 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 0.95 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 0.01 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x2000, dense 2000x20 -> dense 2000x20\")"]` | 0.00 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 0.13 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 0.02 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 0.01 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 0.16 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x200, dense 20x200 -> dense 200x200\")"]` | 0.06 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 0.05 (30%) :white_check_mark: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 0.08 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 0.02 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.14 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 0.11 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 0.52 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 4.52 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 4.55 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 4.73 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 5.24 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 5.47 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 6.95 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 8.56 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 5.83 (30%) :x: | 0.97 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 3.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 8.02 (30%) :x: | 2.40 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 58.49 (30%) :x: | 7.31 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 16.19 (30%) :x: | 7.21 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 2.07 (30%) :x: | 2.16 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 12.72 (30%) :x: | 3.33 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 11.77 (30%) :x: | 7.46 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 7.73 (30%) :x: | 3.48 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 6.59 (30%) :x: | 4.96 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x400, dense 40x4000 -> dense 400x40\")"]` | 22.69 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 192.83 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 2.80 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 20.81 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x4000, dense 40x400 -> dense 4000x40\")"]` | 145.30 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 2.55 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x400, dense 400x40 -> dense 400x400\")"]` | 17.08 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 47.83 (30%) :x: | 1.03 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 37.39 (30%) :x: | 7.32 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 3.76 (30%) :x: | 2.42 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 17.21 (30%) :x: | 7.22 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 6.16 (30%) :x: | 6.35 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.39 (30%) :x: | 1.54 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 15.67 (30%) :x: | 7.47 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 5.24 (30%) :x: | 6.64 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 5.43 (30%) :x: | 4.97 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 5.74 (30%) :x: | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 33.28 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.05 (30%)  | 1.02 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 2.88 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 4.85 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 1.51 (30%) :x: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.57 (30%) :x: | 1.01 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"adjoint\", (20000, 10000))"]` | 133646.88 (30%) :x: | 3008558.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint\", (20000, 20000))"]` | 314312.25 (30%) :x: | 6009086.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint\", (600, 400))"]` | 35.06 (30%) :x: | 3877.00 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint\", (600, 600))"]` | 53.95 (30%) :x: | 5653.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "transpose", "(\"transpose\", (20000, 10000))"]` | 115699.53 (30%) :x: | 2009050.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 290091.92 (30%) :x: | 4009402.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose\", (600, 400))"]` | 27.76 (30%) :x: | 2697.00 (1%) :x: |
| `["sparse", "transpose", "(\"transpose\", (600, 600))"]` | 50.66 (30%) :x: | 3881.00 (1%) :x: |
| `["string", "join"]` | 1.80 (40%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3345
Commit cb95456 (2018-01-08 20:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101625100 s          0 s   15777105 s  4988374267 s        247 s
       #2  3501 MHz  402040730 s          0 s   17149544 s  4689027181 s         82 s
       #3  3501 MHz   82270370 s          0 s    9321420 s  5023633047 s        110 s
       #4  3501 MHz   77497887 s          0 s    9255269 s  5028877309 s         45 s
       
  Memory: 31.383651733398438 GB (5764.046875 MB free)
  Uptime: 5.1172571e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3355
Commit 8e7ae9f (2018-01-09 14:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101725650 s          0 s   15788499 s  4989236898 s        248 s
       #2  3501 MHz  402951803 s          0 s   17160401 s  4689082741 s         82 s
       #3  3501 MHz   82357519 s          0 s    9329636 s  5024515108 s        110 s
       #4  3501 MHz   77587849 s          0 s    9263159 s  5029757276 s         45 s
       
  Memory: 31.383651733398438 GB (5401.41796875 MB free)
  Uptime: 5.1182354e7 sec
  Load Avg:  1.06103515625  1.03955078125  1.0478515625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
