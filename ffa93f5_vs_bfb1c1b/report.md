# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ffa93f5f08fba3d54da92d71f3403f036d001e89](https://github.com/JuliaLang/julia/commit/ffa93f5f08fba3d54da92d71f3403f036d001e89) vs [JuliaLang/julia@bfb1c1b91d38bfc222660d22b8500c2016051633](https://github.com/JuliaLang/julia/commit/bfb1c1b91d38bfc222660d22b8500c2016051633)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26775#issuecomment-386850085)

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
| `["array", "accumulate", "(\"accumulate!\", \"Float64\")"]` | 1.87 (15%) :x: | Inf (1%) :x: |
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 2.72 (15%) :x: | Inf (1%) :x: |
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 3.26 (15%) :x: | Inf (1%) :x: |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 2.18 (15%) :x: | 2.00 (1%) :x: |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"getindex\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 1024)"]` | 2.73 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 256)"]` | 3.83 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 1024)"]` | 3.44 (45%) :x: | Inf (1%) :x: |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 256)"]` | 3.99 (45%) :x: | Inf (1%) :x: |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 0.99 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 0.97 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 0.99 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 0.97 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 0.96 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 1.01 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 0.98 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 1.02 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Dict\")"]` | 1.16 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 0.98 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Dict\")"]` | 1.13 (25%)  | 1.33 (1%) :x: |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 0.99 (25%)  | 1.25 (1%) :x: |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"'a':'z'\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Vector\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Vector\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Vector\")"]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Vector\")"]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 1.74 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 1.48 (40%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{Float32}\")"]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"positive argument\", \"Float32\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"2f0^-12 <= abs(x) < 1f0\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Commit ffa93f5 (2018-05-06 02:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    9139498 s        261 s    1159746 s  330452398 s          4 s
       #2  3501 MHz   55046340 s          0 s     804618 s  285494574 s          1 s
       #3  3501 MHz    6416240 s       2371 s     640265 s  333996385 s          6 s
       #4  3501 MHz    6216707 s          0 s     802450 s  334229555 s          1 s
       
  Memory: 31.383651733398438 GB (5767.6953125 MB free)
  Uptime: 3.415834e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.5021
Commit bfb1c1b (2018-05-06 00:40 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    9283594 s        261 s    1171166 s  331285961 s          4 s
       #2  3501 MHz   55951308 s          0 s     815280 s  285570838 s          1 s
       #3  3501 MHz    6532017 s       2371 s     649317 s  334862932 s          6 s
       #4  3501 MHz    6327399 s          0 s     811405 s  335101872 s          1 s
       
  Memory: 31.383651733398438 GB (5852.4765625 MB free)
  Uptime: 3.42576e6 sec
  Load Avg:  1.01123046875  1.01953125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
