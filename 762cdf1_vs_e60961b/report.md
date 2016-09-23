# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@762cdf14382f4979df6ff9f909d0af9f053082dc](https://github.com/JuliaLang/julia/commit/762cdf14382f4979df6ff9f909d0af9f053082dc) vs [JuliaLang/julia@e60961be73e79eee5094f85b3aafbf785ac96fce](https://github.com/JuliaLang/julia/commit/e60961be73e79eee5094f85b3aafbf785ac96fce)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/762cdf14382f4979df6ff9f909d0af9f053082dc#commitcomment-19146596)

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
| `["array","bool","bitarray_true_fill!"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","bool","boolarray_true_load!"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd",500)]` | 1.59 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.61 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sum","3darray")]` | 8.35 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","Array{Int32,2}")]` | 1.62 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.62 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.62 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.66 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 1.59 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 1.96 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","Array{Int32,2}")]` | 3.22 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 3.22 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.61 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.51 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.61 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.69 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 1.71 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","Array{Int32,2}")]` | 3.22 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 3.22 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 1.59 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 1.96 (40%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 1.87 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["linalg","blas","axpy!"]` | 2.05 (40%) :x: | 1.00 (1%)  |
| `["linalg","blas","scal!"]` | 1.93 (40%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.53 (25%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(0)")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","Array")]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","NullableArray")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","Array")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 4.12 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 3.83 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 3.52 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 4.48 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 3.65 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Complex{Float64}")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float64")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Bool")]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Complex{Float64}")]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float32")]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float64")]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int64")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int8")]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float32")]` | 6.84 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float64")]` | 3.29 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int64")]` | 2.70 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int8")]` | 21.65 (15%) :x: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float32")]` | 2.21 (15%) :x: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float64")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4095)]` | 9.09 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4096)]` | 9.63 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4095)]` | 4.77 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4096)]` | 4.83 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4095)]` | 7.72 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4096)]` | 8.09 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4095)]` | 1.41 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4096)]` | 1.47 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 3.80 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 3.89 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 1.97 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 1.98 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 1.88 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 1.97 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 1.81 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 1.90 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 13.31 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 13.91 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 6.96 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 7.03 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int32",4095)]` | 7.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int32",4096)]` | 7.40 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 5.77 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 6.29 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 5.77 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 6.33 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.28 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 3.36 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 3.28 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 3.36 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 4.14 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 4.35 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 4.14 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 4.35 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4095)]` | 9.48 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4096)]` | 9.81 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 4.88 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 4.91 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4095)]` | 5.40 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4096)]` | 5.53 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4095)]` | 1.67 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4096)]` | 1.66 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 15.92 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 15.92 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 9.32 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 9.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 6.63 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 6.97 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4095)]` | 3.68 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4096)]` | 3.73 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 10.30 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 10.63 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 5.30 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 5.33 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4095)]` | 3.79 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4096)]` | 3.82 (20%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ascending")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","integer",1000)]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",100)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","range",100)]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","range",1000)]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.60 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 2.17 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.72 (40%) :x: | 1.00 (1%)  |

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
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
Julia Version 0.6.0-dev.743
Commit 762cdf1 (2016-09-23 13:55 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15524.75390625 MB free)
Uptime: 1.0289328e7 sec
Load Avg:  1.01416015625  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17190692 s          0 s    3579575 s  1005227084 s         32 s
#2  3501 MHz   45389809 s          0 s    2243874 s  980628578 s          4 s
#3  3501 MHz   15974734 s          0 s    1964029 s  1010502099 s         21 s
#4  3501 MHz   13659426 s          0 s    1973938 s  1012786353 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.742
Commit e60961b (2016-09-23 11:05 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (15190.01171875 MB free)
Uptime: 1.0294025e7 sec
Load Avg:  1.0029296875  0.99755859375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   17254832 s          0 s    3587687 s  1005623068 s         32 s
#2  3501 MHz   45597138 s          0 s    2251400 s  980882946 s          4 s
#3  3501 MHz   16015696 s          0 s    1969265 s  1010924825 s         21 s
#4  3501 MHz   13785539 s          0 s    1984250 s  1013119137 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
