# Benchmark Report

## Job Properties

*Commit(s):* [Sacha0/julia@37446654c5aca4d75441ebadc0a72f7fabd29f44](https://github.com/Sacha0/julia/commit/37446654c5aca4d75441ebadc0a72f7fabd29f44) vs [JuliaLang/julia@8afbe45b5b1f3e8bd2010f2fa85c5854e9c4fa0a](https://github.com/JuliaLang/julia/commit/8afbe45b5b1f3e8bd2010f2fa85c5854e9c4fa0a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24045#issuecomment-335636416)

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
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.00 (25%)  | 1.01 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.95 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","atan2",("x one","Float64")]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("A_mul_B!","dense 4000x40, sparse 40x40 -> dense 4000x40")]` | 0.13 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B!","dense 400x40, sparse 40x400 -> dense 400x400")]` | 0.06 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B!","dense 400x400, sparse 400x40 -> dense 400x40")]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B!","dense 400x400, sparse 400x400 -> dense 400x400")]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B!","dense 40x40, sparse 40x4000 -> dense 40x4000")]` | 0.08 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B!","dense 40x400, sparse 400x4000 -> dense 40x4000")]` | 0.01 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B!","dense 40x4000, sparse 4000x400 -> dense 40x400")]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B!","dense 40x4000, sparse 4000x4000 -> dense 40x4000")]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_B","dense 500x5, sparse 5x5 -> dense 500x5")]` | 0.24 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","matmul",("A_mul_B","dense 50x5, sparse 5x50 -> dense 50x50")]` | 0.31 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","matmul",("A_mul_B","dense 50x50, sparse 50x5 -> dense 50x5")]` | 0.45 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","matmul",("A_mul_B","dense 50x50, sparse 50x50 -> dense 50x50")]` | 0.30 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","matmul",("A_mul_Bc","dense 500x5, sparse 5x5 -> dense 500x5")]` | 0.05 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","dense 50x5, sparse 50x5 -> dense 50x50")]` | 0.06 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","dense 50x50, sparse 50x50 -> dense 50x50")]` | 0.04 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","dense 50x50, sparse 5x50 -> dense 50x5")]` | 0.07 (30%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","dense 5x5, sparse 500x5 -> dense 5x500")]` | 0.09 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","dense 5x50, sparse 500x50 -> dense 5x500")]` | 0.04 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","dense 5x500, sparse 500x500 -> dense 5x500")]` | 0.01 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","dense 5x500, sparse 50x500 -> dense 5x50")]` | 0.01 (30%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bc","sparse 500x5, dense 5x5 -> dense 500x5")]` | 0.12 (30%) :white_check_mark: | 1.01 (1%)  |
| `["sparse","matmul",("A_mul_Bc","sparse 500x50, dense 5x50 -> dense 500x5")]` | 0.03 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse","matmul",("A_mul_Bc","sparse 500x500, dense 5x500 -> dense 500x5")]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("A_mul_Bc","sparse 50x5, dense 50x5 -> dense 50x50")]` | 0.30 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse","matmul",("A_mul_Bc","sparse 50x50, dense 50x50 -> dense 50x50")]` | 0.22 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("A_mul_Bc","sparse 50x500, dense 5x500 -> dense 50x5")]` | 0.11 (30%) :white_check_mark: | 9.84 (1%) :x: |
| `["sparse","matmul",("A_mul_Bc","sparse 5x5, dense 500x5 -> dense 5x500")]` | 0.81 (30%)  | 1.98 (1%) :x: |
| `["sparse","matmul",("A_mul_Bc","sparse 5x50, dense 50x50 -> dense 5x50")]` | 1.50 (30%) :x: | 9.84 (1%) :x: |
| `["sparse","matmul",("A_mul_Bt","dense 500x5, sparse 5x5 -> dense 500x5")]` | 0.01 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","dense 50x5, sparse 50x5 -> dense 50x50")]` | 0.03 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","dense 50x50, sparse 50x50 -> dense 50x50")]` | 0.02 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","dense 50x50, sparse 5x50 -> dense 50x5")]` | 0.07 (30%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","dense 5x5, sparse 500x5 -> dense 5x500")]` | 0.05 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","dense 5x50, sparse 500x50 -> dense 5x500")]` | 0.03 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","dense 5x500, sparse 500x500 -> dense 5x500")]` | 0.01 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","dense 5x500, sparse 50x500 -> dense 5x50")]` | 0.02 (30%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["sparse","matmul",("A_mul_Bt","sparse 500x5, dense 5x5 -> dense 500x5")]` | 0.12 (30%) :white_check_mark: | 1.01 (1%)  |
| `["sparse","matmul",("A_mul_Bt","sparse 500x50, dense 5x50 -> dense 500x5")]` | 0.03 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse","matmul",("A_mul_Bt","sparse 500x500, dense 5x500 -> dense 500x5")]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("A_mul_Bt","sparse 50x5, dense 50x5 -> dense 50x50")]` | 0.27 (30%) :white_check_mark: | 1.09 (1%) :x: |
| `["sparse","matmul",("A_mul_Bt","sparse 50x50, dense 50x50 -> dense 50x50")]` | 0.19 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("A_mul_Bt","sparse 50x500, dense 5x500 -> dense 50x5")]` | 0.11 (30%) :white_check_mark: | 9.84 (1%) :x: |
| `["sparse","matmul",("A_mul_Bt","sparse 5x5, dense 500x5 -> dense 5x500")]` | 1.13 (30%)  | 1.98 (1%) :x: |
| `["sparse","matmul",("A_mul_Bt","sparse 5x50, dense 50x50 -> dense 5x50")]` | 1.54 (30%) :x: | 9.84 (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 2000x20, sparse 2000x200 -> dense 20x200")]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 2000x20, sparse 2000x2000 -> dense 20x2000")]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 200x20, sparse 200x2000 -> dense 20x2000")]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 200x200, sparse 200x20 -> dense 200x20")]` | 0.03 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 200x200, sparse 200x200 -> dense 200x200")]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 20x20, sparse 20x2000 -> dense 20x2000")]` | 0.05 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 20x200, sparse 20x200 -> dense 200x200")]` | 0.05 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","dense 20x2000, sparse 20x20 -> dense 2000x20")]` | 0.11 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("Ac_mul_B!","sparse 2000x200, dense 2000x20 -> dense 200x20")]` | 1.71 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B!","sparse 2000x2000, dense 2000x20 -> dense 2000x20")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B!","sparse 200x20, dense 200x200 -> dense 20x200")]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B!","sparse 200x200, dense 200x200 -> dense 200x200")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B!","sparse 200x2000, dense 200x20 -> dense 2000x20")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B!","sparse 20x2000, dense 20x20 -> dense 2000x20")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B","dense 500x5, sparse 500x50 -> dense 5x50")]` | 0.01 (30%) :white_check_mark: | 1.70 (1%) :x: |
| `["sparse","matmul",("Ac_mul_B","dense 500x5, sparse 500x500 -> dense 5x500")]` | 0.01 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_B","dense 50x5, sparse 50x500 -> dense 5x500")]` | 0.02 (30%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_B","dense 50x50, sparse 50x5 -> dense 50x5")]` | 0.11 (30%) :white_check_mark: | 1.73 (1%) :x: |
| `["sparse","matmul",("Ac_mul_B","dense 50x50, sparse 50x50 -> dense 50x50")]` | 0.02 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_B","dense 5x5, sparse 5x500 -> dense 5x500")]` | 0.04 (30%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_B","dense 5x50, sparse 5x50 -> dense 50x50")]` | 0.03 (30%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_B","dense 5x500, sparse 5x5 -> dense 500x5")]` | 0.05 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_B","sparse 500x50, dense 500x5 -> dense 50x5")]` | 1.77 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B","sparse 50x5, dense 50x50 -> dense 5x50")]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B","sparse 50x500, dense 50x5 -> dense 500x5")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B","sparse 5x50, dense 5x50 -> dense 50x50")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_B","sparse 5x500, dense 5x5 -> dense 500x5")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("Ac_mul_Bc","dense 500x5, sparse 500x500 -> dense 5x500")]` | 0.01 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","dense 500x5, sparse 50x500 -> dense 5x50")]` | 0.03 (30%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","dense 50x5, sparse 500x50 -> dense 5x500")]` | 0.06 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","dense 50x50, sparse 50x50 -> dense 50x50")]` | 0.10 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","dense 50x50, sparse 5x50 -> dense 50x5")]` | 0.26 (30%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","dense 5x5, sparse 500x5 -> dense 5x500")]` | 0.14 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","dense 5x50, sparse 50x5 -> dense 50x50")]` | 0.14 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","dense 5x500, sparse 5x5 -> dense 500x5")]` | 0.11 (30%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 500x50, dense 5x500 -> dense 50x5")]` | 0.05 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 500x500, dense 5x500 -> dense 500x5")]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 50x5, dense 50x50 -> dense 5x50")]` | 0.57 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 50x50, dense 50x50 -> dense 50x50")]` | 0.15 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 50x500, dense 5x50 -> dense 500x5")]` | 0.05 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 5x5, dense 500x5 -> dense 5x500")]` | 0.47 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 5x50, dense 50x5 -> dense 50x50")]` | 0.50 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("Ac_mul_Bc","sparse 5x500, dense 5x5 -> dense 500x5")]` | 0.27 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 4000x40, sparse 4000x400 -> dense 40x400")]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 4000x40, sparse 4000x4000 -> dense 40x4000")]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 400x40, sparse 400x4000 -> dense 40x4000")]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 400x400, sparse 400x40 -> dense 400x40")]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 400x400, sparse 400x400 -> dense 400x400")]` | 0.00 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 40x40, sparse 40x4000 -> dense 40x4000")]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 40x400, sparse 40x400 -> dense 400x400")]` | 0.01 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","dense 40x4000, sparse 40x40 -> dense 4000x40")]` | 0.03 (30%) :white_check_mark: | Inf (1%) :x: |
| `["sparse","matmul",("At_mul_B!","sparse 4000x400, dense 4000x40 -> dense 400x40")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B!","sparse 4000x4000, dense 4000x40 -> dense 4000x40")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B!","sparse 400x40, dense 400x400 -> dense 40x400")]` | 1.95 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B!","sparse 400x400, dense 400x400 -> dense 400x400")]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B!","sparse 400x4000, dense 400x40 -> dense 4000x40")]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B!","sparse 40x40, dense 40x4000 -> dense 40x4000")]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B!","sparse 40x4000, dense 40x40 -> dense 4000x40")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B","dense 500x5, sparse 500x50 -> dense 5x50")]` | 0.01 (30%) :white_check_mark: | 1.25 (1%) :x: |
| `["sparse","matmul",("At_mul_B","dense 500x5, sparse 500x500 -> dense 5x500")]` | 0.00 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_B","dense 50x5, sparse 50x500 -> dense 5x500")]` | 0.02 (30%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_B","dense 50x50, sparse 50x5 -> dense 50x5")]` | 0.08 (30%) :white_check_mark: | 1.28 (1%) :x: |
| `["sparse","matmul",("At_mul_B","dense 50x50, sparse 50x50 -> dense 50x50")]` | 0.01 (30%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_B","dense 5x5, sparse 5x500 -> dense 5x500")]` | 0.03 (30%) :white_check_mark: | 0.15 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_B","dense 5x50, sparse 5x50 -> dense 50x50")]` | 0.01 (30%) :white_check_mark: | 0.17 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_B","dense 5x500, sparse 5x5 -> dense 500x5")]` | 0.02 (30%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_B","sparse 500x50, dense 500x5 -> dense 50x5")]` | 1.78 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B","sparse 500x500, dense 500x5 -> dense 500x5")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B","sparse 50x5, dense 50x50 -> dense 5x50")]` | 1.90 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B","sparse 50x500, dense 50x5 -> dense 500x5")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_B","sparse 5x500, dense 5x5 -> dense 500x5")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","matmul",("At_mul_Bt","dense 500x5, sparse 500x500 -> dense 5x500")]` | 0.01 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","dense 500x5, sparse 50x500 -> dense 5x50")]` | 0.04 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","dense 50x5, sparse 500x50 -> dense 5x500")]` | 0.03 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","dense 50x50, sparse 50x50 -> dense 50x50")]` | 0.08 (30%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","dense 50x50, sparse 5x50 -> dense 50x5")]` | 0.27 (30%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","dense 5x5, sparse 500x5 -> dense 5x500")]` | 0.06 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","dense 5x50, sparse 50x5 -> dense 50x50")]` | 0.08 (30%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","dense 5x500, sparse 5x5 -> dense 500x5")]` | 0.07 (30%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["sparse","matmul",("At_mul_Bt","sparse 500x50, dense 5x500 -> dense 50x5")]` | 0.05 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse","matmul",("At_mul_Bt","sparse 500x500, dense 5x500 -> dense 500x5")]` | 0.01 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("At_mul_Bt","sparse 50x5, dense 50x50 -> dense 5x50")]` | 0.62 (30%) :white_check_mark: | 1.85 (1%) :x: |
| `["sparse","matmul",("At_mul_Bt","sparse 50x50, dense 50x50 -> dense 50x50")]` | 0.14 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("At_mul_Bt","sparse 50x500, dense 5x50 -> dense 500x5")]` | 0.06 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("At_mul_Bt","sparse 5x5, dense 500x5 -> dense 5x500")]` | 0.70 (30%)  | 1.98 (1%) :x: |
| `["sparse","matmul",("At_mul_Bt","sparse 5x50, dense 50x5 -> dense 50x50")]` | 0.47 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","matmul",("At_mul_Bt","sparse 5x500, dense 5x5 -> dense 500x5")]` | 0.36 (30%) :white_check_mark: | 1.98 (1%) :x: |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.70 (30%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","atan2"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","sincos"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","matmul"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2118
Commit 3744665 (2017-10-10 22:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   89607720 s          0 s   13914688 s  4220205114 s        181 s
       #2  3501 MHz  362386970 s          0 s   14938389 s  3948471315 s         66 s
       #3  3501 MHz   75002666 s          0 s    8538283 s  4248034886 s         86 s
       #4  3501 MHz   70217566 s          0 s    8414420 s  4253347836 s         32 s
       
  Memory: 31.383651733398438 GB (3238.17578125 MB free)
  Uptime: 4.3334223e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2115
Commit 8afbe45 (2017-10-10 22:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   89690604 s          0 s   13924928 s  4220925712 s        182 s
       #2  3501 MHz  363139933 s          0 s   14950248 s  3948522537 s         66 s
       #3  3501 MHz   75100814 s          0 s    8546482 s  4248744533 s         86 s
       #4  3501 MHz   70297457 s          0 s    8422190 s  4254076524 s         32 s
       
  Memory: 31.383651733398438 GB (3238.015625 MB free)
  Uptime: 4.3342393e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
