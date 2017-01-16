# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3c9e6f7b861b2bc22e4417186ece634ba2bd3dba](https://github.com/JuliaLang/julia/commit/3c9e6f7b861b2bc22e4417186ece634ba2bd3dba) vs [JuliaLang/julia@281e2bef9850cc49adf8c96bbbf8c2dcd8c0b7c9](https://github.com/JuliaLang/julia/commit/281e2bef9850cc49adf8c96bbbf8c2dcd8c0b7c9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20025#issuecomment-272778157)

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
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Complex{Float64}","Int")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Float64","Int")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:1.0:100000.0")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 0.30 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","linspace(1.0,2.0,10000)")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:1.0:100000.0")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("norm","Int64")]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["micro","pisum"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float32}")]` | 1.64 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |

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

#### Comparison Build

```
?
```
