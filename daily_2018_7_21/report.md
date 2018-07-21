# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1d3c9c8651ee48ee7e27fe478d369b707c1efb10](https://github.com/JuliaLang/julia/commit/1d3c9c8651ee48ee7e27fe478d369b707c1efb10)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/1d3c9c8651ee48ee7e27fe478d369b707c1efb10#commitcomment-29786836)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-07-21 vs 2018-07-19

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.52 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "string", "Date"]` | 1.19 (15%) :x: | 0.92 (1%) :white_check_mark: |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 0.90 (15%)  | 0.90 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 0.90 (15%)  | 0.80 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 0.92 (15%)  | 0.96 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 0.90 (15%)  | 0.87 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 0.91 (15%)  | 0.82 (1%) :white_check_mark: |
| `["problem", "json", "parse_json"]` | 0.86 (15%)  | 0.94 (1%) :white_check_mark: |
| `["problem", "spellcheck", "spellcheck"]` | 0.98 (15%)  | 1.05 (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551616\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"UInt64\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float32\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.52 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "mandelbrot"]` | 1.00 (15%)  | 0.97 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 1.23 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta2.61
Commit 1d3c9c8 (2018-07-21 02:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   44966632 s        282 s    4647910 s  945962781 s         11 s
       #2  3501 MHz  212011784 s          0 s    3066668 s  782861652 s          8 s
       #3  3501 MHz   30588734 s       2381 s    2506027 s  964454412 s         17 s
       #4  3501 MHz   28471823 s          0 s    2919732 s  966262759 s          9 s
       
  Memory: 31.383651733398438 GB (6409.37890625 MB free)
  Uptime: 9.985782e6 sec
  Load Avg:  0.92724609375  1.01025390625  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
