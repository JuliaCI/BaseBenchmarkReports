# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@469194a3ed09fe0c878b5f53272fe3c590ff3d68](https://github.com/JuliaLang/julia/commit/469194a3ed09fe0c878b5f53272fe3c590ff3d68) vs [JuliaLang/julia@8f46450f61c27de38e26f13c5fe20c2a4b2e6108](https://github.com/JuliaLang/julia/commit/8f46450f61c27de38e26f13c5fe20c2a4b2e6108)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25377#issuecomment-383167483)

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
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.31 (15%) :x: | 1.03 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.35 (15%) :x: | 1.05 (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 4.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 3.00 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.75 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 2.63 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 171.08 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 0.98 (15%)  | 1.01 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 9.85 (15%) :x: | 2.50 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 4.53 (15%) :x: | 2.14 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 6.19 (15%) :x: | 2.25 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 19.38 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 14.55 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 17.04 (15%) :x: | Inf (1%) :x: |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"length\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"pop!\", \"unspecified\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "query", "(\"daysofweekinmonth\", \"Date\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.31 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 1.00 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 1.03 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.23 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 1.01 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.05 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.10 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 1.04 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 0.94 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 1.07 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 0.94 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 0.93 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 0.97 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 1.02 (45%)  | 1.03 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 1.07 (45%)  | 1.03 (1%) :x: |
| `["micro", "fib"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 6.22 (15%) :x: | 7.58 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 1.47 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float32\")"]` | 1.56 (40%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float64\")"]` | 1.72 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isless\", \"BigFloat\")"]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint\", (600, 600))"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 1.02 (15%)  | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 1.55 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 1.55 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 0.99 (15%)  | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.50 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 1.57 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.32 (15%) :x: | 0.32 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 4.90 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 4.88 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 0.92 (15%)  | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 3.99 (15%) :x: | 0.96 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 4.10 (15%) :x: | 0.96 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 1.15 (15%)  | 0.78 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 4.73 (15%) :x: | 0.89 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 4.78 (15%) :x: | 0.89 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.94 (15%)  | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 4.14 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 4.16 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 0.91 (15%)  | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 4.08 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 4.09 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 1.23 (15%) :x: | 0.52 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 5.07 (15%) :x: | 0.76 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 5.11 (15%) :x: | 0.76 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 2.06 (15%) :x: | 0.99 (1%)  |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 1.04 (15%)  | 0.97 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 2.29 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.68 (15%) :x: | 0.38 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 7.58 (15%) :x: | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 1.24 (15%) :x: | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 5.31 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.44 (15%) :x: | 0.81 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 7.21 (15%) :x: | 0.91 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 1.10 (15%)  | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 5.94 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 1.11 (15%)  | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 5.82 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.49 (15%) :x: | 0.56 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 7.83 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 1.38 (15%) :x: | 0.90 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 5.68 (15%) :x: | 0.95 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 1.41 (15%) :x: | 0.90 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 5.69 (15%) :x: | 0.95 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.62 (15%) :x: | 0.38 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 7.79 (15%) :x: | 0.84 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.22 (15%) :x: | 0.94 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 5.32 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 1.43 (15%) :x: | 0.81 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 7.32 (15%) :x: | 0.91 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 1.10 (15%)  | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 5.95 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 1.11 (15%)  | 0.86 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 5.77 (15%) :x: | 0.93 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.46 (15%) :x: | 0.56 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 7.90 (15%) :x: | 0.79 (1%) :white_check_mark: |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "accumulate"]`
- `["array", "any/all"]`
- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "equality"]`
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
- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "optimizations"]`
- `["collection", "queries & updates"]`
- `["collection", "set operations"]`
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["find", "findall"]`
- `["find", "findnext"]`
- `["find", "findprev"]`
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
- `["scalar", "acosh"]`
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "asinh"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "atanh"]`
- `["scalar", "cbrt"]`
- `["scalar", "cos"]`
- `["scalar", "cosh"]`
- `["scalar", "exp2"]`
- `["scalar", "expm1"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "sinh"]`
- `["scalar", "tan"]`
- `["scalar", "tanh"]`
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
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.4966
Commit 469194a (2018-04-20 17:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    4441740 s        259 s     603671 s  203003909 s          2 s
       #2  3501 MHz   34010956 s          0 s     502198 s  173864798 s          0 s
       #3  3501 MHz    3909546 s       2368 s     392980 s  203817717 s          2 s
       #4  3501 MHz    3822967 s          0 s     498375 s  203974202 s          1 s
       
  Memory: 31.383651733398438 GB (15828.01171875 MB free)
  Uptime: 2.085113e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4916
Commit 8f46450 (2018-04-20 15:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    4533187 s        259 s     613146 s  203775703 s          2 s
       #2  3501 MHz   34807336 s          0 s     511952 s  173934057 s          0 s
       #3  3501 MHz    4017039 s       2368 s     400662 s  204577308 s          2 s
       #4  3501 MHz    3913716 s          0 s     505752 s  204751410 s          1 s
       
  Memory: 31.383651733398438 GB (15524.4140625 MB free)
  Uptime: 2.093872e6 sec
  Load Avg:  1.03564453125  1.0263671875  1.0458984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
