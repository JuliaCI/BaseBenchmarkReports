# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a5209a6a7a64bb0254ddf0c6845c201efd11cf98](https://github.com/JuliaLang/julia/commit/a5209a6a7a64bb0254ddf0c6845c201efd11cf98) vs [JuliaLang/julia@91c1af8d9a2116191e0f933061f35da852bab716](https://github.com/JuliaLang/julia/commit/91c1af8d9a2116191e0f933061f35da852bab716)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25818#issuecomment-361704548)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"==\", \"BitSet\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"==\", \"self\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"Vector\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"empty\", \"Int\", \"<\", \"BitSet\")"]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["find", "(\"BitArray{1}\", \"10-90\")"]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 1.44 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{UInt64}\")"]` | 2.03 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 2.03 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.03 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 2.05 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 1.98 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 2.02 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigInt\")"]` | 1.96 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 2.02 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigInt}\")"]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigInt\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.93 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"UInt64\")"]` | 1.82 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 1.88 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 1.69 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 2.34 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 2.36 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.41 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 2.16 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 2.35 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.65 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 1.47 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 1.67 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 2.37 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 2.37 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", \"Array{Union{Nothing, BigFloat},1}\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", \"Array{Union{Nothing, Complex{Float64}},1}\")"]` | 0.99 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", \"Array{Union{Nothing, Float32},1}\")"]` | 0.86 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", \"Array{Union{Nothing, Float64},1}\")"]` | 0.93 (15%)  | 0.00 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.3668
Commit a5209a6 (2018-01-30 19:18 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  116186013 s          0 s   20475925 s  5147499881 s        101 s
       #2  3501 MHz  500233527 s          0 s   12860640 s  4783518077 s         25 s
       #3  3501 MHz   95944537 s          0 s   10957174 s  5190232277 s         86 s
       #4  3501 MHz   91849157 s          0 s   11149559 s  5194128150 s         22 s
       
  Memory: 31.383651733398438 GB (4880.0625 MB free)
  Uptime: 5.2996312e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3661
Commit 91c1af8 (2018-01-30 17:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  116276452 s          0 s   20486664 s  5148344777 s        101 s
       #2  3501 MHz  501132325 s          0 s   12870764 s  4783558220 s         25 s
       #3  3501 MHz   96029193 s          0 s   10964911 s  5191088737 s         86 s
       #4  3501 MHz   91931797 s          0 s   11157438 s  5194986675 s         22 s
       
  Memory: 31.383651733398438 GB (4985.9140625 MB free)
  Uptime: 5.3005808e7 sec
  Load Avg:  0.93505859375  1.0048828125  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
