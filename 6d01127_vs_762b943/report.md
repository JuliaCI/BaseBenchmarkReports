# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6d01127b89608628e6ad363b01f8f2518eabce57](https://github.com/JuliaLang/julia/commit/6d01127b89608628e6ad363b01f8f2518eabce57) vs [JuliaLang/julia@762b943d1d7b3adf3da37c1067b70e17d365b236](https://github.com/JuliaLang/julia/commit/762b943d1d7b3adf3da37c1067b70e17d365b236)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21067#issuecomment-287428073)

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
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["array","index","3d"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["array","index","4d"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["array","index","5d"]` | 1.62 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["array","index","7d"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:0.00010001000100010001:2.0")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:0.00010001000100010001:2.0")]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:0.00010001000100010001:2.0")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1.0:1.0:100000.0")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:0.00010001000100010001:2.0")]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:0.00010001000100010001:2.0")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:0.00010001000100010001:2.0")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:0.00010001000100010001:2.0")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:0.00010001000100010001:2.0")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:0.00010001000100010001:2.0")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:100000.0")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 2.33 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_mapreduce","Float64")]` | 4.97 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_reduce","Float64")]` | 5.06 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("var","Int64")]` | 4.14 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 2.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 2.21 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 2.02 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 19.42 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 6.80 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 11.57 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 12.57 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),1)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 2.03 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","day"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 3.25 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 3.62 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 3.32 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","month"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 3.34 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","year"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Month")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 1.85 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","conversion","DateTime -> Date"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["io","read","read"]` | 2.76 (15%) :x: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 5.89 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","BigInt")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 2.87 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int64")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int8")]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","BigFloat")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","BigInt")]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 16.67 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Complex{Float64}")]` | 2.94 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 21.24 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float64")]` | 2.97 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int64")]` | 2.97 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 17.27 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Bool")]` | 2.76 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Complex{Float64}")]` | 2.92 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float32")]` | 2.76 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float64")]` | 2.77 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int64")]` | 2.76 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int8")]` | 2.76 (50%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_devec"]` | 2.64 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float64}")]` | 2.80 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Int64}")]` | 3.36 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{UInt64}")]` | 2.31 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Int64")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","UInt64")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 2.80 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 2.97 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.10 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Float32")]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Int64")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","UInt64")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float32}")]` | 2.96 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 2.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 2.27 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float32}")]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 2.27 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Int64")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{Float64}")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Int64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","UInt64")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Float32")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Int64")]` | 2.19 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","UInt64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{Float32}")]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{Float64}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{UInt64}")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Float64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","UInt64")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Float32}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Float32")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Float64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Int64")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 1.62 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{UInt64}")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Int64}")]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{UInt64}")]` | 1.74 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{Float32}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Float32")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Float32}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 3.44 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 4.10 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{UInt64}")]` | 3.63 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float64")]` | 2.80 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Int64")]` | 2.66 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","UInt64")]` | 2.25 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 3.90 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 3.96 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 2.79 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float32")]` | 2.28 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Int64")]` | 2.28 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 2.49 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 3.63 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 3.80 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 2.76 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float32")]` | 2.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float64")]` | 2.97 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 2.41 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float32}")]` | 2.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 2.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 2.76 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float32")]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Int64")]` | 2.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{Float64}")]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{Int64}")]` | 2.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{UInt64}")]` | 2.31 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Float64")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Int64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","UInt64")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Float32}")]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Int64}")]` | 2.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Float32")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Int64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","UInt64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Float32}")]` | 2.66 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Float64}")]` | 2.64 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{UInt64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Float32")]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float32}")]` | 2.25 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 2.49 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 2.27 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Float32")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Int64")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 2.28 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Int64}")]` | 2.80 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{UInt64}")]` | 2.31 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Int64")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","UInt64")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 2.41 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 2.25 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float32")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Int64")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float32}")]` | 2.97 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float64}")]` | 2.66 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 2.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float32}")]` | 2.20 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.09 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float32")]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Int64")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Float64}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Int64}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{UInt64}")]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Float64")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","UInt64")]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Float32}")]` | 1.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Int64}")]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Float32")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Int64")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Float32}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Float64}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{UInt64}")]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","UInt64")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float32}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Float32")]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Float64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Int64")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 1.62 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{UInt64}")]` | 1.74 (40%) :x: | 1.00 (1%)  |
| `["shootout","spectralnorm"]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 20.72 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 21.36 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 10.58 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 10.68 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",1000)]` | 1.32 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.170
Commit 6d01127 (2017-03-17 17:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8018.83984375 MB free)
Uptime: 2.5424997e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53338010 s          0 s    8254448 s  2475486135 s         77 s
#2  3501 MHz  193651004 s          0 s    8867603 s  2335848513 s         26 s
#3  3501 MHz   44336238 s          0 s    5180794 s  2491835827 s         41 s
#4  3501 MHz   40070006 s          0 s    5134802 s  2496375005 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.167
Commit 762b943 (2017-03-17 17:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7801.0859375 MB free)
Uptime: 2.5430573e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53433049 s          0 s    8264372 s  2475936756 s         77 s
#2  3501 MHz  194151574 s          0 s    8876542 s  2335895958 s         26 s
#3  3501 MHz   44420072 s          0 s    5189004 s  2492300675 s         41 s
#4  3501 MHz   40151302 s          0 s    5143163 s  2496842465 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
