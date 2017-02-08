# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e2cceb619d100d57ccdd06aa1fdc6b4ec6d650a5](https://github.com/JuliaLang/julia/commit/e2cceb619d100d57ccdd06aa1fdc6b4ec6d650a5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/e2cceb619d100d57ccdd06aa1fdc6b4ec6d650a5#commitcomment-20799190)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-02-08 vs 2017-01-28

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
| `["array","cat",("catnd",5)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("append!",256)]` | 0.91 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array","growth",("push_single!",2048)]` | 0.93 (15%)  | 1.04 (1%) :x: |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.03 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.03 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.95 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.96 (50%)  | 0.94 (1%) :white_check_mark: |
| `["dates","accessor","millisecond"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Day")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Day")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Hour")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Millisecond")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Minute")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Second")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates","conversion","Date -> DateTime"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.12 (15%)  | 0.98 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","DateFormat")]` | 1.06 (15%)  | 0.97 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 0.99 (45%)  | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 0.99 (45%)  | 0.53 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 0.99 (45%)  | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 0.99 (45%)  | 0.53 (1%) :white_check_mark: |
| `["nullable","basic",("get1","Nullable{Bool}(true)")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{Float32}(1.0)")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{Float64}(1.0)")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{Int64}(1)")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get1","Nullable{Int8}(1)")]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Bool}()")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Bool}(true)")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float32}()")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float64}()")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int64}()")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int64}(1)")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int8}()")]` | 1.61 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int8}(1)")]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(false)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}(true)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}()")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(false)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}(true)","Nullable{Bool}(true)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}()")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(0.0)")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}(1.0)")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}()")]` | 2.33 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(0.0)")]` | 2.33 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}(1.0)","Nullable{Float32}(1.0)")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}()")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(0.0)")]` | 2.33 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}(1.0)")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}()")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(0.0)")]` | 2.34 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}(1.0)","Nullable{Float64}(1.0)")]` | 2.33 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}()")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(0)")]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}(1)")]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}()")]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(0)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}(1)","Nullable{Int64}(1)")]` | 1.82 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(0)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}(1)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}()")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(0)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}(1)","Nullable{Int8}(1)")]` | 1.81 (30%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Bool}()")]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 1.03 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigInt}")]` | 1.14 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 1.12 (50%)  | 1.08 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 1.30 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float32}")]` | 0.97 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 0.98 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigInt")]` | 1.15 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 1.10 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 1.11 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Int64}")]` | 1.30 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Int64")]` | 1.09 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 1.13 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 1.04 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 1.12 (50%)  | 1.08 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigFloat}")]` | 0.95 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 1.12 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float32}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float64}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Int64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{UInt64}")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","Int64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float32}","UInt64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 1.12 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float64}")]` | 1.81 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","Int64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","UInt64")]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 1.10 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigInt}")]` | 1.08 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float32}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Int64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float32}")]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 0.99 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{Float32}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{Float64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Float32")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Float64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 2.59 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Float64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Int64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{BigInt}")]` | 1.10 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","Int64","Complex{Float32}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{Float64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Complex{Int64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Float64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Int64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 1.13 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("add","UInt64","Complex{Float32}")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Float64}")]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","UInt64")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float32")]` | 0.97 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 1.16 (50%)  | 1.08 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 1.12 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 1.07 (50%)  | 1.08 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 1.12 (50%)  | 1.08 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigFloat")]` | 0.99 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float32}","Float32")]` | 3.60 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Float64")]` | 4.15 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","Int64")]` | 3.75 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float32}","UInt64")]` | 3.65 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","Float32")]` | 4.14 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Float64")]` | 4.11 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","Int64")]` | 4.97 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Float64}","UInt64")]` | 4.13 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 1.17 (50%)  | 1.08 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Float32")]` | 3.61 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Float64")]` | 4.12 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","Int64")]` | 5.41 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{Int64}","UInt64")]` | 5.45 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 1.15 (50%)  | 1.08 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float32")]` | 3.62 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float64")]` | 4.12 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Int64")]` | 4.26 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","UInt64")]` | 4.12 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Complex{Int64}")]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Float32")]` | 1.81 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Float64")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","Int64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float32","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Float32")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Float64")]` | 2.06 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","Int64")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","UInt64")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Float64")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 4.11 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","UInt64")]` | 3.35 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Float64")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","Int64")]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","UInt64")]` | 2.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 1.09 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 1.17 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 1.17 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 1.02 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 1.13 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 1.12 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 1.08 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 1.17 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 2.90 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 3.88 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{UInt64}")]` | 3.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","Int64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float32}","UInt64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 2.89 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 1.81 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 3.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 3.12 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float32")]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","Int64")]` | 2.13 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 3.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 3.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 1.82 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float32}")]` | 3.86 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 3.10 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 1.82 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float32")]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.59 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{UInt64}","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 1.00 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 1.13 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{Float32}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{Float64}")]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{Int64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Complex{UInt64}")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Float32")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","Float64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 1.15 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{Float32}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Float64}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{Int64}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Float64")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Float32}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Complex{Float64}")]` | 2.13 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Float64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Int64")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float32}")]` | 2.06 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Complex{UInt64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","UInt64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float32}")]` | 1.05 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 1.04 (50%)  | 1.24 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigInt")]` | 1.14 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 1.14 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Int64}")]` | 1.29 (50%)  | 1.27 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Int64")]` | 1.10 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 1.13 (50%)  | 1.50 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 1.09 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 1.14 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigFloat}")]` | 1.08 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 1.16 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float32}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Int64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{UInt64}")]` | 2.33 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","Int64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float32}","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 1.18 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float64}")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 2.60 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float32")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","Int64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","UInt64")]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 1.15 (50%)  | 1.29 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigInt}")]` | 1.15 (50%)  | 1.29 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float32}")]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.59 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float32")]` | 2.07 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Float32}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Float64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{Int64}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Complex{UInt64}")]` | 2.58 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Float32")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","Float64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","UInt64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Float32}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Float64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{Int64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Complex{UInt64}")]` | 2.85 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Float64")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","Int64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","UInt64")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Float32}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Complex{Float64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Float32")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Float64")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Int64","Int64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float32}")]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float64}")]` | 2.33 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Complex{UInt64}")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Float32")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","Float64")]` | 1.81 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","UInt64","UInt64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float32}")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Float32")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Int64")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("add","UInt64")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Float32")]` | 1.81 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Float64")]` | 2.06 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 4.11 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","UInt64")]` | 2.33 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Float64}")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{Int64}")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Float32")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","UInt64")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Float64}")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{Int64}")]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Complex{UInt64}")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","Float32")]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float32")]` | 1.73 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float64")]` | 1.73 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","norm","Float32")]` | 1.73 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","norm","Float64")]` | 1.74 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float32")]` | 1.93 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float64")]` | 1.69 (40%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Float32}")]` | 2.60 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Float64}")]` | 2.60 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Int64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{UInt64}")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Float32")]` | 1.57 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Float64")]` | 1.81 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Int64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","UInt64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("iseven","Int64")]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("iseven","UInt64")]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Int64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{UInt64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float32")]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Int64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{UInt64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Int64")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","UInt64")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Int64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{UInt64}")]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float32")]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Float32")]` | 2.34 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Float64")]` | 2.34 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Int64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isless","UInt64")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Float32}")]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Float64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Int64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{UInt64}")]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float32")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float64")]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","Int64")]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 61.00 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 64.78 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 59.51 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 62.23 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 22.77 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 22.62 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 22.59 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 22.57 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 39.34 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 41.64 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 39.86 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 41.12 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 7.12 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 7.13 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 6.91 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 6.89 (20%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2661
Commit e2cceb6 (2017-02-08 04:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9604.04296875 MB free)
Uptime: 2.2215674e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   35245988 s          0 s    7717029 s  2172175843 s         64 s
#2  3501 MHz  116347392 s          0 s    4530892 s  2099412729 s          8 s
#3  3501 MHz   31411059 s          0 s    3935664 s  2185201331 s         46 s
#4  3501 MHz   29304180 s          0 s    4078175 s  2187155294 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
