# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1a1a9a63f1b49f8f9e0b0905b834b5fa8d272983](https://github.com/JuliaLang/julia/commit/1a1a9a63f1b49f8f9e0b0905b834b5fa8d272983)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/1a1a9a63f1b49f8f9e0b0905b834b5fa8d272983#commitcomment-18012234)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-25 vs 2016-06-24

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
| `["problem","laplacian","laplace_iter_sub"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigFloat","BigFloat")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Int64")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","UInt64")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 0.81 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 0.72 (50%)  | 0.65 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{UInt64}")]` | 0.79 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Int64")]` | 0.81 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","UInt64")]` | 0.78 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 0.81 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float32}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigInt}")]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.66 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.67 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Int64}")]` | 0.73 (50%)  | 0.65 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Int64")]` | 0.78 (50%)  | 0.57 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 0.78 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigFloat}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 0.71 (50%)  | 0.65 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigInt}")]` | 0.73 (50%)  | 0.65 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigInt")]` | 0.79 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 0.81 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","BigFloat")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","BigInt")]` | 0.81 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","Complex{BigInt}")]` | 0.78 (50%)  | 0.57 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","BigFloat")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","BigInt")]` | 0.78 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 0.78 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","BigFloat")]` | 0.83 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 0.85 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 0.73 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.78 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.78 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 0.86 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 0.86 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Int64")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","UInt64")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","BigFloat")]` | 0.80 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","BigInt")]` | 0.76 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.76 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.79 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.77 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.81 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.81 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 0.78 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 0.84 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigFloat}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigInt}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float32}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float64}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Int64}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{UInt64}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float32")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigFloat}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float32}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float64}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 0.74 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigFloat")]` | 0.84 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigFloat}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 0.85 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigFloat}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 0.80 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigFloat}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 0.80 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigFloat}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 0.74 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.79 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 0.77 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 0.89 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.78 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.76 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","BigFloat")]` | 0.85 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.84 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.73 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","BigFloat")]` | 0.85 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.83 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.72 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","BigFloat")]` | 0.78 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 0.80 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Int64")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","UInt64")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 0.84 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 0.80 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigInt}")]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{UInt64}")]` | 0.84 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Int64")]` | 0.76 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 0.76 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigFloat}")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 0.77 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 0.75 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 0.76 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Int64}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{UInt64}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 0.81 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigInt")]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 0.77 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigInt}")]` | 0.76 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Int64}")]` | 0.70 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{UInt64}")]` | 0.76 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","UInt64")]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 0.80 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 0.76 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 0.80 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 0.77 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigFloat}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigInt}")]` | 0.70 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigInt")]` | 0.83 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigFloat}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigInt}")]` | 0.76 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.74 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","BigFloat")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","BigInt")]` | 0.76 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","BigFloat")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigInt}")]` | 0.81 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","BigFloat")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 0.74 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 0.76 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 0.75 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Int64}")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{UInt64}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Int64")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","UInt64")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 0.77 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigInt}")]` | 0.79 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Int64}")]` | 0.71 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Int64")]` | 0.81 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","UInt64")]` | 0.78 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 0.68 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float32}")]` | 0.78 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 0.78 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 0.72 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 0.82 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.77 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigInt}")]` | 0.82 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Int64}")]` | 0.73 (50%)  | 0.65 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Int64")]` | 0.77 (50%)  | 0.57 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 0.77 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.77 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigFloat}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 0.77 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 0.79 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 0.61 (50%)  | 0.64 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigInt}")]` | 0.65 (50%)  | 0.64 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 0.71 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigInt")]` | 0.72 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 0.79 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 0.83 (50%)  | 0.89 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.70 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 0.78 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.69 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","BigFloat")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","BigInt")]` | 0.69 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 0.72 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigInt}")]` | 0.70 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","BigFloat")]` | 0.75 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","BigInt")]` | 0.64 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 0.73 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","BigFloat")]` | 0.78 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 0.71 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{BigInt}")]` | 0.76 (40%)  | 1.09 (1%) :x: |
| `["scalar","fastmath",("div","BigFloat")]` | 0.84 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","BigInt")]` | 0.76 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","Complex{BigFloat}")]` | 0.70 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 0.75 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","BigFloat")]` | 0.74 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 0.69 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","Complex{BigInt}")]` | 0.81 (40%)  | 1.27 (1%) :x: |
| `["scalar","fastmath",("sub","BigFloat")]` | 0.69 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 0.68 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigInt}")]` | 0.81 (40%)  | 1.27 (1%) :x: |
| `["scalar","predicate",("iseven","BigInt")]` | 0.73 (25%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["scalar","predicate",("isodd","BigInt")]` | 0.72 (25%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.23 (20%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4934
Commit 1a1a9a6 (2016-06-25 02:49 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (26619.4921875 MB free)
Uptime: 2.476997e6 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2517156 s          0 s     567258 s  244060651 s          8 s
#2  3501 MHz    7416482 s          0 s     519382 s  239530377 s          2 s
#3  3501 MHz    2866488 s          0 s     414836 s  244269537 s          2 s
#4  3501 MHz    2007459 s          0 s     379377 s  245195407 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
