# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fd03b1e536114a43906c4f910298edd5b10f2cc6](https://github.com/JuliaLang/julia/commit/fd03b1e536114a43906c4f910298edd5b10f2cc6) vs [JuliaLang/julia@8fd280f06b7490872cabc1a3d0f20e70f74a4cb7](https://github.com/JuliaLang/julia/commit/8fd280f06b7490872cabc1a3d0f20e70f74a4cb7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20485#issuecomment-278362159)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",2048)]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["array","index","3d"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["array","index","4d"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","index","5d"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","index","7d"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.90 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.20 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.21 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 2.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 2.02 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.90 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.90 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.10 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.11 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.91 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 2.13 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 2.18 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 2.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.03 (15%)  | 1.03 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.06 (15%)  | 1.03 (1%) :x: |
| `["problem","laplacian","laplace_iter_devec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ones")]` | 2.01 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ones")]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 2.02 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.80 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.93 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","random")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","random")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.94 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","random")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.88 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 1.84 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.91 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","random")]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 2.02 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 2.05 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ones")]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","random")]` | 1.56 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 2.07 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 2.03 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ones")]` | 2.07 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","random")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 2.07 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 2.11 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 2.11 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 2.08 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 2.04 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 2.08 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","random")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 1.28 (30%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 2.43 (30%) :x: | 1.01 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 2.75 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 1.66 (30%) :x: | 1.04 (1%) :x: |
| `["sparse","index",("spmat","logical",100)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",10)]` | 0.89 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 1.00 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.01 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.43 (30%) :x: | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 2.11 (30%) :x: | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",1000)]` | 2.15 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",10)]` | 0.99 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 1.05 (30%)  | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.05 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spvec","array",1000)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",10000)]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",100000)]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",1000)]` | 3.11 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",10000)]` | 2.06 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",100000)]` | 2.03 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.53 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2670
Commit fd03b1e (2017-02-08 14:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18692.9921875 MB free)
Uptime: 2.2221779e7 sec
Load Avg:  0.9228515625  0.998046875  0.98681640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44711368 s          0 s    6973858 s  2165815752 s         66 s
#2  3501 MHz  140902204 s          0 s    7444736 s  2070227466 s         22 s
#3  3501 MHz   36318274 s          0 s    4358243 s  2180486376 s         37 s
#4  3501 MHz   32446460 s          0 s    4294917 s  2184629339 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2668
Commit 8fd280f (2017-02-08 14:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18264.1640625 MB free)
Uptime: 2.2229707e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   44786462 s          0 s    6983612 s  2166521209 s         66 s
#2  3501 MHz  141399458 s          0 s    7452478 s  2070514564 s         22 s
#3  3501 MHz   36394081 s          0 s    4365178 s  2181195476 s         37 s
#4  3501 MHz   32558487 s          0 s    4304107 s  2185300312 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
