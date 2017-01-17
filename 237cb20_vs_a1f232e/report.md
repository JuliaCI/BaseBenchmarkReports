# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@237cb207cefaa050c9ca94a0f1f4ef8a32a788f6](https://github.com/JuliaLang/julia/commit/237cb207cefaa050c9ca94a0f1f4ef8a32a788f6) vs [JuliaLang/julia@a1f232e77411fcb18e314be1f6f1caa281499f3b](https://github.com/JuliaLang/julia/commit/a1f232e77411fcb18e314be1f6f1caa281499f3b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20025#issuecomment-272988275)

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
| `["array","cat",("hcat",5)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Complex{Float64}","Int")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Float64","Int")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1.0:1.0:100000.0")]` | 0.34 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 0.30 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","linspace(1.0,2.0,10000)")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1.0:1.0:100000.0")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","linspace(1.0,2.0,10000)")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","linspace(1.0,2.0,10000)")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("norm","Int64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 0.36 (15%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),2)]` | 0.29 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["micro","pisum"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float32}")]` | 1.64 (25%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","arithmetic",("unary minus",(600,600))]` | 0.08 (30%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","index",("spmat","array",10)]` | 0.12 (30%) :white_check_mark: | 0.56 (1%) :white_check_mark: |
| `["sparse","index",("spmat","array",100)]` | 0.01 (30%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["sparse","index",("spmat","array",1000)]` | 0.00 (30%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 0.41 (30%) :white_check_mark: | 1.13 (1%) :x: |
| `["sparse","index",("spmat","col","array",100)]` | 0.39 (30%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",1000)]` | 0.16 (30%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","logical",10)]` | 37.40 (30%) :x: | 2.43 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 16.68 (30%) :x: | 1.18 (1%) :x: |
| `["sparse","index",("spmat","col","logical",1000)]` | 2.54 (30%) :x: | 0.44 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 0.84 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.76 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.45 (30%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["sparse","index",("spmat","integer",10)]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","integer",100)]` | 0.56 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","integer",1000)]` | 0.45 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 33.27 (30%) :x: | 2.27 (1%) :x: |
| `["sparse","index",("spmat","logical",100)]` | 2.17 (30%) :x: | 0.43 (1%) :white_check_mark: |
| `["sparse","index",("spmat","logical",1000)]` | 0.11 (30%) :white_check_mark: | 0.10 (1%) :white_check_mark: |
| `["sparse","index",("spmat","range",10)]` | 0.50 (30%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["sparse","index",("spmat","range",100)]` | 0.14 (30%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["sparse","index",("spmat","range",1000)]` | 0.05 (30%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",10)]` | 0.45 (30%) :white_check_mark: | 0.70 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 0.24 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.12 (30%) :white_check_mark: | 0.16 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 0.65 (30%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.53 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",1000)]` | 0.42 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",10)]` | 0.39 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",100)]` | 0.16 (30%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",1000)]` | 0.06 (30%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.00 (30%) :white_check_mark: | 0.57 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 0.00 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.00 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 0.07 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 0.06 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,400))]` | 0.08 (30%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,600))]` | 0.06 (30%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 0.00 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.00 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(600,400))]` | 0.09 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(600,600))]` | 0.06 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,10000))]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(600,400))]` | 0.10 (30%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(600,600))]` | 0.07 (30%) :white_check_mark: | 0.08 (1%) :white_check_mark: |

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
