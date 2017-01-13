# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ff9a94903adde1980e34090342173fd8a1c96f42](https://github.com/JuliaLang/julia/commit/ff9a94903adde1980e34090342173fd8a1c96f42)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ff9a94903adde1980e34090342173fd8a1c96f42#commitcomment-20462959)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-01-13 vs 2017-01-12

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
| `["array","cat",("hcat_setind",5)]` | 1.07 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.11 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.05 (15%)  | 1.06 (1%) :x: |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.00 (50%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.00 (50%) :white_check_mark: | 0.22 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.00 (50%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","linspace(1.0,2.0,10000)")]` | 0.00 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.96 (50%)  | 1.08 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.00 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 1.02 (50%)  | 1.06 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.00 (50%) :white_check_mark: | 0.13 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 1.03 (50%)  | 1.06 (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 0.64 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000:-1:1")]` | 0.82 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000")]` | 0.69 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 0.56 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 0.57 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.57 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.57 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.54 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.56 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.57 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.57 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 0.92 (50%)  | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.56 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.57 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000)")]` | 0.78 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 1.01 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 1.02 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.01 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.02 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.01 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.01 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.01 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.02 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 1.00 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.54 (50%)  | 0.54 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.53 (50%)  | 0.54 (1%) :white_check_mark: |
| `["problem","go","go_game"]` | 1.01 (15%)  | 1.11 (1%) :x: |

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
- `["broadcast","sparse"]`
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
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
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
- `["tuple","index"]`

## Version Info

#### Primary Build

```
?
```
