# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0146f7742cc94965e5f1f10117a8dd3392355692](https://github.com/JuliaLang/julia/commit/0146f7742cc94965e5f1f10117a8dd3392355692) vs [JuliaLang/julia@76fcbbcb0521ca9c03e7c01dce457f9ae5571dd7](https://github.com/JuliaLang/julia/commit/76fcbbcb0521ca9c03e7c01dce457f9ae5571dd7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25736#issuecomment-361018296)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"setindex!\")"]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"Vector\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 27.11 (15%) :x: | 8.23 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 23.97 (15%) :x: | 6.49 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 27.19 (15%) :x: | 8.23 (1%) :x: |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 2.45 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.45 (45%) :x: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 9.15 (15%) :x: | 7.71 (1%) :x: |
| `["problem", "spellcheck", "spellcheck"]` | 39.21 (15%) :x: | 11.76 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967297\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"UInt64\")"]` | 1.71 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 1.73 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 1.51 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["shootout", "k_nucleotide"]` | 5.39 (15%) :x: | 4.57 (1%) :x: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string", "join"]` | 1.51 (40%) :x: | 1.02 (1%) :x: |
| `["union", "array", "(\"perf_countnothing\", \"Array{Union{Nothing, BigFloat},1}\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", \"Array{Union{Nothing, Bool},1}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3603
Commit 0146f77 (2018-01-27 21:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  115808862 s          0 s   20398268 s  5123132059 s        101 s
       #2  3501 MHz  496667950 s          0 s   12807791 s  4762258139 s         25 s
       #3  3501 MHz   95590535 s          0 s   10919752 s  5165738431 s         86 s
       #4  3501 MHz   91464918 s          0 s   11104407 s  5169678244 s         22 s
       
  Memory: 31.383651733398438 GB (5656.265625 MB free)
  Uptime: 5.2747379e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3600
Commit 76fcbbc (2018-01-27 21:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  115897180 s          0 s   20409078 s  5123995263 s        101 s
       #2  3501 MHz  497560469 s          0 s   12817879 s  4762320730 s         25 s
       #3  3501 MHz   95674836 s          0 s   10927583 s  5166611387 s         86 s
       #4  3501 MHz   91572838 s          0 s   11112192 s  5170527913 s         22 s
       
  Memory: 31.383651733398438 GB (5372.94140625 MB free)
  Uptime: 5.2757038e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
