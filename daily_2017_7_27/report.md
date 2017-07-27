# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@af7a92799edb611151166f830270d83d3d7e03cd](https://github.com/JuliaLang/julia/commit/af7a92799edb611151166f830270d83d3d7e03cd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/af7a92799edb611151166f830270d83d3d7e03cd#commitcomment-23325633)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-07-27 vs 2017-07-26

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
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","BigFloat")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","Array","BigInt")]` | 0.93 (50%)  | 0.76 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","NullableArray","BigFloat")]` | 1.00 (50%)  | 0.87 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","NullableArray","BigInt")]` | 0.91 (50%)  | 0.81 (1%) :white_check_mark: |
| `["random","collections",("rand","RandomDevice","small IntSet")]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","BigInt","1:1")]` | 0.75 (25%)  | 0.86 (1%) :white_check_mark: |
| `["random","ranges",("RangeGenerator","BigInt","1:170141183460469231731687303715884105728")]` | 0.75 (25%)  | 0.87 (1%) :white_check_mark: |
| `["random","ranges",("RangeGenerator","BigInt","1:18446744073709551615")]` | 0.76 (25%)  | 0.86 (1%) :white_check_mark: |
| `["random","ranges",("RangeGenerator","BigInt","1:18446744073709551616")]` | 0.76 (25%)  | 0.87 (1%) :white_check_mark: |
| `["random","ranges",("RangeGenerator","BigInt","1:2^10000")]` | 1.07 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","ranges",("RangeGenerator","BigInt","1:4294967295")]` | 0.77 (25%)  | 0.86 (1%) :white_check_mark: |
| `["random","ranges",("RangeGenerator","BigInt","1:4294967297")]` | 0.77 (25%)  | 0.86 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.91 (25%)  | 0.96 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.87 (25%)  | 0.95 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:18446744073709551615)")]` | 0.87 (25%)  | 0.95 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:18446744073709551616)")]` | 0.85 (25%)  | 0.95 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:2^10000)")]` | 0.97 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967295)")]` | 0.88 (25%)  | 0.95 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.95 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 1.84 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.96 (25%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","BigFloat")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.95 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.98 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 0.98 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","Int64")]` | 1.02 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigFloat","UInt64")]` | 1.03 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 0.99 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","BigInt")]` | 0.69 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 1.00 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigInt}")]` | 0.72 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{UInt64}")]` | 0.78 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Int64")]` | 0.70 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","UInt64")]` | 0.70 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 1.00 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 1.00 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 1.08 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.99 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float32}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 1.02 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 1.01 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 1.00 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 1.01 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 1.01 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 0.98 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigInt")]` | 0.71 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.97 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigInt}")]` | 0.81 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.98 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Int64}")]` | 0.76 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{UInt64}")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Int64")]` | 0.72 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 0.72 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.99 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 0.97 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.98 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 0.75 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigInt}")]` | 0.80 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigInt")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigInt}")]` | 0.78 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 1.00 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.98 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 1.00 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","BigFloat")]` | 1.02 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","BigInt")]` | 0.69 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 1.00 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Int64","Complex{BigInt}")]` | 0.73 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","BigFloat")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","BigInt")]` | 0.71 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 0.97 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 0.72 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","BigFloat")]` | 1.02 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 0.99 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Int64")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","UInt64")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","BigFloat")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","BigInt")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.00 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.00 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.00 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.00 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.00 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 0.98 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 1.02 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.96 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigInt}")]` | 0.92 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float32}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float64}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Int64}")]` | 0.94 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{UInt64}")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float32")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigFloat}")]` | 0.91 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 1.01 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float32}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float64}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 0.98 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 0.98 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.99 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigFloat")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.96 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigInt}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigFloat}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigInt}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 0.95 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 1.00 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigFloat}")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 0.98 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 1.01 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.99 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 0.99 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.00 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 0.99 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.00 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 1.00 (50%)  | 0.84 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","BigFloat")]` | 1.04 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 1.02 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","BigFloat")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","BigFloat")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 0.99 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","Int64")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigFloat","UInt64")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","BigInt")]` | 0.73 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigInt}")]` | 0.81 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Int64}")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{UInt64}")]` | 0.75 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.95 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.96 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Int64")]` | 0.71 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","UInt64")]` | 0.72 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 1.00 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 1.00 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 0.99 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Int64}")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{UInt64}")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 1.01 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 1.01 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigInt")]` | 0.81 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigInt}")]` | 0.84 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.95 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Int64}")]` | 0.83 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{UInt64}")]` | 0.83 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Int64")]` | 0.78 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","UInt64")]` | 0.81 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.98 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.98 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 1.01 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.95 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 1.05 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigInt")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigFloat}")]` | 0.95 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigInt}")]` | 0.84 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigInt")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigFloat}")]` | 0.96 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigInt}")]` | 0.83 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.96 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 1.01 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 1.01 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.95 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","BigFloat")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","BigInt")]` | 0.69 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Int64","Complex{BigInt}")]` | 0.77 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","BigFloat")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","BigInt")]` | 0.72 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 0.94 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigInt}")]` | 0.78 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("rem type","Bool","BigInt")]` | 0.95 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","arithmetic",("rem type","Char","BigInt")]` | 0.92 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","arithmetic",("rem type","Int64","BigInt")]` | 0.92 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","arithmetic",("rem type","UInt64","BigInt")]` | 0.92 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","BigFloat")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 0.99 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 0.96 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 0.93 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 0.94 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Int64}")]` | 1.00 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{UInt64}")]` | 1.00 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 0.99 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","Int64")]` | 1.01 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigFloat","UInt64")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 0.99 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","BigInt")]` | 0.71 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 0.94 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigInt}")]` | 0.80 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 1.04 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Int64}")]` | 0.85 (50%)  | 0.77 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{UInt64}")]` | 0.84 (50%)  | 0.77 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.97 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Int64")]` | 0.69 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","UInt64")]` | 0.71 (50%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 0.99 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 0.99 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.98 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float32}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 1.00 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 0.95 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 0.99 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 1.00 (50%)  | 0.81 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.94 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigInt")]` | 0.72 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.95 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigInt}")]` | 0.80 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.94 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Int64}")]` | 0.75 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{UInt64}")]` | 0.79 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Int64")]` | 0.71 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 0.72 (50%)  | 0.83 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.95 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigFloat}")]` | 0.99 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 0.94 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.98 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.96 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 1.00 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 1.00 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigInt}")]` | 1.04 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigInt")]` | 1.02 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 0.98 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigInt}")]` | 1.05 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 0.99 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.98 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 0.97 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 1.00 (50%)  | 0.76 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.99 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 0.95 (50%)  | 0.82 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.94 (50%)  | 0.86 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","BigFloat")]` | 0.98 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","BigInt")]` | 1.01 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 0.96 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Int64","Complex{BigInt}")]` | 1.08 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","BigFloat")]` | 1.00 (50%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","BigInt")]` | 1.00 (50%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 0.97 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigInt}")]` | 1.05 (50%)  | 0.78 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","BigFloat")]` | 0.99 (40%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","BigInt")]` | 0.69 (40%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 0.98 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("add","Complex{BigInt}")]` | 0.81 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","BigFloat")]` | 1.02 (40%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","BigInt")]` | 1.07 (40%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","Complex{BigFloat}")]` | 0.97 (40%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 1.00 (40%)  | 0.80 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","BigFloat")]` | 1.01 (40%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","BigInt")]` | 0.73 (40%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 0.99 (40%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","Complex{BigInt}")]` | 0.84 (40%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","BigFloat")]` | 0.99 (40%)  | 0.85 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","BigInt")]` | 0.71 (40%)  | 0.75 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 0.97 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","fastmath",("sub","Complex{BigInt}")]` | 0.80 (40%)  | 0.79 (1%) :white_check_mark: |
| `["scalar","intfuncs",("nextpow2","BigInt","+")]` | 0.85 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","intfuncs",("nextpow2","BigInt","-")]` | 0.86 (40%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","BigInt","+")]` | 0.82 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","BigInt","-")]` | 0.82 (40%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","predicate",("iseven","BigInt")]` | 0.99 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","predicate",("isfinite","Float64")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","BigInt")]` | 1.00 (40%)  | 0.71 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
- `["scalar","arithmetic"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","sin"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1133
Commit af7a927 (2017-07-26 23:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   79255893 s          0 s   14485298 s  3573517900 s         85 s
       #2  3501 MHz  323622397 s          0 s    8993752 s  3343224905 s         13 s
       #3  3501 MHz   69026641 s          0 s    8023589 s  3599176258 s         70 s
       #4  3501 MHz   65837040 s          0 s    8215813 s  3602153293 s         16 s
       
  Memory: 31.383651733398438 GB (2986.359375 MB free)
  Uptime: 3.6779858e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
