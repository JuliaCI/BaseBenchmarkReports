# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@43a3886a78c5f8c463af50db64255c3771beeceb](https://github.com/JuliaLang/julia/commit/43a3886a78c5f8c463af50db64255c3771beeceb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/43a3886a78c5f8c463af50db64255c3771beeceb#commitcomment-29043883)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-05-19 vs 2018-05-18

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
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"in\", \"true\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"big\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 0.43 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Float64\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"Float64\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float32\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "regex_dna"]` | 80.16 (15%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.5133
Commit 43a3886 (2018-05-19 01:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   15577310 s        265 s    1790658 s  435844489 s          4 s
       #2  3501 MHz   97753280 s          0 s    1404781 s  354930094 s          3 s
       #3  3501 MHz   13035694 s       2373 s    1135259 s  439598590 s          8 s
       #4  3501 MHz   12334842 s          0 s    1339540 s  440266874 s          3 s
       
  Memory: 31.383651733398438 GB (4345.2890625 MB free)
  Uptime: 4.543968e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
