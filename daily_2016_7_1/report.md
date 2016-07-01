# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b2b680b13603f7a00e21537a33ac2d26973ca59d](https://github.com/JuliaLang/julia/commit/b2b680b13603f7a00e21537a33ac2d26973ca59d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b2b680b13603f7a00e21537a33ac2d26973ca59d#commitcomment-18090558)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-07-01 vs 2016-06-30

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
| `["parallel","remotecall",("identity",1024)]` | 0.75 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.74 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.77 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.76 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.75 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["problem","imdb","centrality"]` | 1.01 (15%)  | 1.05 (1%) :x: |
| `["problem","json","parse_json"]` | 0.98 (15%)  | 1.01 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 1.06 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.98 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 1.02 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 1.01 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 1.04 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 1.02 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 1.02 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 1.17 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 1.16 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 1.05 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 1.03 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 0.97 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.99 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 1.00 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 0.96 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 1.04 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 1.07 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 1.07 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 0.98 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.99 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 1.21 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 1.18 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 1.03 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 1.17 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 1.01 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 1.17 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 1.00 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 1.02 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 1.05 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 1.01 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 1.16 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 1.04 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 1.08 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 1.08 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.98 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 0.98 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 1.00 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 1.00 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.98 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.19 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.20 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.20 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 1.10 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 1.10 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 1.01 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 0.98 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 0.97 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 0.97 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 1.15 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 1.15 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 1.14 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 1.02 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 1.14 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 1.02 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 1.02 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 1.09 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.99 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 1.10 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.98 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.96 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.00 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.96 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.98 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.97 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 1.01 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 1.00 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 1.01 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 0.97 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 1.19 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 1.15 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 1.15 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 0.96 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigFloat}")]` | 0.96 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 0.96 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 1.05 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 0.91 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Int64}")]` | 0.95 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{UInt64}")]` | 0.94 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 0.95 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 0.98 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 0.98 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 0.97 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 1.16 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 1.18 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 0.99 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 1.15 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 1.19 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 0.95 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 1.16 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigFloat}")]` | 0.94 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 1.01 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigFloat}")]` | 0.95 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 1.13 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 1.16 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 1.13 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 0.95 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 1.16 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 0.98 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 0.98 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 1.04 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 0.98 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Int64}")]` | 0.96 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{UInt64}")]` | 0.96 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 0.99 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 1.11 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 1.11 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 1.05 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 1.04 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 0.98 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.99 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 1.01 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 1.04 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 1.12 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 1.13 (50%)  | 1.31 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.99 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.99 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 1.19 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 1.17 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 1.04 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 1.18 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 1.01 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 1.16 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 1.17 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 1.02 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 0.98 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 1.01 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 1.00 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 1.15 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 1.03 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 1.10 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 1.16 (50%)  | 1.10 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 0.99 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 1.11 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 0.99 (50%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 0.95 (40%)  | 1.05 (1%) :x: |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 0.97 (40%)  | 1.15 (1%) :x: |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 0.98 (40%)  | 1.15 (1%) :x: |
| `["scalar","iteration","indexed"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","fasta"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.09 (1%) :x: |
| `["shootout","revcomp"]` | 0.85 (15%) :white_check_mark: | 1.01 (1%) :x: |
| `["simd",("conditional_loop!","Int32",4095)]` | 59.56 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 63.43 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 26.81 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 27.04 (20%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+5061
Commit b2b680b (2016-07-01 03:07 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (23955.3125 MB free)
Uptime: 2.995365e6 sec
Load Avg:  0.9228515625  0.9853515625  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3496068 s          0 s     851079 s  294405744 s         12 s
#2  3501 MHz   10563164 s          0 s     565454 s  288224636 s          1 s
#3  3501 MHz    4001090 s          0 s     523423 s  294857319 s          3 s
#4  3501 MHz    3398862 s          0 s     514206 s  295462181 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
