# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@055f6c287b232e611d9fe06ce6e6b0b9201f0c53](https://github.com/JuliaLang/julia/commit/055f6c287b232e611d9fe06ce6e6b0b9201f0c53) vs [JuliaLang/julia@933e3448ce69aa5074651eead126d7f20adc1edf](https://github.com/JuliaLang/julia/commit/933e3448ce69aa5074651eead126d7f20adc1edf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27857#issuecomment-401516193)

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
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 0.02 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 0.02 (25%) :white_check_mark: | 0.86 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.03 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.03 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 4.09 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 4.05 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"Set\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.17 (15%) :x: | Inf (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.52 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.84 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.83 (15%) :white_check_mark: | 0.53 (1%) :white_check_mark: |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.90 (15%)  | 1.50 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.42 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.96 (15%)  | 1.50 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.23 (15%) :x: | Inf (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.36 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.39 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.82 (15%) :white_check_mark: | 0.53 (1%) :white_check_mark: |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.94 (15%)  | 1.50 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.40 (15%) :x: | 0.98 (1%) :white_check_mark: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 1.01 (15%)  | 1.50 (1%) :x: |
| `["micro", "parseint"]` | 1.31 (15%) :x: | 1.01 (1%)  |
| `["misc", "parse", "Int"]` | 1.16 (15%) :x: | 1.01 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.09 (15%)  | 1.01 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.10 (15%)  | 1.01 (1%) :x: |
| `["problem", "fem", "sparse_fem"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 1.02 (15%)  | 1.04 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem", "spellcheck", "spellcheck"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 1.54 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.52 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 1.47 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 0.72 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 0.58 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.61 (40%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "backtracking"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "barbarian backtrack"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1"]` | 1.58 (15%) :x: | 1.40 (1%) :x: |
| `["string", "readuntil", "target length 1000"]` | 1.51 (15%) :x: | 1.57 (1%) :x: |
| `["string", "readuntil", "target length 2"]` | 1.69 (15%) :x: | 1.57 (1%) :x: |
| `["string", "readuntil", "target length 50000"]` | 1.51 (15%) :x: | 1.57 (1%) :x: |
| `["string", "replace"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (2, 2))"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 1.00 (15%)  | 1.03 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 1.00 (15%)  | 1.03 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 0.93 (15%)  | 1.05 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 0.97 (15%)  | 1.15 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.01 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.00 (15%)  | 1.15 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.01 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Int64, false)"]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta.100
Commit 055f6c2 (2018-06-30 04:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   20467464 s        259 s    2968811 s  791720237 s          5 s
       #2  3501 MHz  102319381 s          0 s    1605233 s  712873540 s          6 s
       #3  3501 MHz   14953269 s       2389 s    1686792 s  800287170 s         12 s
       #4  3501 MHz   14356292 s          4 s    1314111 s  801638428 s          4 s
       
  Memory: 31.383651733398438 GB (4995.9765625 MB free)
  Uptime: 8.176714e6 sec
  Load Avg:  1.2431640625  1.064453125  1.0615234375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.98
Commit 933e344 (2018-06-30 04:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   20606420 s        259 s    2980222 s  792532658 s          5 s
       #2  3501 MHz  103194100 s          0 s    1616775 s  712952517 s          6 s
       #3  3501 MHz   15066803 s       2389 s    1695660 s  801130160 s         12 s
       #4  3501 MHz   14476431 s          4 s    1322568 s  802475427 s          4 s
       
  Memory: 31.383651733398438 GB (4779.08984375 MB free)
  Uptime: 8.186378e6 sec
  Load Avg:  1.01806640625  1.02490234375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
