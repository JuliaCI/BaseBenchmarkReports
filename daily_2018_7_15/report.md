# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a8c53e08e961cad86b391dac6b3c212417960d89](https://github.com/JuliaLang/julia/commit/a8c53e08e961cad86b391dac6b3c212417960d89)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a8c53e08e961cad86b391dac6b3c212417960d89#commitcomment-29711288)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-07-15 vs 2018-07-14

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"pop!\", \"unspecified\")"]` | 1.88 (25%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 3.91 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Vector\")"]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float64\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.22 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta2.11
Commit a8c53e0* (2018-07-15 03:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   42928659 s        279 s    4434419 s  896520579 s          9 s
       #2  3501 MHz  198464037 s          0 s    2865631 s  744847719 s          6 s
       #3  3501 MHz   28482856 s       2381 s    2335795 s  914959590 s         15 s
       #4  3501 MHz   26508788 s          0 s    2712269 s  916692865 s          9 s
       
  Memory: 31.383651733398438 GB (5022.3984375 MB free)
  Uptime: 9.467657e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
