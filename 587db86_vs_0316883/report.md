# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@587db864d01c5a3a9345ad5f13b64242349014d4](https://github.com/JuliaLang/julia/commit/587db864d01c5a3a9345ad5f13b64242349014d4) vs [JuliaLang/julia@0316883c2dabb22bf29e587a0004599e656776d3](https://github.com/JuliaLang/julia/commit/0316883c2dabb22bf29e587a0004599e656776d3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-271661524)

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
| `["array","cat",("catnd",5)]` | 1.17 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sum","3dsubarray")]` | 38.66 (50%) :x: | 573.29 (1%) :x: |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 7.92 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","100000:-1:1")]` | 95.26 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","1:100000")]` | 47.01 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","Array{Float32,2}")]` | 66.12 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","Array{Float64,3}")]` | 38.40 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","Array{Int32,2}")]` | 67.33 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 61.97 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 67.82 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 68.67 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 66.94 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 61.19 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 66.89 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","BitArray{2}")]` | 4.96 (50%) :x: | 3.00 (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 67.85 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 61.30 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 51.96 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 61.42 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 6.95 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 68.24 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 50.77 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 36.76 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 69.64 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 65.64 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 53.64 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 61.58 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 7.15 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 69.11 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 58.76 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000)")]` | 5.26 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 1.04 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 1.08 (50%)  | 1.06 (1%) :x: |
| `["array","index",("sumcartesian_view","1:100000")]` | 1.02 (50%)  | 1.07 (1%) :x: |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 1.03 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 1.15 (50%)  | 1.14 (1%) :x: |
| `["array","index",("sumcartesian_view","Array{Int32,2}")]` | 1.02 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.06 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.10 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.04 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.08 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.07 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.01 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 1.01 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 1.10 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.09 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.06 (50%)  | 1.18 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 1.08 (50%)  | 1.21 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.09 (50%)  | 1.22 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 1.07 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.07 (50%)  | 1.18 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.14 (50%)  | 1.14 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 1.09 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.10 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.07 (50%)  | 1.18 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 1.10 (50%)  | 1.21 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.08 (50%)  | 1.22 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 1.11 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.07 (50%)  | 1.18 (1%) :x: |
| `["array","index",("sumcartesian_view","linspace(1.0,2.0,10000)")]` | 1.06 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon_view","1.0:1.0:100000.0")]` | 3.04 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcolon_view","100000:-1:1")]` | 2.17 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcolon_view","1:100000")]` | 3.32 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcolon_view","linspace(1.0,2.0,10000)")]` | 2.12 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 67.99 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 66.84 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 69.19 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 66.44 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 60.38 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 7.95 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 68.71 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 50.75 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 36.85 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 66.26 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 7.22 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 68.17 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 58.64 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 4.47 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 4.54 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.09 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.08 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.08 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.98 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 4.42 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.07 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 4.39 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 3.45 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.11 (50%)  | 1.22 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 1.08 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.07 (50%)  | 1.18 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.13 (50%)  | 1.14 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 4.50 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.11 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 4.63 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 3.46 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.09 (50%)  | 1.22 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 1.08 (50%)  | 1.19 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.06 (50%)  | 1.18 (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 49.50 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 49.89 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 43.43 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 50.61 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 29.38 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 5.29 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 18.97 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 15.71 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 18.05 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 28.55 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 6.02 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 17.50 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumelt","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 18.69 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 4.42 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 4.48 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.46 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.46 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.45 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.46 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 4.45 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.45 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 4.42 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 3.49 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.77 (50%) :x: | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 1.45 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.44 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.50 (50%)  | 1.22 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 4.51 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.44 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 4.54 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 3.57 (50%) :x: | 1.40 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.84 (50%) :x: | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 1.46 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.46 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumrange_view","1.0:1.0:100000.0")]` | 3.14 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumrange_view","100000:-1:1")]` | 2.19 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumrange_view","1:100000")]` | 3.44 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumrange_view","linspace(1.0,2.0,10000)")]` | 2.10 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumvector_view","1.0:1.0:100000.0")]` | 1.41 (50%)  | 1.27 (1%) :x: |
| `["array","index",("sumvector_view","100000:-1:1")]` | 1.38 (50%)  | 1.27 (1%) :x: |
| `["array","index",("sumvector_view","1:100000")]` | 1.44 (50%)  | 1.29 (1%) :x: |
| `["array","index",("sumvector_view","linspace(1.0,2.0,10000)")]` | 1.40 (50%)  | 1.27 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 45.18 (15%) :x: | 8.43 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 36.58 (15%) :x: | 8.95 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",250)]` | 29.19 (15%) :x: | 8.80 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",500)]` | 28.39 (15%) :x: | 8.91 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",100)]` | 43.97 (15%) :x: | 8.43 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 36.39 (15%) :x: | 8.95 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",250)]` | 29.22 (15%) :x: | 8.80 (1%) :x: |
| `["array","subarray",("lucompletepivSub!",500)]` | 28.07 (15%) :x: | 8.91 (1%) :x: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 87.96 (15%) :x: | Inf (1%) :x: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 38.37 (15%) :x: | Inf (1%) :x: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 66.91 (15%) :x: | Inf (1%) :x: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 300.26 (15%) :x: | Inf (1%) :x: |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 254.27 (15%) :x: | 518593.96 (1%) :x: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 100.11 (15%) :x: | Inf (1%) :x: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 147.64 (15%) :x: | Inf (1%) :x: |
| `["dates","parse","Date"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.15 (15%) :x: | 1.01 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 168.27 (45%) :x: | 12.80 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 94.65 (45%) :x: | 12.23 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 165.14 (45%) :x: | 12.82 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 95.56 (45%) :x: | 12.32 (1%) :x: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",1024)]` | 3.38 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 5.91 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",1024)]` | 3.37 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 5.85 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 89.03 (45%) :x: | 6.90 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 46.83 (45%) :x: | 6.63 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 169.83 (45%) :x: | 12.82 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 96.70 (45%) :x: | 12.32 (1%) :x: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 187.02 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 203.46 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 185.94 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 226.45 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 172.55 (45%) :x: | 12.79 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 95.41 (45%) :x: | 12.21 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 127.13 (45%) :x: | 9.85 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 75.55 (45%) :x: | 9.42 (1%) :x: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 186.72 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 204.33 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 169.94 (45%) :x: | 12.82 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 95.63 (45%) :x: | 12.32 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 89.30 (45%) :x: | 6.90 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 56.54 (45%) :x: | 6.63 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 168.97 (45%) :x: | 12.82 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 95.78 (45%) :x: | 12.32 (1%) :x: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 185.85 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 225.82 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 185.22 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 211.25 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 177.44 (45%) :x: | 12.79 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 94.29 (45%) :x: | 12.21 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 128.13 (45%) :x: | 9.85 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 77.75 (45%) :x: | 9.42 (1%) :x: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 185.68 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 204.24 (45%) :x: | 25.00 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 170.95 (45%) :x: | 12.82 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 96.76 (45%) :x: | 12.32 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 74.43 (45%) :x: | 12.80 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 58.57 (45%) :x: | 12.23 (1%) :x: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",1024)]` | 3.08 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 4.58 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",1024)]` | 3.41 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 6.01 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 74.10 (45%) :x: | 12.80 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 58.15 (45%) :x: | 12.23 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 73.49 (45%) :x: | 12.82 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 58.15 (45%) :x: | 12.32 (1%) :x: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",1024)]` | 3.15 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 4.92 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 0.98 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",1024)]` | 3.15 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 4.87 (45%) :x: | 9.00 (1%) :x: |
| `["linalg","factorization",("eig","Matrix",256)]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 1.00 (45%)  | 1.01 (1%) :x: |
| `["linalg","factorization",("schur","Matrix",256)]` | 1.00 (45%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 1.00 (45%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.14 (45%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.11 (45%)  | 1.02 (1%) :x: |
| `["misc","parse","DateTime"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.22 (15%) :x: | 1.06 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.23 (15%) :x: | 1.09 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.21 (15%) :x: | 1.03 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.23 (15%) :x: | 1.07 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.23 (15%) :x: | 1.09 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.29 (15%) :x: | 1.06 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 58.73 (15%) :x: | 38025.27 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 37.70 (15%) :x: | 10.95 (1%) :x: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.39 (15%) :x: | 1.25 (1%) :x: |
| `["problem","monte carlo","euro_option_devec"]` | 1.07 (15%)  | 5.00 (1%) :x: |
| `["problem","monte carlo","euro_option_vec"]` | 20.89 (15%) :x: | 1002.72 (1%) :x: |
| `["problem","seismic",("seismic","Float32")]` | 10.86 (15%) :x: | 6.34 (1%) :x: |
| `["problem","seismic",("seismic","Float64")]` | 6.18 (15%) :x: | 3.67 (1%) :x: |
| `["shootout","nbody_vec"]` | 50.03 (15%) :x: | 104.61 (1%) :x: |
| `["simd",("sum_reduce","Float32",4096)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","random")]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",10)]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 0.56 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,10000))]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |

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
