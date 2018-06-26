# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@394bc4ae7caeb85d6a20e61647f05fe05e1344dd](https://github.com/JuliaLang/julia/commit/394bc4ae7caeb85d6a20e61647f05fe05e1344dd) vs [JuliaLang/julia@c44644442949238da70670b547312ca1ae9a9c7d](https://github.com/JuliaLang/julia/commit/c44644442949238da70670b547312ca1ae9a9c7d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27776#issuecomment-400111137)

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
| `["array", "cat", "(\"catnd\", 5)"]` | 1.06 (15%)  | 1.04 (1%) :x: |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 1.96 (15%) :x: | 1.10 (1%) :x: |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 12.53 (50%) :x: | 2.56 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 12.54 (50%) :x: | 2.56 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 12.13 (50%) :x: | 2.56 (1%) :x: |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 13.50 (50%) :x: | 2.56 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 14.85 (50%) :x: | 2.56 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1.0:1.0:100000.0\")"]` | 15.88 (50%) :x: | 2.56 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"100000:-1:1\")"]` | 10.87 (50%) :x: | 2.67 (1%) :x: |
| `["array", "index", "(\"sumvector_view\", \"1:100000\")"]` | 17.56 (50%) :x: | 2.79 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"specified\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"unspecified\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"push!\", \"new\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"setindex!\", \"new\")"]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "mandel"]` | 1.00 (15%)  | 1.09 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.00 (15%)  | 1.05 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.02 (15%)  | 1.10 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.02 (15%)  | 1.06 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.01 (15%)  | 1.09 (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 0.59 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\")"]` | 13.89 (25%) :x: | 4.13 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", 100)"]` | 3.46 (25%) :x: | 2.25 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 5.62 (25%) :x: | 2.00 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 1.59 (25%) :x: | 1.35 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\")"]` | 13.10 (25%) :x: | 4.13 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\", 100)"]` | 2.41 (25%) :x: | 2.25 (1%) :x: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt32\")"]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "mandelbrot"]` | 1.00 (15%)  | 1.09 (1%) :x: |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 0.80 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 1.21 (20%) :x: | 1.01 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 1.20 (20%) :x: | 1.01 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Int32\", 4095)"]` | 1.17 (20%)  | 1.01 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Int32\", 4096)"]` | 1.17 (20%)  | 1.01 (1%) :x: |
| `["simd", "(\"sum_reduce\", \"Int64\", 4095)"]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int64\", 4096)"]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta.17
Commit 394bc4a (2018-06-26 00:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   17468525 s        259 s    2710394 s  759504134 s          5 s
       #2  3501 MHz   89068961 s          0 s    1408786 s  690803389 s          5 s
       #3  3501 MHz   12796282 s       2389 s    1514259 s  767079012 s         11 s
       #4  3501 MHz   12393921 s          4 s    1153226 s  768213174 s          4 s
       
  Memory: 31.383651733398438 GB (5150.02734375 MB free)
  Uptime: 7.821e6 sec
  Load Avg:  1.01220703125  1.02001953125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.12
Commit c446444 (2018-06-25 19:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   17589068 s        259 s    2722661 s  760460381 s          5 s
       #2  3501 MHz   90064510 s          0 s    1419917 s  690889980 s          5 s
       #3  3501 MHz   12939508 s       2389 s    1523408 s  768019589 s         11 s
       #4  3501 MHz   12511351 s          4 s    1161540 s  769180513 s          4 s
       
  Memory: 31.383651733398438 GB (5024.59375 MB free)
  Uptime: 7.831939e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
