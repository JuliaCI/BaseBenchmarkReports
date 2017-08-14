# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@89f3e17cd77c0ff8c28f38328147cf2d7ad8081a](https://github.com/pkofod/julia/commit/89f3e17cd77c0ff8c28f38328147cf2d7ad8081a) vs [JuliaLang/julia@a62160e95b12cfaba91ba02e6998127b5c8a19d7](https://github.com/JuliaLang/julia/commit/a62160e95b12cfaba91ba02e6998127b5c8a19d7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22824#issuecomment-322276164)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.43 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.43 (45%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","positive argument","Float32")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","cos_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","cos_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32","sin_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","sin_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32","cos_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","cos_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float32","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float32","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float32","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float32")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float64")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","sin_kernel")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","sin_kernel")]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","sin_kernel")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float32","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float32","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float32")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float64")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.17 (15%) :x: | 1.00 (1%)  |
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
Julia Version 0.7.0-DEV.1372
Commit 89f3e17 (2017-08-14 18:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84969967 s          0 s   15300186 s  3727396913 s         88 s
       #2  3501 MHz  353303240 s          0 s    9700366 s  3473658426 s         13 s
       #3  3501 MHz   74230440 s          0 s    8527464 s  3754293637 s         74 s
       #4  3501 MHz   70882619 s          0 s    8711277 s  3757452325 s         17 s
       
  Memory: 31.383651733398438 GB (2905.75 MB free)
  Uptime: 3.8388958e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1342
Commit a62160e (2017-08-14 17:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   85050439 s          0 s   15309205 s  3727992422 s         88 s
       #2  3501 MHz  353925155 s          0 s    9711459 s  3473712397 s         13 s
       #3  3501 MHz   74325314 s          0 s    8534472 s  3754878787 s         74 s
       #4  3501 MHz   70960213 s          0 s    8718380 s  3758054714 s         17 s
       
  Memory: 31.383651733398438 GB (3108.31640625 MB free)
  Uptime: 3.8395834e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
