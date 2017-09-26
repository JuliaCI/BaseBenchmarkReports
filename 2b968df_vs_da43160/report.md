# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@2b968dff2a9374af92690aa8f1a725a087cd6711](https://github.com/pkofod/julia/commit/2b968dff2a9374af92690aa8f1a725a087cd6711) vs [JuliaLang/julia@da4316011f476b7e3b4f60ec4e26d5dd03eb1209](https://github.com/JuliaLang/julia/commit/da4316011f476b7e3b4f60ec4e26d5dd03eb1209)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22824#issuecomment-332101675)

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
| `["array","growth",("push_single!",256)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.54 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrt","UpperTriangular",1024)]` | 0.54 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","Float64"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["random","collections",("rand","RandomDevice","large String")]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random","collections",("rand","RandomDevice","small String")]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.07 (25%)  | 1.01 (1%) :x: |
| `["random","types",("rand!","MersenneTwister","Complex{Int16}")]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand!","MersenneTwister","Complex{Int8}")]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand!","MersenneTwister","Complex{UInt32}")]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Int32")]` | 1.21 (25%)  | 1.07 (1%) :x: |
| `["random","types",("randexp!","MersenneTwister","Float16")]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randn!","MersenneTwister","Float16")]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randn!","MersenneTwister","Float32")]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randn!","MersenneTwister","Float64")]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= abs(x) < 1","negative argument","Float64")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","cos_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","cos_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32","sin_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32","sin_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","sin_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","cos_kernel")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float32","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float32","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float32","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float32")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float64")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","sin_kernel")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","sin_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float64","sin_kernel")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float64","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float32")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float64")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(8,8))]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","atan"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1966
Commit 2b968df (2017-09-26 06:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   86672414 s          0 s   13509444 s  4096557758 s        168 s
       #2  3501 MHz  346527397 s          0 s   14382281 s  3837890721 s         58 s
       #3  3501 MHz   72346814 s          0 s    8272696 s  4123736247 s         78 s
       #4  3501 MHz   67664698 s          0 s    8164980 s  4128921382 s         28 s
       
  Memory: 31.383651733398438 GB (3128.1953125 MB free)
  Uptime: 4.2061595e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1959
Commit da43160 (2017-09-26 06:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   86766015 s          0 s   13518986 s  4097121870 s        168 s
       #2  3501 MHz  347136266 s          0 s   14393837 s  3837939360 s         58 s
       #3  3501 MHz   72434258 s          0 s    8280628 s  4124309912 s         78 s
       #4  3501 MHz   67743950 s          0 s    8172611 s  4129503696 s         28 s
       
  Memory: 31.383651733398438 GB (2676.7890625 MB free)
  Uptime: 4.2068295e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
