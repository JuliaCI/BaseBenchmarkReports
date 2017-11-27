# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@31995428f8791b8bf63017d584405245d9f86aed](https://github.com/JuliaLang/julia/commit/31995428f8791b8bf63017d584405245d9f86aed)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/31995428f8791b8bf63017d584405245d9f86aed#commitcomment-25863356)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-11-27 vs 2017-11-22

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
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.61 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 0.99 (15%)  | 3.00 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Hour\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["dates", "construction", "Date"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 2.44 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["micro", "fib"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 0.98 (15%)  | 0.96 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 0.99 (15%)  | 0.99 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.10 (15%)  | 1.02 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.11 (15%)  | 1.03 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.11 (15%)  | 1.03 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.11 (15%)  | 1.03 (1%) :x: |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["problem", "json", "parse_json"]` | 0.30 (15%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:1)\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:1)\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Float64\")"]` | 0.29 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Int64\")"]` | 0.23 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Bool\")"]` | 0.22 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 0.28 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 0.22 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 0.28 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 0.29 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int16}\")"]` | 0.22 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int32}\")"]` | 0.21 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int64}\")"]` | 0.27 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int8}\")"]` | 0.21 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 0.30 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 0.22 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 0.23 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt64}\")"]` | 0.28 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt8}\")"]` | 0.22 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float16\")"]` | 0.27 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float32\")"]` | 0.22 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float64\")"]` | 0.21 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int128\")"]` | 0.24 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int16\")"]` | 0.20 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int32\")"]` | 0.20 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int64\")"]` | 0.22 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int8\")"]` | 0.20 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt128\")"]` | 0.25 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt16\")"]` | 0.20 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt32\")"]` | 0.20 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt64\")"]` | 0.21 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt8\")"]` | 0.20 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Float64\")"]` | 0.21 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Int64\")"]` | 0.24 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"Float64\")"]` | 0.23 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float16\")"]` | 0.42 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float32\")"]` | 0.24 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float64\")"]` | 0.26 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"Float64\")"]` | 0.35 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"Float64\")"]` | 0.24 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 0.33 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 0.27 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 0.20 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float16\")"]` | 0.26 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float32\")"]` | 0.29 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float64\")"]` | 0.37 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"RandomDevice\", \"Float64\")"]` | 0.30 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "pidigits"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint\", (20000, 10000))"]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint\", (20000, 20000))"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 8, Float32)"]` | 1.76 (40%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 1.56 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "growth"]`
- `["array", "index"]`
- `["array", "reductions"]`
- `["array", "reverse"]`
- `["array", "setindex!"]`
- `["array", "subarray"]`
- `["broadcast", "dotop"]`
- `["broadcast", "fusion"]`
- `["broadcast", "mix_scalar_tuple"]`
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["micro"]`
- `["misc", "afoldl"]`
- `["misc", "bitshift"]`
- `["misc", "julia"]`
- `["misc", "parse"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
- `["nullable", "basic"]`
- `["nullable", "nullablearray"]`
- `["parallel", "remotecall"]`
- `["problem", "chaosgame"]`
- `["problem", "fem"]`
- `["problem", "go"]`
- `["problem", "grigoriadis khachiyan"]`
- `["problem", "imdb"]`
- `["problem", "json"]`
- `["problem", "laplacian"]`
- `["problem", "monte carlo"]`
- `["problem", "raytrace"]`
- `["problem", "seismic"]`
- `["problem", "simplex"]`
- `["problem", "spellcheck"]`
- `["problem", "stockcorr"]`
- `["problem", "ziggurat"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["scalar", "acos"]`
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "cos"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "transpose"]`
- `["string"]`
- `["string", "readuntil"]`
- `["string", "search"]`
- `["string", "searchindex"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2663
Commit 3199542 (2017-11-27 04:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  104061212 s          0 s   18461799 s  4604826213 s         98 s
       #2  3501 MHz  444733760 s          0 s   11786077 s  4281894283 s         22 s
       #3  3501 MHz   87842931 s          0 s   10071340 s  4640974162 s         81 s
       #4  3501 MHz   84027930 s          0 s   10262040 s  4644586771 s         21 s
       
  Memory: 31.383651733398438 GB (2756.796875 MB free)
  Uptime: 4.7411542e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
