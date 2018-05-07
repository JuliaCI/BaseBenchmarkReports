# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@74af87841b8652e80de10ae4a101de2d6a2f4434](https://github.com/JuliaLang/julia/commit/74af87841b8652e80de10ae4a101de2d6a2f4434)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/74af87841b8652e80de10ae4a101de2d6a2f4434#commitcomment-28876089)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-05-07 vs 2018-05-06

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
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "5d"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(10, \"tup_tup\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(3, \"tup_tup\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter!\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"true\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967295)\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967297)\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Float64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"UInt64\", \"-\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isequal\", \"BigFloat\")"]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isless\", \"BigFloat\")"]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.46 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (2, 2), (2, 2))"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (4, 4), (4, 4))"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (8, 8), (8, 8))"]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (16, 16), (16,))"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (2, 2), (2,))"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (8, 8), (8,))"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (2, 2))"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4,))"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.5025
Commit 74af878 (2018-05-06 22:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   10009308 s        264 s    1242817 s  339958916 s          4 s
       #2  3501 MHz   61248694 s          0 s     886528 s  289700590 s          1 s
       #3  3501 MHz    7278769 s       2371 s     704922 s  343552888 s          6 s
       #4  3501 MHz    7053564 s          0 s     869192 s  343812371 s          1 s
       
  Memory: 31.383651733398438 GB (6129.95703125 MB free)
  Uptime: 3.520801e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
