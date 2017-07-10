# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3334724ba3289593d33b4771a07f2ac4271fb008](https://github.com/JuliaLang/julia/commit/3334724ba3289593d33b4771a07f2ac4271fb008)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3334724ba3289593d33b4771a07f2ac4271fb008#commitcomment-23003078)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-07-10 vs 2017-07-08

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
| `["array","cat",("catnd",5)]` | 0.71 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 0.62 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.75 (15%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["array","cat",("hvcat",5)]` | 0.74 (15%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["array","cat",("hvcat_setind",5)]` | 0.70 (15%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 1.67 (15%) :x: | 0.83 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.75 (15%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["array","convert",("Int","Complex{Float64}")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","sub2ind"]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.13 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.02 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.29 (50%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","1.0:0.00010001000100010001:2.0")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","1.0:1.0:100000.0")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","1:100000")]` | 0.14 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","Array{Float32,2}")]` | 0.34 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Float64,3}")]` | 0.76 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Int32,2}")]` | 0.34 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.41 (50%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.02 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Float32,2}")]` | 0.34 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Float64,3}")]` | 0.78 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Int32,2}")]` | 0.34 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.94 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.94 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.93 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.94 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.41 (50%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.94 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.85 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.93 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.90 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.92 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.94 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.84 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.95 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.30 (50%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","1.0:0.00010001000100010001:2.0")]` | 0.24 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1.0:1.0:100000.0")]` | 0.24 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1:100000")]` | 0.13 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","BitArray{2}")]` | 0.27 (50%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","reductions",("var","Float64")]` | 0.92 (15%)  | 1.50 (1%) :x: |
| `["array","reductions",("var","Int64")]` | 1.01 (15%)  | 1.44 (1%) :x: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.18 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.45 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 0.45 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",10)]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Month")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweek","Date")]` | 0.49 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","DateTime")]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofmonth","Date")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 0.48 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","read"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.96 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc","afoldl","Complex{Float64}"]` | 0.08 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","afoldl","Float64"]` | 0.05 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","afoldl","Int"]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","Int")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 0.70 (15%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["misc","repeat",(200,24,1)]` | 0.31 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["misc","splatting",(3,3,3)]` | 0.67 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","Array","Bool")]` | 0.15 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 0.25 (50%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.79 (15%) :white_check_mark: | 1.01 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 0.77 (15%) :white_check_mark: | 1.01 (1%)  |
| `["parallel","remotecall",("identity",4096)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",512)]` | 0.78 (15%) :white_check_mark: | 1.01 (1%)  |
| `["parallel","remotecall",("identity",64)]` | 0.78 (15%) :white_check_mark: | 1.01 (1%)  |
| `["problem","go","go_game"]` | 0.83 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["problem","simplex","simplex"]` | 1.00 (15%)  | 0.77 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.93 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 0.96 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 0.96 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.96 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.96 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 0.96 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.97 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.98 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.96 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 0.96 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.26 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.31 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.98 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 0.99 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.98 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.98 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 0.98 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.96 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.95 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.91 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","underflow","Float64")]` | 0.28 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","norm","Float64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 0.41 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float32")]` | 0.33 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float64")]` | 0.34 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","norm","Float32")]` | 0.33 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","norm","Float64")]` | 0.34 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float32")]` | 0.34 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float64")]` | 0.45 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","-")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 0.26 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 0.31 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","meteor_contest"]` | 0.96 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","nbody"]` | 1.00 (15%)  | 1.54 (1%) :x: |
| `["shootout","nbody_vec"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 2.08 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 2.06 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 1.28 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 0.53 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 0.99 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 1.01 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 0.99 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 1.00 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 0.99 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.00 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.98 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 0.98 (30%)  | 2.00 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.00 (30%)  | 2.00 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.04 (30%)  | 1.60 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.02 (30%)  | 1.60 (1%) :x: |
| `["sort","issorted",("forwards","descending")]` | 2.05 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","random")]` | 2.13 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 3.85 (30%) :x: | 1.67 (1%) :x: |
| `["sort","issorted",("reverse","descending")]` | 1.02 (30%)  | 1.67 (1%) :x: |
| `["sort","issorted",("reverse","ones")]` | 1.00 (30%)  | 1.67 (1%) :x: |
| `["sort","issorted",("reverse","random")]` | 4.09 (30%) :x: | 1.67 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.97 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.97 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 0.99 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 1.01 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 0.95 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 0.93 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.97 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 1.01 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 0.99 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 0.99 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.00 (30%)  | 1.22 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.00 (30%)  | 1.22 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 0.99 (30%)  | 2.00 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 0.99 (30%)  | 2.00 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 1.00 (30%)  | 1.80 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 1.00 (30%)  | 1.80 (1%) :x: |
| `["sparse","index",("spmat","integer",10)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",10)]` | 0.89 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 0.83 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.86 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 0.86 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.80 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",10)]` | 0.51 (30%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 0.20 (30%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.14 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spvec","integer",1000)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 0.86 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.03 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 1.03 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 1.03 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 1.01 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.09 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(600,400))]` | 1.05 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(600,600))]` | 1.01 (30%)  | 2.00 (1%) :x: |
| `["tuple","index",("sumelt","NTuple",3,Float64)]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","linear algebra",("matvec",(4,4),(4,))]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 0.09 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 0.11 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,))]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(8,))]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.876
Commit 3334724 (2017-07-10 02:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   74395320 s          0 s   13810932 s  3432499249 s         84 s
       #2  3501 MHz  311984231 s          0 s    8726544 s  3208178341 s         13 s
       #3  3501 MHz   66806153 s          0 s    7791215 s  3454663923 s         69 s
       #4  3501 MHz   63653452 s          0 s    7973618 s  3457617099 s         16 s
       
  Memory: 31.383651733398438 GB (2783.98828125 MB free)
  Uptime: 3.5309686e7 sec
  Load Avg:  1.01416015625  1.02099609375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
