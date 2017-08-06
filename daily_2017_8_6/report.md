# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ae1719872092b594228a9bfeedfc3fa8e91c9529](https://github.com/JuliaLang/julia/commit/ae1719872092b594228a9bfeedfc3fa8e91c9529)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ae1719872092b594228a9bfeedfc3fa8e91c9529#commitcomment-23500994)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-06 vs 2017-08-05

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
| `["array","growth",("append!",256)]` | 0.99 (15%)  | 1.03 (1%) :x: |
| `["array","growth",("prerend!",2048)]` | 0.92 (15%)  | 0.90 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["random","collections",("rand!","ImplicitRNG","small IntSet")]` | 0.28 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand!","MersenneTwister","small IntSet")]` | 0.26 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand!","RandomDevice","small IntSet")]` | 0.02 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","small IntSet")]` | 0.28 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","small IntSet")]` | 0.26 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","RandomDevice","small IntSet")]` | 0.26 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.01 (25%)  | 1.02 (1%) :x: |
| `["random","types",("rand","MersenneTwister","UInt32")]` | 0.89 (25%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","acos",("0.5 <= |x| < 1","negative argument","Float32")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= |x| < 1","negative argument","Float64")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= |x| < 1","positive argument","Float32")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= |x| < 1","positive argument","Float64")]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","negative argument","Float32")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","negative argument","Float64")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float32")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float64")]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("small","negative argument","Float32")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("small","negative argument","Float64")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("small","positive argument","Float32")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("small","positive argument","Float64")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("zero","Float32")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("zero","Float64")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("|x| < 0.5","negative argument","Float32")]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("|x| < 0.5","negative argument","Float64")]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("|x| < 0.5","positive argument","Float32")]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("|x| < 0.5","positive argument","Float64")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= |x| < 0.975","negative argument","Float32")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= |x| < 0.975","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= |x| < 0.975","positive argument","Float32")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= |x| < 0.975","positive argument","Float64")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= |x| < 1.0","negative argument","Float64")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= |x| < 1.0","positive argument","Float64")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","negative argument","Float32")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","negative argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float32")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","negative argument","Float32")]` | 0.28 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","negative argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","positive argument","Float32")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","positive argument","Float64")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float32")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float64")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","negative argument","Float32")]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","negative argument","Float64")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","positive argument","Float32")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","positive argument","Float64")]` | 0.27 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","cos_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","cos_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","cos_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float32","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float32","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","cos_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.21 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64")]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64")]` | 0.21 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64")]` | 0.21 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64")]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64")]` | 0.21 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) > 2.0^20*π/2","positive argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64")]` | 0.24 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 0.21 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32","cos_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32","cos_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32","sin_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float32","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32","sin_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float32","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float32","sin_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","cos_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","cos_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float32","cos_kernel")]` | 0.36 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32","sin_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32","sin_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1257
Commit ae17198 (2017-08-06 00:04 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82939512 s          0 s   14966840 s  3655498952 s         86 s
       #2  3501 MHz  341187799 s          0 s    9410577 s  3411608749 s         13 s
       #3  3501 MHz   72101180 s          0 s    8317989 s  3682177945 s         73 s
       #4  3501 MHz   68818088 s          0 s    8509325 s  3685253364 s         17 s
       
  Memory: 31.383651733398438 GB (5511.7578125 MB free)
  Uptime: 3.7644013e7 sec
  Load Avg:  0.92578125  0.9990234375  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
