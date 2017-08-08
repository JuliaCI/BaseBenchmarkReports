# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@af70f66d98e3bf677c710e7865fbf654515db46f](https://github.com/JuliaLang/julia/commit/af70f66d98e3bf677c710e7865fbf654515db46f) vs [JuliaLang/julia@66a505d619da6037ca45d2b5e5d13ecd203b40fe](https://github.com/JuliaLang/julia/commit/66a505d619da6037ca45d2b5e5d13ecd203b40fe)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23169#issuecomment-320796809)

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
| `["array","cat",("catnd",5)]` | 1.27 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 1.07 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.34 (15%) :x: | 1.21 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 1.38 (15%) :x: | 1.29 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 1.53 (15%) :x: | 1.29 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.10 (15%)  | 1.20 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.43 (15%) :x: | 1.21 (1%) :x: |
| `["array","convert",("Int","Complex{Float64}")]` | 2.37 (15%) :x: | 1.00 (1%)  |
| `["array","index","sub2ind"]` | 208278.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sum","3dsubarray")]` | 1.05 (50%)  | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 76.99 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 10.86 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","Array{Int32,2}")]` | 85.33 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 79.66 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 91.56 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 76.04 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 85.89 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 76.20 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 86.00 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 76.62 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 60.95 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 12.41 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 9.76 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 76.80 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 12.63 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 11.81 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 85.92 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 92.32 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 21.53 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 13.42 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 85.50 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 21.76 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 3.05 (50%) :x: | 1.08 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 1.51 (50%) :x: | 1.17 (1%) :x: |
| `["array","index",("sumcolon","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 1.54 (50%) :x: | 1.17 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 76.05 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 86.08 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 76.65 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 86.55 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 2.34 (50%) :x: | 1.10 (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 16.28 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 60.75 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 15.53 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 76.06 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 12.65 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 11.91 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 20.48 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 93.08 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 15.15 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 86.58 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 22.30 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 2.35 (50%) :x: | 1.10 (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 16.26 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 15.56 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 20.55 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 15.70 (50%) :x: | Inf (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.23 (50%)  | 1.10 (1%) :x: |
| `["array","index",("sumrange","Array{Float32,2}")]` | 1.02 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 1.02 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.03 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.02 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.26 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.23 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 3.20 (50%) :x: | 1.08 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.02 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.03 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.04 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.01 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.23 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.03 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumvector","100000:-1:1")]` | 1.09 (50%)  | 1.13 (1%) :x: |
| `["array","index",("sumvector","1:100000")]` | 1.34 (50%)  | 1.13 (1%) :x: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 1.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","BitArray{2}")]` | 4.04 (50%) :x: | 1.12 (1%) :x: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.12 (50%)  | 1.15 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.18 (50%)  | 1.15 (1%) :x: |
| `["array","reductions",("var","Float64")]` | 0.89 (15%)  | 0.83 (1%) :white_check_mark: |
| `["array","reductions",("var","Int64")]` | 0.98 (15%)  | 0.85 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Year")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 1.08 (45%)  | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 0.98 (15%)  | 1.02 (1%) :x: |
| `["misc","parse","Int"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.32 (15%) :x: | 1.21 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["problem","simplex","simplex"]` | 1.00 (15%)  | 1.30 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.06 (15%)  | 1.11 (1%) :x: |
| `["random","collections",("rand!","ImplicitRNG","large String")]` | 1.01 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","ImplicitRNG","small String")]` | 1.00 (25%)  | 1.29 (1%) :x: |
| `["random","collections",("rand!","MersenneTwister","large String")]` | 1.01 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","MersenneTwister","small String")]` | 1.00 (25%)  | 1.29 (1%) :x: |
| `["random","collections",("rand!","RandomDevice","large String")]` | 1.04 (25%)  | 1.01 (1%) :x: |
| `["random","collections",("rand!","RandomDevice","small String")]` | 1.04 (25%)  | 1.29 (1%) :x: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 1.20 (25%)  | 1.07 (1%) :x: |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 1.04 (25%)  | 1.03 (1%) :x: |
| `["random","ranges",("RangeGenerator","Int32","1:1")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt128","1:170141183460469231731687303715884105728")]` | 1.65 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt16","1:1")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt8","1:1")]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.01 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.02 (50%)  | 0.97 (1%) :white_check_mark: |
| `["scalar","iteration","in"]` | 2.37 (25%) :x: | 1.00 (1%)  |
| `["scalar","iteration","indexed"]` | 3.54 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 1.00 (15%)  | 0.65 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4095)]` | 0.62 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["simd",("local_arrays","Float32",4096)]` | 0.61 (20%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4096)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 0.99 (30%)  | 1.22 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.00 (30%)  | 1.22 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 0.95 (30%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 0.99 (30%)  | 1.13 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 2.52 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","splogical",1000)]` | 3.63 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["string","search","String"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.99 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.99 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 1.15 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1283
Commit af70f66 (2017-08-07 22:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83432386 s          0 s   15043146 s  3670208620 s         86 s
       #2  3501 MHz  343855978 s          0 s    9472093 s  3424200184 s         13 s
       #3  3501 MHz   72614855 s          0 s    8368152 s  3696933677 s         73 s
       #4  3501 MHz   69313937 s          0 s    8555998 s  3700034078 s         17 s
       
  Memory: 31.383651733398438 GB (4578.35546875 MB free)
  Uptime: 3.7797298e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1281
Commit 66a505d (2017-08-07 21:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83509287 s          0 s   15052322 s  3670805802 s         86 s
       #2  3501 MHz  344481097 s          0 s    9482806 s  3424249627 s         13 s
       #3  3501 MHz   72693334 s          0 s    8375238 s  3697533283 s         73 s
       #4  3501 MHz   69408983 s          0 s    8563026 s  3700617367 s         17 s
       
  Memory: 31.383651733398438 GB (4360.0390625 MB free)
  Uptime: 3.7804157e7 sec
  Load Avg:  1.0654296875  1.037109375  1.04833984375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
