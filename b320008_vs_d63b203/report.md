# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b320008dc50c173d48c4de0fd7db14def5a79bfa](https://github.com/JuliaLang/julia/commit/b320008dc50c173d48c4de0fd7db14def5a79bfa) vs [JuliaLang/julia@d63b2033040e9df12ba94cafbed03bb63a115a52](https://github.com/JuliaLang/julia/commit/d63b2033040e9df12ba94cafbed03bb63a115a52)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26775#issuecomment-381049496)

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
| `["array", "accumulate", "(\"accumulate!\", \"Float64\")"]` | 2.43 (15%) :x: | Inf (1%) :x: |
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 4.15 (15%) :x: | Inf (1%) :x: |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 3.15 (15%) :x: | Inf (1%) :x: |
| `["array", "accumulate", "(\"cumsum\", \"Float64\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 2.98 (15%) :x: | 2.00 (1%) :x: |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Int64\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.09 (15%)  | Inf (1%) :x: |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.77 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 57.41 (15%) :x: | Inf (1%) :x: |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 76.55 (15%) :x: | Inf (1%) :x: |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 16.42 (15%) :x: | Inf (1%) :x: |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 9.68 (15%) :x: | Inf (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 4.63 (15%) :x: | Inf (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 4.39 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 4.98 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 3.83 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 1.32 (15%) :x: | 2.51 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 4.08 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.17 (15%) :x: | 1.78 (1%) :x: |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 58.80 (15%) :x: | Inf (1%) :x: |
| `["find", "findprev", "(\"BitArray{1}\", \"10-90\")"]` | 74.55 (15%) :x: | Inf (1%) :x: |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 17.03 (15%) :x: | Inf (1%) :x: |
| `["find", "findprev", "(\"BitArray{1}\", \"90-10\")"]` | 10.25 (15%) :x: | Inf (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 4.36 (15%) :x: | Inf (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 4.42 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 4.96 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 3.89 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 1.30 (15%) :x: | 2.51 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 4.40 (15%) :x: | 1.76 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.15 (15%)  | 1.78 (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 1024)"]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 256)"]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 1024)"]` | 1.51 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 256)"]` | 1.50 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 1024)"]` | 4.48 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 256)"]` | 4.64 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 1024)"]` | 4.52 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 256)"]` | 4.83 (45%) :x: | Inf (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 0.99 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 1.00 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 0.99 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 1.01 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 1.01 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 1.01 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 1.01 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 1.00 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Dict\")"]` | 1.00 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 1.03 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Dict\")"]` | 0.99 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 1.00 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Vector\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Vector\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Vector\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Vector\")"]` | 0.49 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigInt\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 1.68 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 1.75 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isless\", \"BigInt\")"]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.4872
Commit b320008 (2018-04-13 06:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    2351820 s        256 s     347514 s  141493796 s          1 s
       #2  3501 MHz   20043037 s          0 s     307984 s  124048779 s          0 s
       #3  3501 MHz    2315751 s       2368 s     245930 s  141660006 s          2 s
       #4  3501 MHz    2221185 s          0 s     328586 s  141779992 s          1 s
       
  Memory: 31.383651733398438 GB (20225.13671875 MB free)
  Uptime: 1.444955e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4870
Commit d63b203 (2018-04-13 02:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    2449912 s        256 s     357522 s  142274737 s          1 s
       #2  3501 MHz   20855085 s          0 s     317580 s  124118922 s          0 s
       #3  3501 MHz    2402493 s       2368 s     253492 s  142456619 s          2 s
       #4  3501 MHz    2326577 s          0 s     336174 s  142558662 s          1 s
       
  Memory: 31.383651733398438 GB (19839.15234375 MB free)
  Uptime: 1.453878e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
