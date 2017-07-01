# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ae3f0b9a769be587b4f417aea6da67a5be844914](https://github.com/JuliaLang/julia/commit/ae3f0b9a769be587b4f417aea6da67a5be844914) vs [JuliaLang/julia@b5a61db1d75f26202bf8449e47bbf5aad5342529](https://github.com/JuliaLang/julia/commit/b5a61db1d75f26202bf8449e47bbf5aad5342529)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22210#issuecomment-312423053)

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
| `["array","cat",("catnd",5)]` | 0.74 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 0.62 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.78 (15%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["array","cat",("hvcat",5)]` | 0.74 (15%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["array","cat",("hvcat_setind",5)]` | 0.71 (15%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 1.65 (15%) :x: | 0.83 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.73 (15%) :white_check_mark: | 0.82 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","Array{Float64,1}")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","sub2ind"]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.16 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
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
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.13 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.08 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.12 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.05 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.31 (50%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","1.0:0.00010001000100010001:2.0")]` | 0.25 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","1.0:1.0:100000.0")]` | 0.25 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","1:100000")]` | 0.16 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","Array{Float32,2}")]` | 0.34 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Float64,3}")]` | 0.74 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Int32,2}")]` | 0.34 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.01 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.38 (50%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
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
| `["array","index",("sumlinear_view","Array{Float64,3}")]` | 0.66 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Int32,2}")]` | 0.34 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.38 (50%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.79 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.93 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.91 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.97 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.85 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.96 (50%)  | 0.86 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 0.75 (50%)  | 0.91 (1%) :white_check_mark: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.31 (50%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","1.0:0.00010001000100010001:2.0")]` | 0.26 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1.0:1.0:100000.0")]` | 0.25 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1:100000")]` | 0.15 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","BitArray{2}")]` | 0.23 (50%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","reductions",("var","Float64")]` | 1.03 (15%)  | 1.50 (1%) :x: |
| `["array","reductions",("var","Int64")]` | 1.01 (15%)  | 1.44 (1%) :x: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.16 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.54 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",10)]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweek","Date")]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","DateTime")]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofmonth","Date")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","read"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.96 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc","afoldl","Complex{Float64}"]` | 0.11 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","afoldl","Float64"]` | 0.06 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","afoldl","Int"]` | 0.07 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","Int")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 0.01 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 0.72 (15%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["misc","repeat",(200,24,1)]` | 0.32 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["misc","splatting",(3,3,3)]` | 0.68 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","Array","Bool")]` | 0.17 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Bool")]` | 0.25 (50%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.76 (15%) :white_check_mark: | 1.01 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 0.82 (15%) :white_check_mark: | 1.01 (1%)  |
| `["parallel","remotecall",("identity",4096)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",512)]` | 0.78 (15%) :white_check_mark: | 1.01 (1%)  |
| `["problem","go","go_game"]` | 0.85 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["problem","simplex","simplex"]` | 1.00 (15%)  | 0.77 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.95 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.00 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 0.99 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 0.98 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 0.97 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 1.03 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.93 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.08 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 0.98 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 0.91 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.26 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.29 (50%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.94 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 1.00 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.97 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.92 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 0.97 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.97 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","norm","Float32")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","norm","Float64")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float32")]` | 0.34 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float64")]` | 0.30 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","norm","Float32")]` | 0.37 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","norm","Float64")]` | 0.38 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float32")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float64")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","-")]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","in"]` | 0.32 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 0.32 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","meteor_contest"]` | 0.96 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","nbody"]` | 0.96 (15%)  | 1.54 (1%) :x: |
| `["shootout","nbody_vec"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 2.34 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 2.10 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.02 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 0.98 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 0.94 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 0.98 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 1.03 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 0.94 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.00 (30%)  | 2.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.00 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.98 (30%)  | 1.29 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 0.98 (30%)  | 2.00 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.01 (30%)  | 2.00 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.04 (30%)  | 1.60 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.02 (30%)  | 1.60 (1%) :x: |
| `["sort","issorted",("forwards","descending")]` | 1.68 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","random")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 3.48 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","random")]` | 3.41 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.98 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 1.00 (30%)  | 1.33 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 0.92 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 0.92 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.96 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 1.02 (30%)  | 2.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 0.98 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 0.98 (30%)  | 1.29 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 0.99 (30%)  | 1.22 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 0.99 (30%)  | 1.22 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 0.99 (30%)  | 2.00 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 0.99 (30%)  | 2.00 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 1.00 (30%)  | 1.80 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 0.99 (30%)  | 1.80 (1%) :x: |
| `["sparse","index",("spmat","integer",10)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","logical",100)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",10)]` | 0.87 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 0.84 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.91 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 0.92 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.82 (30%)  | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",10)]` | 0.54 (30%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 0.25 (30%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.14 (30%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spvec","integer",1000)]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 0.71 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.66 (30%) :white_check_mark: | 2.00 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 1.01 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 1.03 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 0.79 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.99 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(600,400))]` | 1.02 (30%)  | 2.00 (1%) :x: |
| `["sparse","transpose",("transpose!",(600,600))]` | 1.02 (30%)  | 2.00 (1%) :x: |
| `["tuple","index",("sumelt","NTuple",3,Float64)]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",3,Float64)]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","linear algebra",("matvec",(4,4),(4,))]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,2))]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 0.09 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 0.11 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,))]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(8,))]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.817
Commit ae3f0b9 (2017-07-01 09:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71478583 s          0 s   10993084 s  3365589343 s        100 s
       #2  3501 MHz  282255326 s          0 s   12129746 s  3154791036 s         39 s
       #3  3501 MHz   61405967 s          0 s    7140205 s  3385353928 s         53 s
       #4  3501 MHz   56836260 s          0 s    7054518 s  3390344480 s         19 s
       
  Memory: 31.383651733398438 GB (3266.2578125 MB free)
  Uptime: 3.4554611e7 sec
  Load Avg:  1.07275390625  1.03564453125  1.04931640625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.810
Commit b5a61db (2017-07-01 00:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71553844 s          0 s   11002110 s  3366023569 s        100 s
       #2  3501 MHz  282735199 s          0 s   12137758 s  3154823016 s         39 s
       #3  3501 MHz   61486311 s          0 s    7147555 s  3385786079 s         53 s
       #4  3501 MHz   56916430 s          0 s    7061622 s  3390777245 s         19 s
       
  Memory: 31.383651733398438 GB (3235.73046875 MB free)
  Uptime: 3.4559817e7 sec
  Load Avg:  1.1630859375  1.0478515625  1.05615234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
