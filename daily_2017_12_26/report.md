# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f3d6132db7df1039581f569accffde501fb13115](https://github.com/JuliaLang/julia/commit/f3d6132db7df1039581f569accffde501fb13115)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f3d6132db7df1039581f569accffde501fb13115#commitcomment-26480086)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-12-26 vs 2017-12-23

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.27 (15%) :x: | 2.33 (1%) :x: |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 1.56 (15%) :x: | 2.63 (1%) :x: |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 1.53 (15%) :x: | 1.33 (1%) :x: |
| `["array", "growth", "(\"push_single!\", 256)"]` | 1.68 (15%) :x: | 2.18 (1%) :x: |
| `["array", "growth", "(\"push_single!\", 8)"]` | 1.75 (15%) :x: | 2.84 (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.09 (15%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"getindex\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"specified\")"]` | 1.67 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"true\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"pop!\", \"unspecified\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"Vector\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["find", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.98 (15%)  | 0.98 (1%) :white_check_mark: |
| `["find", "(\"Base.Generator{Array{Bool,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##3#6\\\"))}\", \"50-50\")"]` | 1.01 (15%)  | 0.98 (1%) :white_check_mark: |
| `["find", "(\"BitArray{1}\", \"50-50\")"]` | 1.01 (15%)  | 0.98 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.83 (15%) :white_check_mark: | 0.99 (1%)  |
| `["find", "(\"ispos\", \"Base.Generator{Array{Bool,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 0.84 (15%) :white_check_mark: | 0.99 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.71 (15%) :x: | 1.76 (1%) :x: |
| `["problem", "ziggurat", "ziggurat"]` | 2.46 (15%) :x: | 2.86 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 1.67 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand!\", \"RandomDevice\", \"Int\", \"1:1000\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Bool\", \"RangeGenerator(true:true)\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967295)\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigInt\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Float64\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isless\", \"Float32\")"]` | 1.88 (25%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 1.60 (20%) :x: | 1.56 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 1.41 (20%) :x: | 1.56 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Float64\", 4095)"]` | 1.29 (20%) :x: | 1.33 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Float64\", 4096)"]` | 1.29 (20%) :x: | 1.33 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Int32\", 4095)"]` | 1.57 (20%) :x: | 1.56 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Int32\", 4096)"]` | 1.39 (20%) :x: | 1.56 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Int64\", 4095)"]` | 1.40 (20%) :x: | 1.33 (1%) :x: |
| `["simd", "(\"local_arrays\", \"Int64\", 4096)"]` | 1.27 (20%) :x: | 1.33 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 1.09 (30%)  | 1.02 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 1.38 (30%) :x: | 1.31 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 100)"]` | 1.37 (30%) :x: | 1.19 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 1000)"]` | 1.01 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 1.20 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.04 (30%)  | 1.03 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 1.02 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"integer\", 10000)"]` | 2.40 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 0.99 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"logical\", 10000)"]` | 1.06 (30%)  | 1.03 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"logical\", 100000)"]` | 1.00 (30%)  | 0.99 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", \"Array{Union{Nothing, BigInt},1}\")"]` | 0.99 (15%)  | 0.99 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

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
- `["find"]`
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
- `["scalar", "cos"]`
- `["scalar", "cosh"]`
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
- `["string"]`
- `["string", "readuntil"]`
- `["string", "search"]`
- `["string", "searchindex"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3185
Commit f3d6132 (2017-12-26 02:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110155737 s          0 s   19423291 s  4847648914 s        100 s
       #2  3501 MHz  466672618 s          0 s   12339616 s  4509901941 s         24 s
       #3  3501 MHz   92173670 s          0 s   10533479 s  4886699623 s         84 s
       #4  3501 MHz   88244352 s          0 s   10724862 s  4890433437 s         21 s
       
  Memory: 31.383651733398438 GB (3994.140625 MB free)
  Uptime: 4.9917841e7 sec
  Load Avg:  0.96923828125  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
