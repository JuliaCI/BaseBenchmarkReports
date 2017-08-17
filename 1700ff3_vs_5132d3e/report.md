# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1700ff3188e2ce279218a928432771538aac2716](https://github.com/JuliaLang/julia/commit/1700ff3188e2ce279218a928432771538aac2716) vs [JuliaLang/julia@5132d3e2d7a7bea2ac070d7ccbe908740a702e0b](https://github.com/JuliaLang/julia/commit/5132d3e2d7a7bea2ac070d7ccbe908740a702e0b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23240#issuecomment-322947518)

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
| `["array","cat",("catnd",500)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 0.91 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.50 (15%) :x: | 1.21 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 1.54 (15%) :x: | 1.29 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 1.69 (15%) :x: | 1.29 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.06 (15%)  | 1.20 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.54 (15%) :x: | 1.21 (1%) :x: |
| `["array","growth",("prerend!",2048)]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1:100000")]` | 2.49 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 13.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 13.50 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 5.26 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 13.04 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 6.29 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 13.00 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 6.28 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 13.11 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 8.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 12.89 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 6.64 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 2.68 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","1:100000")]` | 8.06 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000")]` | 2.94 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 2.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 12.17 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 6.24 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 13.34 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 6.31 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 9.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 13.03 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 7.43 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 2.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000")]` | 2.33 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 2.31 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.89 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.90 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.89 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.90 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.85 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.87 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","1:100000")]` | 9.34 (50%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["io","read","readstring"]` | 1.09 (15%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",1024)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.84 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.85 (45%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.04 (15%)  | 1.02 (1%) :x: |
| `["misc","julia",("macroexpand","evalpoly")]` | 1.06 (15%)  | 1.02 (1%) :x: |
| `["misc","repeat",(200,24,1)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["problem","json","parse_json"]` | 1.01 (15%)  | 0.99 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem","simplex","simplex"]` | 1.00 (15%)  | 1.30 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.06 (15%)  | 0.90 (1%) :white_check_mark: |
| `["random","ranges",("RangeGenerator","Int16","1:1")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","Int8","1:1")]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand!","MersenneTwister","Int","1:1000")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.46 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","UInt128","RangeGenerator(1:170141183460469231731687303715884105728)")]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.92 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","fastmath",("mul","BigInt")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","+")]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody"]` | 1.00 (15%)  | 0.65 (1%) :white_check_mark: |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.50 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 22.91 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 28.05 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 12.67 (20%) :x: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 13.94 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4095)]` | 13.54 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4096)]` | 14.25 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 10.84 (20%) :x: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 11.13 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 19.39 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 19.79 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 15.32 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 14.91 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 18.17 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 18.93 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 13.57 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 14.04 (20%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","range",10)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,))]` | 3.95 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 11.13 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 4.08 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 4.32 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 4.80 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,4))]` | 3.95 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 4.60 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 2.88 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1373
Commit 1700ff3 (2017-08-17 01:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   80560697 s          0 s   12399151 s  3757319321 s        141 s
       #2  3501 MHz  323090331 s          0 s   13536526 s  3515192274 s         49 s
       #3  3501 MHz   68705913 s          0 s    7849060 s  3780489182 s         66 s
       #4  3501 MHz   64054290 s          0 s    7785588 s  3785559458 s         23 s
       
  Memory: 31.383651733398438 GB (4930.36328125 MB free)
  Uptime: 3.8587354e7 sec
  Load Avg:  1.0068359375  1.02099609375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1369
Commit 5132d3e (2017-08-16 21:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   80641760 s          0 s   12408153 s  3757835467 s        141 s
       #2  3501 MHz  323633585 s          0 s   13547483 s  3515246071 s         50 s
       #3  3501 MHz   68786178 s          0 s    7856287 s  3781009548 s         66 s
       #4  3501 MHz   64147180 s          0 s    7792976 s  3786067272 s         23 s
       
  Memory: 31.383651733398438 GB (4553.98046875 MB free)
  Uptime: 3.8593441e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
