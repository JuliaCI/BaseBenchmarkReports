# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@242de064c46cee7deebdaaef489170582d85780e](https://github.com/JuliaLang/julia/commit/242de064c46cee7deebdaaef489170582d85780e) vs [JuliaLang/julia@6a1e339ac1ca24b0d00c1721a1833fb39106c559](https://github.com/JuliaLang/julia/commit/6a1e339ac1ca24b0d00c1721a1833fb39106c559)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/242de064c46cee7deebdaaef489170582d85780e#commitcomment-20329150)

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
| `["array","cat",("catnd",5)]` | 0.51 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["array","cat",("catnd",500)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 0.98 (15%)  | 0.97 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 1.10 (15%)  | 0.97 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 1.27 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","index","2d"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","3d"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","4d"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","5d"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","sub2ind"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000000:-1:1")]` | 0.45 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000000")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.94 (50%)  | 0.92 (1%) :white_check_mark: |
| `["array","index",("sumelt","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.39 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","100000000:-1:1")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000000")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","BitArray{2}")]` | 0.96 (50%)  | 0.93 (1%) :white_check_mark: |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 0.93 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","100000000:-1:1")]` | 0.92 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","1:100000000")]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Float32,2}")]` | 0.89 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","Array{Int32,2}")]` | 0.92 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.86 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.91 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.93 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.88 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.90 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 0.95 (50%)  | 0.95 (1%) :white_check_mark: |
| `["array","reductions",("mean","Float64")]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sum","Float64")]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs","Float64")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs2","Float64")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.24 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.10 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.12 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.30 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.64 (15%) :white_check_mark: | 1.35 (1%) :x: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 0.98 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),2)]` | 0.45 (15%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["broadcast","sparse",((10000000,),2)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Day")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Day")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Hour")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Millisecond")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Minute")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Second")]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","conversion","Date -> DateTime"]` | 0.50 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.88 (15%)  | 0.55 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.89 (15%)  | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.51 (15%) :white_check_mark: | 0.34 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.20 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.01 (45%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.96 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.96 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.93 (45%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 0.79 (45%)  | 0.84 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 0.59 (45%)  | 0.60 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 0.04 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.05 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 0.04 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.05 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.62 (45%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 0.78 (45%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.72 (45%)  | 0.72 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 0.82 (45%)  | 0.72 (1%) :white_check_mark: |
| `["micro","parseint"]` | 0.96 (15%)  | 0.78 (1%) :white_check_mark: |
| `["micro","randmatstat"]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc","bitshift",("Int","Int")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 2.68 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Bool}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Bool}(true)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float32}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float32}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float64}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int64}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int8}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int8}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(false)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(true)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(false)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(true)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(0.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(1.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(0.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(1.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(0.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(1.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(0.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(1.0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(1)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(0)")]` | 0.33 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(0)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(1)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}()")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(0)")]` | 0.33 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(1)")]` | 0.25 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Bool}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Bool}(true)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float32}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float32}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Float64}(1.0)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int64}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int8}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int8}(1)")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 0.26 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int64")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int8")]` | 0.27 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 0.29 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 0.24 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 0.17 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 0.05 (50%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.01 (15%)  | 1.10 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.00 (15%)  | 1.18 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 0.99 (15%)  | 1.05 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 0.99 (15%)  | 1.13 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.00 (15%)  | 1.18 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.51 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.50 (15%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_devec"]` | 1.01 (15%)  | 0.50 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.63 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 2.94 (50%) :x: | 4.29 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 2.77 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 2.66 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 2.63 (50%) :x: | 3.84 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.07 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.06 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.97 (50%) :x: | 1.79 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 2.02 (50%) :x: | 1.79 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 2.07 (50%) :x: | 2.00 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 2.10 (50%) :x: | 2.00 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.05 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.06 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 2.60 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.05 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Int64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Int64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{UInt64}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","UInt64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","norm","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float32")]` | 0.19 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float64")]` | 0.19 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float32")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float32")]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float64")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float32")]` | 0.09 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float64")]` | 0.09 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float32")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float64")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("significand","subnorm","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{BigInt}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{BigInt}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigInt")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{BigInt}")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Float32}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Int64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{UInt64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float32")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","UInt64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.20 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["shootout","revcomp"]` | 1.09 (25%)  | 0.97 (1%) :white_check_mark: |
| `["simd",("inner","Float32",4095)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Int32",4095)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Int32",4096)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["simd",("local_arrays","Int64",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.72 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 0.71 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.65 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4095)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float32",4096)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4095)]` | 0.68 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Float64",4096)]` | 0.67 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort forwards","ascending")]` | 1.66 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 2.44 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","random")]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ascending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","descending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm forwards","descending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(600,600))]` | 0.50 (30%) :white_check_mark: | 0.99 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.12 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.10 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 0.66 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.67 (30%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.56 (30%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1778
Commit 242de06 (2016-12-30 02:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3109.671875 MB free)
Uptime: 1.8766377e7 sec
Load Avg:  1.05908203125  1.029296875  1.048828125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   31480927 s          0 s    5074000 s  1836284486 s         55 s
#2  3501 MHz   94577058 s          0 s    6092172 s  1772845563 s         20 s
#3  3501 MHz   26848210 s          0 s    3399568 s  1845530231 s         30 s
#4  3501 MHz   22832246 s          0 s    3306973 s  1849796427 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.1-pre+31
Commit 6a1e339 (2016-11-17 17:50 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3391.66015625 MB free)
Uptime: 1.8772524e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   31535165 s          0 s    5082510 s  1836834567 s         55 s
#2  3501 MHz   95015182 s          0 s    6103820 s  1773009919 s         20 s
#3  3501 MHz   26892190 s          0 s    3406314 s  1846093242 s         31 s
#4  3501 MHz   22878099 s          0 s    3313449 s  1850358222 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
