# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7a65d001b952e57a4907c071a5590080c7065ac2](https://github.com/JuliaLang/julia/commit/7a65d001b952e57a4907c071a5590080c7065ac2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/7a65d001b952e57a4907c071a5590080c7065ac2#commitcomment-17928583)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-20 vs 2016-06-19

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
| `["linalg","blas","gemv!"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigFloat","BigFloat")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.91 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.90 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 0.90 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Int64")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","UInt64")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 0.88 (50%)  | 1.21 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{UInt64}")]` | 0.88 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Int64")]` | 0.90 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","UInt64")]` | 0.91 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 0.79 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.88 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float32}")]` | 0.94 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 0.95 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 0.91 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.87 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Int64}")]` | 0.88 (50%)  | 1.21 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{UInt64}")]` | 0.90 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Int64")]` | 0.91 (50%)  | 1.17 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 0.91 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.91 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigFloat}")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 0.90 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 0.90 (50%)  | 1.21 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigInt}")]` | 0.88 (50%)  | 1.21 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigInt")]` | 0.87 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigInt}")]` | 0.90 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Int64","BigFloat")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Int64","BigInt")]` | 0.91 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Int64","Complex{BigInt}")]` | 0.92 (50%)  | 1.17 (1%) :x: |
| `["scalar","arithmetic",("add","UInt64","BigFloat")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","UInt64","BigInt")]` | 0.90 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 0.91 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","BigFloat")]` | 0.93 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 0.81 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 0.94 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Int64")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","UInt64")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","BigFloat")]` | 0.90 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","BigInt")]` | 0.89 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.84 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.82 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.89 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.89 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.91 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.90 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigFloat}")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigInt}")]` | 0.83 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float32}")]` | 0.84 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float64}")]` | 0.84 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Int64}")]` | 0.83 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{UInt64}")]` | 0.84 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float32")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigFloat}")]` | 0.80 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 0.87 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float32}")]` | 0.88 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float64}")]` | 0.85 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 0.90 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigFloat")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigFloat}")]` | 0.86 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigInt}")]` | 0.88 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 0.94 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigFloat}")]` | 0.81 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigInt}")]` | 0.80 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 0.89 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 0.92 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigFloat}")]` | 0.86 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 0.90 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 0.89 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.91 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigFloat}")]` | 0.89 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 0.87 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 0.95 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.90 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.88 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 0.83 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 0.94 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.89 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.87 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.82 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","BigFloat")]` | 0.93 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.90 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.83 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","BigFloat")]` | 0.93 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.92 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.85 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","BigFloat")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 0.80 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Int64")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","UInt64")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Int64}")]` | 0.85 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Int64")]` | 0.91 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigFloat}")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 0.86 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Int64}")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{UInt64}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 0.90 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Int64}")]` | 0.84 (50%)  | 1.18 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Int64")]` | 0.85 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 0.88 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 0.80 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigInt")]` | 0.85 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigFloat}")]` | 0.80 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigInt}")]` | 0.83 (50%)  | 1.18 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigFloat}")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.88 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.87 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Int64","BigFloat")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Int64","BigInt")]` | 0.91 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigInt}")]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","UInt64","BigFloat")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","BigFloat")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 0.88 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 0.88 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 0.88 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Int64}")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{UInt64}")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 0.90 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Int64")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","UInt64")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigInt}")]` | 0.85 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.83 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Int64}")]` | 0.83 (50%)  | 1.23 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{UInt64}")]` | 0.86 (50%)  | 1.18 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Int64")]` | 0.89 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","UInt64")]` | 0.90 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 0.93 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 0.80 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.88 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float32}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 0.90 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 0.90 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.86 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.80 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.79 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Int64}")]` | 0.84 (50%)  | 1.21 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{UInt64}")]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Int64")]` | 0.90 (50%)  | 1.17 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 0.89 (50%)  | 1.25 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigFloat}")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.82 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 0.92 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.80 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 0.84 (50%)  | 1.22 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 0.81 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigInt}")]` | 0.80 (50%)  | 1.22 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigInt")]` | 0.83 (50%)  | 1.14 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 0.84 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigInt}")]` | 0.85 (50%)  | 1.29 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 0.91 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 0.89 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Int64","BigFloat")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Int64","BigInt")]` | 0.84 (50%)  | 1.29 (1%) :x: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 0.85 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigInt}")]` | 0.83 (50%)  | 1.22 (1%) :x: |
| `["scalar","arithmetic",("sub","UInt64","BigFloat")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","UInt64","BigInt")]` | 0.84 (50%)  | 1.29 (1%) :x: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 0.86 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigInt}")]` | 0.83 (50%)  | 1.29 (1%) :x: |
| `["scalar","fastmath",("add","BigFloat")]` | 0.88 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 0.86 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("div","BigFloat")]` | 0.93 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("div","BigInt")]` | 0.90 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("div","Complex{BigFloat}")]` | 0.91 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 0.88 (40%)  | 1.14 (1%) :x: |
| `["scalar","fastmath",("mul","BigFloat")]` | 0.83 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 0.79 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("sub","BigFloat")]` | 0.82 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 0.81 (40%)  | 1.15 (1%) :x: |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("iseven","BigInt")]` | 0.82 (25%)  | 1.14 (1%) :x: |
| `["scalar","predicate",("isodd","BigInt")]` | 0.82 (25%)  | 1.14 (1%) :x: |
| `["shootout","revcomp"]` | 0.76 (15%) :white_check_mark: | 1.01 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.19 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["io"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem"]`
- `["problem","seismic"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4871
Commit 7a65d00 (2016-06-19 23:46 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (26745.8828125 MB free)
Uptime: 2.045027e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96044921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2519873 s          0 s     596998 s  200855759 s          6 s
#2  3501 MHz    8572493 s          0 s     439662 s  195361291 s          1 s
#3  3501 MHz    3444774 s          0 s     426723 s  200511934 s          1 s
#4  3501 MHz    2794146 s          0 s     398715 s  201196377 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
