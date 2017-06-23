# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@bdd5477d13aa8a71823ad782e8b35fec28b1227a](https://github.com/JuliaLang/julia/commit/bdd5477d13aa8a71823ad782e8b35fec28b1227a) vs [JuliaLang/julia@5176ded01dbd60ae013abdac4b189f075e6ae82b](https://github.com/JuliaLang/julia/commit/5176ded01dbd60ae013abdac4b189f075e6ae82b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22481#issuecomment-310731715)

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
| `["array","cat",("catnd",5)]` | 7.89 (15%) :x: | 1.15 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 12.02 (15%) :x: | 1.18 (1%) :x: |
| `["array","growth",("push_multiple!",2048)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","index","7d"]` | 1.58 (15%) :x: | Inf (1%) :x: |
| `["array","index",("sum","3darray")]` | 52.49 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.16 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.34 (50%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BitArray{2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 2250.90 (50%) :x: | 6.00 (1%) :x: |
| `["array","index",("sumcolon_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 591.61 (50%) :x: | 2.25 (1%) :x: |
| `["array","index",("sumcolon_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.02 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 2747.17 (50%) :x: | 6.00 (1%) :x: |
| `["array","index",("sumcolon_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 678.56 (50%) :x: | 2.25 (1%) :x: |
| `["array","index",("sumeach","Array{Float64,3}")]` | 6.79 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","BitArray{2}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Float64,3}")]` | 181.24 (50%) :x: | 2.38 (1%) :x: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.84 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumelt","100000:-1:1")]` | 7.00 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BitArray{2}")]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.63 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.10 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.15 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.10 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.15 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","Array{Float64,3}")]` | 175.14 (50%) :x: | 2.38 (1%) :x: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.84 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.02 (50%) :x: | 1.44 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 15.08 (50%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 14.64 (50%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 15.11 (50%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 15.25 (50%) :x: | 1.07 (1%) :x: |
| `["array","index",("sumrange_view","Array{Float32,2}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1797.64 (50%) :x: | 4.75 (1%) :x: |
| `["array","index",("sumrange_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 610.15 (50%) :x: | 2.25 (1%) :x: |
| `["array","index",("sumrange_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1998.51 (50%) :x: | 4.75 (1%) :x: |
| `["array","index",("sumrange_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 694.12 (50%) :x: | 2.25 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 224.98 (50%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 227.86 (50%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 269.10 (50%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 265.73 (50%) :x: | 2.00 (1%) :x: |
| `["array","reductions",("maxabs","Float64")]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("var","Int64")]` | 0.99 (15%)  | 0.89 (1%) :white_check_mark: |
| `["array","reverse","rev_load_fast!"]` | 2.59 (15%) :x: | 1.00 (1%)  |
| `["array","reverse","rev_load_slow!"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",3)]` | 8.22 (15%) :x: | 1.23 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 8.10 (15%) :x: | 1.23 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 8.17 (15%) :x: | 1.23 (1%) :x: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 8.22 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 3.79 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 4.46 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 5.30 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 4.98 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 7.91 (15%) :x: | Inf (1%) :x: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 3.41 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 8.93 (15%) :x: | Inf (1%) :x: |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 4.39 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 11.15 (15%) :x: | Inf (1%) :x: |
| `["broadcast","sparse",((1000,1000),1)]` | 1.81 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",3)]` | 1.75 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","day"]` | 4.16 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","hour"]` | 5.85 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 4.78 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 5.89 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","month"]` | 4.88 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 6.02 (15%) :x: | 1.00 (1%)  |
| `["dates","accessor","year"]` | 5.31 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Day")]` | 1.99 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Month")]` | 2.87 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 2.75 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Day")]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Hour")]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Millisecond")]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Minute")]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 3.51 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Second")]` | 1.79 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 3.63 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 2.62 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 2.45 (15%) :x: | 1.00 (1%)  |
| `["dates","conversion","DateTime -> Date"]` | 5.96 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 2.28 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 2.60 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.95 (15%)  | 1.02 (1%) :x: |
| `["dates","parse",("Date","ISODateFormat")]` | 2.32 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","DateFormat")]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 2.62 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","Date")]` | 3.06 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 4.44 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweekofmonth","Date")]` | 3.76 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweekofmonth","DateTime")]` | 3.83 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofyear","Date")]` | 3.07 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofyear","DateTime")]` | 3.18 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("daysofweekinmonth","Date")]` | 2.99 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("daysofweekinmonth","DateTime")]` | 3.20 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofmonth","Date")]` | 3.90 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofmonth","DateTime")]` | 3.87 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 2.90 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","DateTime")]` | 4.31 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("isleapyear","Date")]` | 4.18 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("isleapyear","DateTime")]` | 4.22 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofmonth","Date")]` | 3.09 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofmonth","DateTime")]` | 3.10 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 2.94 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 4.18 (25%) :x: | 1.00 (1%)  |
| `["dates","string","Date"]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",1024)]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 2.11 (45%) :x: | 1.00 (1%)  |
| `["micro","mandel"]` | 2.01 (15%) :x: | 1.01 (1%)  |
| `["micro","parseint"]` | 2.03 (15%) :x: | 1.00 (1%)  |
| `["misc","afoldl","Complex{Float64}"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["misc","afoldl","Float64"]` | 1.18 (15%) :x: | 1.08 (1%) :x: |
| `["misc","afoldl","Int"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 2.64 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","Int"]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.33 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 0.31 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Complex{Float64}")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Complex{Float64}")]` | 2.24 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Complex{Float64}")]` | 5.58 (50%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","NullableArray","Complex{Float64}")]` | 5.73 (50%) :x: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.23 (15%) :x: | 1.09 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.95 (15%)  | 1.01 (1%) :x: |
| `["problem","raytrace","raytrace"]` | 1.39 (15%) :x: | 0.74 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float32}")]` | 1.79 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float64}")]` | 3.69 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Int64}")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 3.69 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float64}")]` | 3.70 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float32}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 4.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 4.31 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 4.47 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 2.89 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 4.29 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 4.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 2.89 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 2.88 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 4.45 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float32}")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float64}")]` | 1.93 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Float64")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Float32}")]` | 2.11 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Float64}")]` | 1.99 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Int64}")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{UInt64}")]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Float32")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Int64")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","UInt64")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Float64}")]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Float64")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Int64")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","UInt64")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Float64}")]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Int64")]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","UInt64")]` | 1.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Complex{Float32}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Complex{Int64}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{Float32}")]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{Int64}")]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{UInt64}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Float32}")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Float64}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{Int64}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{UInt64}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 1.82 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 3.23 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float64")]` | 4.45 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Int64")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","UInt64")]` | 2.14 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 3.23 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 3.69 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 3.24 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 2.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float32")]` | 4.29 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Int64")]` | 4.45 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 3.36 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 3.24 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 3.69 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 3.23 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float32")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float64")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 2.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 3.23 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 3.69 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float32")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.88 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Int64")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{Float64}")]` | 4.30 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{Int64}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{UInt64}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Float32}")]` | 4.45 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Int64}")]` | 4.27 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 2.89 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Float32}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Float64}")]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{UInt64}")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float32}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 3.36 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float32}")]` | 1.83 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Int64}")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float64}")]` | 4.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 2.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float32}")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float64}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 4.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 4.29 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 4.47 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 3.70 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 4.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 2.87 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Float64}")]` | 3.69 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Int64}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Float32}")]` | 3.37 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Int64}")]` | 3.69 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{UInt64}")]` | 2.63 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Float32}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Float64}")]` | 3.37 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{UInt64}")]` | 4.32 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float32}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float64}")]` | 2.98 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Int64}")]` | 4.44 (50%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float32}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 3.69 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 3.69 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 3.69 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Float32}")]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Float64}")]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Float32}")]` | 1.83 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Float64}")]` | 4.32 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Int64}")]` | 4.32 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 4.32 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Float32}")]` | 1.79 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Float64}")]` | 4.32 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Int64}")]` | 4.32 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{UInt64}")]` | 4.32 (40%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","UInt64","-")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Float32}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Int64}")]` | 1.83 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{UInt64}")]` | 2.18 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("iseven","UInt64")]` | 1.79 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 3.01 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 2.98 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float32")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 2.17 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 3.05 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 3.36 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Float32")]` | 2.17 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Float64")]` | 2.17 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float32}")]` | 2.42 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float64}")]` | 2.42 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float32")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float64")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","UInt64")]` | 1.99 (25%) :x: | 1.00 (1%)  |
| `["shootout","mandelbrot"]` | 2.17 (15%) :x: | 1.05 (1%) :x: |
| `["shootout","nbody_vec"]` | 2.14 (15%) :x: | 1.00 (1%)  |
| `["shootout","spectralnorm"]` | 1.09 (15%)  | 0.22 (1%) :white_check_mark: |
| `["simd",("conditional_loop!","Float32",4095)]` | 38.18 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float32",4096)]` | 38.33 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4095)]` | 31.71 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Float64",4096)]` | 31.40 (20%) :x: | Inf (1%) :x: |
| `["simd",("conditional_loop!","Int32",4095)]` | 133.88 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 134.08 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 58.73 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 59.36 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4095)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 2.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ones")]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.97 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 2.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 1.74 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ones")]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.97 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 1.94 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 2.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.96 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 2.42 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.94 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.97 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","descending")]` | 2.29 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 2.09 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","random")]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 2.32 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 2.21 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 2.04 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","random")]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 2.23 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 2.38 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 2.12 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","random")]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 2.35 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 2.23 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 2.08 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","random")]` | 1.57 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 2.48 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 2.60 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ones")]` | 2.40 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","random")]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 2.65 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","descending")]` | 2.65 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","ones")]` | 2.39 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm reverse","random")]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 2.61 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 2.77 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 2.44 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 2.70 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 2.71 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 2.43 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","random")]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.86 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 2.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 1.60 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",1000)]` | 2.30 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",10000)]` | 1.63 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",100000)]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","linear algebra",("matmat",(2,2),(2,2))]` | 3.28 (15%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matvec",(2,2),(2,))]` | 4.30 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(16,))]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(16,16))]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,2))]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(4,))]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(4,4))]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(8,))]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(8,8))]` | 1.36 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.689
Commit bdd5477 (2017-06-23 17:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   70943683 s          0 s   13250136 s  3295156459 s         82 s
       #2  3501 MHz  297421742 s          0 s    8421964 s  3081344669 s         12 s
       #3  3501 MHz   64240453 s          0 s    7514812 s  3315789512 s         68 s
       #4  3501 MHz   61174753 s          0 s    7688563 s  3318667308 s         15 s
       
  Memory: 31.383651733398438 GB (2503.2578125 MB free)
  Uptime: 3.3891915e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.686
Commit 5176ded (2017-06-23 17:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71017871 s          0 s   13258802 s  3295598366 s         83 s
       #2  3501 MHz  297910267 s          0 s    8429779 s  3081374686 s         12 s
       #3  3501 MHz   64319746 s          0 s    7522129 s  3316229131 s         68 s
       #4  3501 MHz   61250066 s          0 s    7696048 s  3319110890 s         15 s
       
  Memory: 31.383651733398438 GB (2364.54296875 MB free)
  Uptime: 3.3897183e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
