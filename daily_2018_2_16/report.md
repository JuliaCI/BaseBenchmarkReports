# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d7e723ddee6386b9c71e2356e5c0b3b2aa4dffb1](https://github.com/JuliaLang/julia/commit/d7e723ddee6386b9c71e2356e5c0b3b2aa4dffb1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/d7e723ddee6386b9c71e2356e5c0b3b2aa4dffb1#commitcomment-27598348)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-02-16 vs 2018-02-15

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
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcartesian_view\", \"1:100000\")"]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"next\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"push!\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Minute\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Month\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Bool\")"]` | 1.50 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float32\")"]` | 1.88 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{Float32}\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 100)"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3994
Commit d7e723d (2018-02-16 04:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  118585948 s          0 s   20937898 s  5285707255 s        103 s
       #2  3501 MHz  522186449 s          0 s   13174467 s  4902684911 s         26 s
       #3  3501 MHz   98356550 s          0 s   11212568 s  5329016751 s         86 s
       #4  3501 MHz   94091652 s          0 s   11403568 s  5333081365 s         23 s
       
  Memory: 31.383651733398438 GB (5640.1640625 MB free)
  Uptime: 5.4411452e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
