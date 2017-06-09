# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@60d0ad2adf82c22b264723c6078f77aa269ab792](https://github.com/JuliaLang/julia/commit/60d0ad2adf82c22b264723c6078f77aa269ab792) vs [JuliaLang/julia@f541d29b9110caf4c58be538beb0e0d972d4f1ef](https://github.com/JuliaLang/julia/commit/f541d29b9110caf4c58be538beb0e0d972d4f1ef)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21888#issuecomment-307472399)

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
| `["array","bool","boolarray_bool_load!"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",8)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array","index","3d"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["array","index","4d"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","index","5d"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sum","3dsubarray")]` | 12.11 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","Array{Float32,2}")]` | 8.28 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","Array{Float64,3}")]` | 6.93 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","Array{Int32,2}")]` | 7.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 8.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 7.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 8.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 7.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 8.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 7.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 7.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 7.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 7.39 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 7.17 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 8.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.47 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 6.88 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 7.16 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 6.85 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 6.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 6.70 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 6.90 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:0.00010001000100010001:2.0")]` | 5.93 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 5.91 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 55784.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1:100000")]` | 155109.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","1:100000")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 8.28 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 7.74 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 8.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 7.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 7.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 8.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.67 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 5.99 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 6.85 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 6.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:0.00010001000100010001:2.0")]` | 5.91 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 5.94 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","100000:-1:1")]` | 55318.19 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 160612.68 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 10.41 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 20.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 12.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 12.34 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 12.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 12.34 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 9.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 7.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 10.87 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 7.93 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 2.48 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 8.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.42 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 7.20 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 9.96 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 7.85 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 10.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 7.72 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 8.03 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.09 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:0.00010001000100010001:2.0")]` | 5.90 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 5.94 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","100000:-1:1")]` | 51195.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 160360.90 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:0.00010001000100010001:2.0")]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","100000:-1:1")]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1:100000")]` | 3.04 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 4.36 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 4.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 4.31 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 4.23 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 4.37 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 4.36 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 2.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 2.34 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 4.38 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 3.28 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 2.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 3.31 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","1.0:0.00010001000100010001:2.0")]` | 2.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","1.0:1.0:100000.0")]` | 2.69 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","100000:-1:1")]` | 2.69 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","1:100000")]` | 2.70 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 3.34 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 3.33 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 3.33 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 3.34 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 3.33 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 3.29 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.01 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 3.29 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 3.27 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.00 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 3.28 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 3.31 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 3.28 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1.0:0.00010001000100010001:2.0")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1.0:1.0:100000.0")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1:100000")]` | 2.03 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_fast!"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_slow!"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 2.38 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 2.90 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 2.24 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"tup_tup")]` | 2.63 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 3.30 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 2.31 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 3.46 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 3.68 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 2.12 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"tup_tup")]` | 3.11 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",10)]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 2.01 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Month")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 3.81 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 4.68 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 3.79 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 4.73 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 2.57 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.99 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 2.56 (15%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","Date")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 1.37 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["dates","string","Date"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 1.89 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 1.86 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 1.66 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 1.91 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 1.71 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 1.70 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 2.22 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 3.26 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 4.63 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 3.10 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 4.23 (45%) :x: | 1.00 (1%)  |
| `["micro","mandel"]` | 3.16 (15%) :x: | 1.00 (1%)  |
| `["micro","parseint"]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["misc","afoldl","Float64"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 4.62 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 1.84 (15%) :x: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.66 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{BigInt}(1)")]` | 1.65 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigFloat}()")]` | 1.83 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigFloat}()")]` | 1.98 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 1.98 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigInt}()")]` | 1.99 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigInt}(1)")]` | 1.99 (60%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_all","NullableArray")]` | 6.20 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 4.35 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 5.97 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Complex{Float64}")]` | 5.50 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 4.61 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 5.45 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 7.34 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 5.72 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Complex{Float64}")]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Bool")]` | 8.71 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Complex{Float64}")]` | 12.36 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float32")]` | 8.23 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Float64")]` | 11.96 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int64")]` | 12.34 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","NullableArray","Int8")]` | 8.76 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Complex{Float64}")]` | 9.80 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int64")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Complex{Float64}")]` | 15.99 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float32")]` | 3.76 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Float64")]` | 5.51 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int64")]` | 8.48 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Int8")]` | 3.44 (50%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float64}")]` | 3.25 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 3.76 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 2.80 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float64}")]` | 2.99 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 3.48 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Float32")]` | 3.90 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Float64")]` | 3.95 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Int64")]` | 3.31 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","UInt64")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 2.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 3.49 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Int64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 3.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 3.49 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Int64")]` | 3.79 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","UInt64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{Float64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 3.78 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Float64}")]` | 3.96 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{Float64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{Int64}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{UInt64}")]` | 3.79 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Float64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 3.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{UInt64}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float32}")]` | 1.53 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","UInt64")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Complex{Float64}")]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 2.05 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Complex{Float64}")]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Complex{Int64}")]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Complex{UInt64}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{Float64}")]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{Int64}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{UInt64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Float64}")]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Int64}")]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{UInt64}")]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 2.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float64")]` | 2.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 3.25 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 2.98 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float32")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float64")]` | 2.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Int64")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 2.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 2.98 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 2.65 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float64")]` | 3.31 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Int64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 3.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 2.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 2.98 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Int64")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","UInt64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{Float64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Float32}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Float64}")]` | 3.33 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Int64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 2.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Float64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Int64}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{UInt64}")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 2.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 3.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{UInt64}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 2.80 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 3.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 3.25 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float64}")]` | 3.49 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 2.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float32")]` | 3.30 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float64")]` | 3.96 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Int64")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","UInt64")]` | 2.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float64}")]` | 2.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 3.49 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Int64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 3.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 2.99 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 3.49 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 2.29 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Int64")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","UInt64")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Float64}")]` | 2.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Float32}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Float64}")]` | 3.31 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Int64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{UInt64}")]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Float64}")]` | 2.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Int64}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{UInt64}")]` | 3.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float64}")]` | 2.54 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Int64}")]` | 2.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{UInt64}")]` | 3.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 2.98 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 2.98 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 2.98 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Float64}")]` | 2.65 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Float64}")]` | 3.49 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Int64}")]` | 3.49 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 3.49 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Float64}")]` | 2.99 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Int64}")]` | 3.49 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{UInt64}")]` | 3.49 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float64")]` | 1.43 (40%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","Int64","+")]` | 1.86 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","Int64","-")]` | 1.87 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","UInt64","+")]` | 2.02 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","UInt64","-")]` | 2.03 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","+")]` | 2.15 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","-")]` | 2.08 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","UInt64","+")]` | 2.22 (25%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","UInt64","-")]` | 2.23 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{BigFloat}")]` | 1.45 (40%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 1.66 (40%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 2.82 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 2.84 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ones")]` | 2.64 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 3.54 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ones")]` | 2.44 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ones")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ones")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.90 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 2.28 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",10)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",10)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",100)]` | 1.89 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.79 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",100)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",1000)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",1000)]` | 2.65 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",10000)]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",100000)]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(600,600))]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(4,4),(4,4))]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,))]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,4))]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","intfuncs"]`
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
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.491
Commit 60d0ad2 (2017-06-06 12:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68664372 s          0 s   10548098 s  3182379053 s         92 s
       #2  3501 MHz  269156299 s          0 s   11566762 s  2981944944 s         38 s
       #3  3501 MHz   58956917 s          0 s    6846024 s  3201320476 s         49 s
       #4  3501 MHz   54463435 s          0 s    6783358 s  3206184004 s         17 s
       
  Memory: 31.383651733398438 GB (2851.8125 MB free)
  Uptime: 3.2686065e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.515
Commit f541d29 (2017-06-09 18:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68761490 s          0 s   10558108 s  3182805441 s         92 s
       #2  3501 MHz  269634642 s          0 s   11575848 s  2981992478 s         38 s
       #3  3501 MHz   59045049 s          0 s    6854598 s  3201758606 s         49 s
       #4  3501 MHz   54546326 s          0 s    6791862 s  3206627570 s         17 s
       
  Memory: 31.383651733398438 GB (2818.09375 MB free)
  Uptime: 3.269142e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
