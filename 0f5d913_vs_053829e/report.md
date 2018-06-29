# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0f5d913cd8999ae76a8bdd14f7b849ca049b6725](https://github.com/JuliaLang/julia/commit/0f5d913cd8999ae76a8bdd14f7b849ca049b6725) vs [JuliaLang/julia@053829ec8e7e01ee8a31954ec1e0705ead6c1d25](https://github.com/JuliaLang/julia/commit/053829ec8e7e01ee8a31954ec1e0705ead6c1d25)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27857#issuecomment-401246608)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.57 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.30 (15%) :x: | 1.15 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 0.33 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 0.32 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 0.31 (50%) :white_check_mark: | 0.26 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.31 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.34 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.99 (50%)  | 0.98 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.32 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 0.33 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.00 (50%)  | 0.98 (1%) :white_check_mark: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 0.02 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 0.02 (25%) :white_check_mark: | 0.86 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.03 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"setindex!\", \"new\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.03 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 4.14 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 4.15 (25%) :x: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 1.40 (15%) :x: | 1.25 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 1.35 (15%) :x: | 1.13 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 1.38 (15%) :x: | 1.25 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "Date"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "DateTime"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 60.50 (15%) :x: | Inf (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 127.97 (15%) :x: | 10.99 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 129.89 (15%) :x: | 10.99 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 50.59 (15%) :x: | 5.69 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 6.90 (15%) :x: | 11.64 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 128.28 (15%) :x: | 10.99 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 7.77 (15%) :x: | 11.71 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 74.72 (15%) :x: | Inf (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 132.55 (15%) :x: | 10.99 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 165.38 (15%) :x: | 10.99 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 54.51 (15%) :x: | 5.69 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 7.79 (15%) :x: | 11.64 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 141.71 (15%) :x: | 10.99 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 8.88 (15%) :x: | 11.72 (1%) :x: |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "parse", "DateTime"]` | 1.16 (15%) :x: | 1.01 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.08 (15%)  | 1.01 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.08 (15%)  | 1.01 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 1.00 (15%)  | 1.05 (1%) :x: |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int64}\")"]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int64\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow1023\", \"positive argument\", Float64)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 0.59 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 1.73 (20%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "backtracking"]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "barbarian backtrack"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1"]` | 1.47 (15%) :x: | 1.40 (1%) :x: |
| `["string", "readuntil", "target length 1000"]` | 1.51 (15%) :x: | 1.57 (1%) :x: |
| `["string", "readuntil", "target length 2"]` | 1.61 (15%) :x: | 1.57 (1%) :x: |
| `["string", "readuntil", "target length 50000"]` | 1.51 (15%) :x: | 1.57 (1%) :x: |
| `["tuple", "linear algebra", "(\"matmat\", (8, 8), (8, 8))"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 1.01 (15%)  | 1.03 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 1.01 (15%)  | 1.03 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 0.99 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 0.97 (15%)  | 1.05 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 1.00 (15%)  | 1.15 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 1.00 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 0.99 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 1.03 (15%)  | 1.15 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 0.96 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 1.02 (15%)  | 1.04 (1%) :x: |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 1.19 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta.88
Commit 0f5d913 (2018-06-29 04:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   19748780 s        259 s    2910399 s  783706576 s          5 s
       #2  3501 MHz  100431289 s          0 s    1577808 s  705991908 s          6 s
       #3  3501 MHz   14696310 s       2389 s    1664730 s  791759127 s         12 s
       #4  3501 MHz   14132551 s          4 s    1292665 s  793075251 s          4 s
       
  Memory: 31.383651733398438 GB (5033.5546875 MB free)
  Uptime: 8.088586e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.86
Commit 053829e (2018-06-29 04:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   19872148 s        259 s    2921948 s  784542117 s          5 s
       #2  3501 MHz  101319190 s          0 s    1589384 s  706065268 s          6 s
       #3  3501 MHz   14824004 s       2389 s    1673718 s  792595558 s         12 s
       #4  3501 MHz   14247236 s          4 s    1301631 s  793924925 s          4 s
       
  Memory: 31.383651733398438 GB (4951.27734375 MB free)
  Uptime: 8.098325e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
