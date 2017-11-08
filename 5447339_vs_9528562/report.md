# Benchmark Report

## Job Properties

*Commit(s):* [Sacha0/julia@5447339e807c88dc94ba188ea0b117f252ea8c16](https://github.com/Sacha0/julia/commit/5447339e807c88dc94ba188ea0b117f252ea8c16) vs [JuliaLang/julia@95285623b15a1ca9efbcd24db98b7613d71f3aa7](https://github.com/JuliaLang/julia/commit/95285623b15a1ca9efbcd24db98b7613d71f3aa7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24045#issuecomment-342771928)

*Tag Predicate:* `"sparse" && "matmul"`

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
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 0.12 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 0.06 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 0.08 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 0.22 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 0.29 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.42 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.31 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 0.03 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 0.04 (30%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.03 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.07 (30%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.01 (30%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 0.11 (30%) :white_check_mark: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 0.03 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 0.29 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.22 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 0.11 (30%) :white_check_mark: | 9.84 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 0.96 (30%)  | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.39 (30%) :x: | 9.84 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 0.01 (30%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 0.01 (30%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.01 (30%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.04 (30%) :white_check_mark: | 0.18 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.00 (30%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.02 (30%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 0.13 (30%) :white_check_mark: | 1.01 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 0.03 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 0.31 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.21 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 0.12 (30%) :white_check_mark: | 9.84 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.09 (30%)  | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.51 (30%) :x: | 9.84 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 0.04 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 0.05 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 0.06 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 0.10 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.01 (30%) :white_check_mark: | 1.30 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.00 (30%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.11 (30%) :white_check_mark: | 2.97 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.02 (30%) :white_check_mark: | 0.58 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 0.02 (30%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 0.03 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.04 (30%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.03 (30%) :white_check_mark: | 0.24 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 0.02 (30%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.07 (30%) :white_check_mark: | 0.58 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.24 (30%) :white_check_mark: | 0.28 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.02 (30%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 0.08 (30%) :white_check_mark: | 0.52 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.08 (30%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 0.04 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 0.53 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.17 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 0.05 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 0.62 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 0.48 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 0.24 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.03 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.01 (30%) :white_check_mark: | 1.01 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.00 (30%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.08 (30%) :white_check_mark: | 1.91 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.01 (30%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 0.02 (30%) :white_check_mark: | 0.09 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 0.01 (30%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.02 (30%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.04 (30%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.05 (30%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.21 (30%) :white_check_mark: | 0.36 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.01 (30%) :white_check_mark: | 0.18 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 0.04 (30%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 0.06 (30%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 0.04 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 0.63 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 0.16 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 0.05 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 0.72 (30%)  | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 0.50 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 0.34 (30%) :white_check_mark: | 1.98 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["sparse", "matmul"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2226
Commit 5447339 (2017-10-19 23:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92602386 s          0 s   14386828 s  4461167498 s        201 s
       #2  3501 MHz  368661478 s          0 s   15561432 s  4186108401 s         69 s
       #3  3501 MHz   76188905 s          0 s    8692285 s  4491626394 s         90 s
       #4  3501 MHz   71383028 s          0 s    8556314 s  4496985070 s         36 s
       
  Memory: 31.383651733398438 GB (11946.75 MB free)
  Uptime: 4.5784063e7 sec
  Load Avg:  0.9228515625  1.2099609375  1.572265625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2463
Commit 9528562 (2017-11-08 04:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92687975 s          0 s   14394901 s  4461268182 s        202 s
       #2  3501 MHz  368794942 s          0 s   15569510 s  4186161426 s         69 s
       #3  3501 MHz   76277828 s          0 s    8700000 s  4491724264 s         90 s
       #4  3501 MHz   71483741 s          0 s    8563921 s  4497071417 s         36 s
       
  Memory: 31.383651733398438 GB (11709.07421875 MB free)
  Uptime: 4.5786015e7 sec
  Load Avg:  1.0029296875  1.18994140625  1.74951171875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
