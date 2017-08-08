# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6cb586062ed9e44efc3cbfe9812e0287841bc004](https://github.com/JuliaLang/julia/commit/6cb586062ed9e44efc3cbfe9812e0287841bc004) vs [JuliaLang/julia@4fea2033758793c6ba980695fe252eeb69fa5761](https://github.com/JuliaLang/julia/commit/4fea2033758793c6ba980695fe252eeb69fa5761)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22826#issuecomment-320823922)

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
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 8.26 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 5.49 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 8.22 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 6.36 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 8.22 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 6.37 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.43 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.51 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 8.11 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.53 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 6.99 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 2.72 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.95 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.93 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","Array{Float32,2}")]` | 0.28 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Float64,3}")]` | 0.78 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","Array{Int32,2}")]` | 0.28 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 8.22 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 6.37 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 8.22 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 6.42 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.93 (50%)  | 0.70 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.46 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 8.09 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.48 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 2.70 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","Array{Float32,2}")]` | 0.29 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Float64,3}")]` | 0.80 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","Array{Int32,2}")]` | 0.29 (50%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.06 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.04 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.48 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.47 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.48 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.47 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.94 (50%)  | 0.70 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.48 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.89 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.41 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.40 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.00 (50%)  | 0.63 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.46 (50%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 0.89 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.41 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 0.39 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.78 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.02 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.97 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.76 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","Array{Float32,2}")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","negative argument","Float64")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","positive argument","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","positive argument","Float32")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","negative argument","Float64")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("abs(x) < 0.5","positive argument","Float64")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1286
Commit 6cb5860 (2017-08-08 01:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83587576 s          0 s   15061519 s  3671401468 s         86 s
       #2  3501 MHz  345119671 s          0 s    9493808 s  3424285305 s         13 s
       #3  3501 MHz   72771380 s          0 s    8382410 s  3698133228 s         73 s
       #4  3501 MHz   69488056 s          0 s    8570111 s  3701216520 s         17 s
       
  Memory: 31.383651733398438 GB (4550.41796875 MB free)
  Uptime: 3.7811014e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1283
Commit 4fea203 (2017-08-07 22:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83662834 s          0 s   15070582 s  3672003917 s         87 s
       #2  3501 MHz  345741964 s          0 s    9504708 s  3424340949 s         13 s
       #3  3501 MHz   72868099 s          0 s    8389468 s  3698718358 s         73 s
       #4  3501 MHz   69568622 s          0 s    8577367 s  3701817647 s         17 s
       
  Memory: 31.383651733398438 GB (4187.90234375 MB free)
  Uptime: 3.7817909e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
