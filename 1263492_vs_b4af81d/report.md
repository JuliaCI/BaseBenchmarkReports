# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@12634929d161243300d546929c8e754926f2632b](https://github.com/JuliaLang/julia/commit/12634929d161243300d546929c8e754926f2632b) vs [JuliaLang/julia@b4af81d347c306de7469213ac5dab047c688b651](https://github.com/JuliaLang/julia/commit/b4af81d347c306de7469213ac5dab047c688b651)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26435#issuecomment-374321319)

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
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_fill!"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"UnitRange{Int64}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float64,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 1.00 (15%)  | 1.10 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 1.00 (15%)  | 1.13 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 2.29 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.57 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 1.86 (15%) :x: | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"big\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["io", "read", "readstring"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.48 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.48 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "splatting", "(3, 3, 3)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.19 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.4639
Commit 1263492 (2018-03-19 18:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  111929722 s          0 s   17474703 s  5571228269 s        292 s
       #2  3501 MHz  456848131 s          0 s   18462952 s  5229013802 s         90 s
       #3  3501 MHz   88339196 s          0 s   10078043 s  5613431543 s        134 s
       #4  3501 MHz   83482803 s          0 s   10091526 s  5618662293 s         54 s
       
  Memory: 31.383651733398438 GB (5244.375 MB free)
  Uptime: 5.7140867e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4636
Commit b4af81d (2018-03-19 17:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  112022155 s          0 s   17485480 s  5572074525 s        292 s
       #2  3501 MHz  457726195 s          0 s   18473620 s  5229076556 s         90 s
       #3  3501 MHz   88430710 s          0 s   10086470 s  5614283955 s        134 s
       #4  3501 MHz   83583374 s          0 s   10099782 s  5619506063 s         54 s
       
  Memory: 31.383651733398438 GB (5334.40234375 MB free)
  Uptime: 5.71504e7 sec
  Load Avg:  1.03564453125  1.0263671875  1.0458984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
