# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ddba7015007e43d095fbbeca6cfad1dbbb8ed038](https://github.com/JuliaLang/julia/commit/ddba7015007e43d095fbbeca6cfad1dbbb8ed038) vs [JuliaLang/julia@fe27001391a0cb07dd6a08034c943ad0ff38cb80](https://github.com/JuliaLang/julia/commit/fe27001391a0cb07dd6a08034c943ad0ff38cb80)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22594#issuecomment-324468133)

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
| `["array","cat",("catnd",500)]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.92 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sum","3darray")]` | 8.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 7.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","Array{Int32,2}")]` | 4.49 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 8.02 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 4.20 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 7.75 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 4.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 7.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 4.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 7.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 5.78 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 4.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.49 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 4.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","Array{Int32,2}")]` | 3.95 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 3.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 3.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 7.12 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 7.82 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 4.82 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 8.20 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 4.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 5.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.86 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 4.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","Array{Int32,2}")]` | 3.96 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","Array{Int32,2}")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 3.95 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 3.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 6.87 (50%) :x: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_mapreduce","Int64")]` | 3.71 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_reduce","Int64")]` | 3.55 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("mean","Float64")]` | 8.28 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("sum","Float64")]` | 8.79 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("sumabs","Float64")]` | 8.35 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("sumabs","Int64")]` | 3.43 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("sumabs2","Float64")]` | 10.91 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("sumabs2","Int64")]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("var","Float64")]` | 6.69 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("var","Int64")]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_fast!"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 3.12 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 3.46 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 1.59 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 2.33 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.68 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 2.08 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 2.08 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 1.65 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 1.50 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.15 (45%) :x: | 1.00 (1%)  |
| `["linalg","blas","axpy!"]` | 2.14 (40%) :x: | 1.00 (1%)  |
| `["linalg","blas","scal!"]` | 2.00 (40%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float32")]` | 2.20 (15%) :x: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float64")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.01 (25%)  | 1.02 (1%) :x: |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand!","MersenneTwister","Float32")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("small","positive argument","Float32")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","UInt64","-")]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4095)]` | 9.43 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4096)]` | 9.59 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4095)]` | 4.67 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4096)]` | 4.73 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4095)]` | 7.94 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4096)]` | 8.17 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4095)]` | 1.43 (20%) :x: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4096)]` | 1.46 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 7.18 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 6.97 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 2.99 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 3.64 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 22.79 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 27.92 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 13.35 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 13.85 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int32",4095)]` | 7.59 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Int32",4096)]` | 7.91 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 7.26 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 7.27 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 7.95 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 8.10 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 2.63 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 2.72 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 2.52 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 2.30 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 5.95 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 6.05 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 5.71 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 5.92 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4095)]` | 13.43 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4096)]` | 14.07 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 10.75 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 10.97 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4095)]` | 8.02 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4096)]` | 8.76 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4095)]` | 2.58 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4096)]` | 2.56 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 11.72 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 10.60 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 8.74 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 9.46 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 7.13 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 8.51 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4095)]` | 4.58 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4096)]` | 4.55 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 13.60 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 14.18 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 10.20 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 10.49 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4095)]` | 4.62 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4096)]` | 4.71 (20%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 1.48 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 1.48 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 1.47 (40%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 5.86 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 1.23 (15%) :x: | 1.00 (1%)  |

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
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
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
Julia Version 0.7.0-DEV.1468
Commit ddba701 (2017-08-23 20:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82557190 s          0 s   12638216 s  3813900841 s        151 s
       #2  3501 MHz  332779579 s          0 s   13800036 s  3564117741 s         51 s
       #3  3501 MHz   70070688 s          0 s    7993370 s  3837909321 s         71 s
       #4  3501 MHz   65404431 s          0 s    7913692 s  3843031287 s         24 s
       
  Memory: 31.383651733398438 GB (3113.859375 MB free)
  Uptime: 3.9177006e7 sec
  Load Avg:  1.0830078125  1.03125  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1466
Commit fe27001 (2017-08-23 20:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82635403 s          0 s   12648246 s  3814524825 s        151 s
       #2  3501 MHz  333432620 s          0 s   13811705 s  3564167348 s         51 s
       #3  3501 MHz   70150250 s          0 s    8001260 s  3838536057 s         71 s
       #4  3501 MHz   65503066 s          0 s    7921364 s  3843639517 s         24 s
       
  Memory: 31.383651733398438 GB (3111.640625 MB free)
  Uptime: 3.9184156e7 sec
  Load Avg:  1.076171875  1.03076171875  1.05029296875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
