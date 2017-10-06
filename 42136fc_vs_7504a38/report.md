# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@42136fc5952bb846952ccae3d133a5dcac82913a](https://github.com/pkofod/julia/commit/42136fc5952bb846952ccae3d133a5dcac82913a) vs [JuliaLang/julia@7504a381631328bd8e6411a179e12977b0d0a41c](https://github.com/JuliaLang/julia/commit/7504a381631328bd8e6411a179e12977b0d0a41c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22824#issuecomment-334658542)

*Tag Predicate:* `"scalar"`

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
| `["scalar","atan2",("x one","Float32")]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan2",("x one","Float64")]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","cos_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","cos_kernel")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","cos_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","cos_kernel")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","sin_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","cos_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float32","cos_kernel")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","cos_kernel")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float32","cos_kernel")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","cos_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","sin_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","cos_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.38 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float32","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","negative argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float32","cos_kernel")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float32")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("no reduction","zero","Float64")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64","sin_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","sin_kernel")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","sin_kernel")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64","cos_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64","sin_kernel")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64","sin_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64","sin_kernel")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64","sin_kernel")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64","sin_kernel")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64","cos_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64","cos_kernel")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64","sin_kernel")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","cos_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32","sin_kernel")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","cos_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","cos_kernel")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32","sin_kernel")]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","cos_kernel")]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64","sin_kernel")]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","negative argument","Float64","sin_kernel")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float32","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","positive argument","Float64","sin_kernel")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float32")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("no reduction","zero","Float64")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float32")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float32")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float32")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float32")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float32")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float32")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float32")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float32")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float32")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float32")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float32")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float32")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float32")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float32")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float32")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 4π/4","positive argument","Float64")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float32")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float32")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float32")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 8π/4","negative argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float32")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float32")]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float32")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64")]` | 0.34 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","negative argument","Float32")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","negative argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","positive argument","Float32")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","positive argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","zero","Float32")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sincos",("no reduction","zero","Float64")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","atan2"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","sincos"]`
- `["scalar","tan"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2065
Commit 42136fc (2017-10-05 22:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88747566 s          0 s   13771290 s  4179398515 s        178 s
       #2  3501 MHz  359191224 s          0 s   14809394 s  3909963713 s         64 s
       #3  3501 MHz   74451949 s          0 s    8487065 s  4206733931 s         84 s
       #4  3501 MHz   69707644 s          0 s    8364555 s  4212003303 s         30 s
       
  Memory: 31.383651733398438 GB (3090.1171875 MB free)
  Uptime: 4.2915111e7 sec
  Load Avg:  0.9228515625  0.998046875  1.15380859375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2051
Commit 7504a38 (2017-10-05 22:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88828217 s          0 s   13779676 s  4179645002 s        178 s
       #2  3501 MHz  359466177 s          0 s   14817275 s  3910017141 s         64 s
       #3  3501 MHz   74550567 s          0 s    8494886 s  4206963672 s         84 s
       #4  3501 MHz   69790978 s          0 s    8372196 s  4212248752 s         30 s
       
  Memory: 31.383651733398438 GB (2960.140625 MB free)
  Uptime: 4.291848e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.14111328125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
