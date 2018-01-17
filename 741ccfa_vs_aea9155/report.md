# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@741ccfa9a3d407782e00816da3798ec29904f077](https://github.com/JuliaLang/julia/commit/741ccfa9a3d407782e00816da3798ec29904f077) vs [JuliaLang/julia@aea91558d3b60bf6d2bcdbd608b369e28ffffc9f](https://github.com/JuliaLang/julia/commit/aea91558d3b60bf6d2bcdbd608b369e28ffffc9f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25496#issuecomment-358087762)

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
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 1.83 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"var\", \"Float64\")"]` | 23.92 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"var\", \"Int64\")"]` | 7.40 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"unspecified\")"]` | 1.71 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"specified\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"unspecified\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"new\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"overwrite\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"pop!\", \"unspecified\")"]` | 0.55 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 1.55 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 1.59 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"small\")"]` | 1.41 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 0.46 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.46 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.03 (15%)  | 1.14 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 4.53 (25%) :x: | 1.16 (1%) :x: |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 1.49 (25%) :x: | 1.06 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967297)\")"]` | 1.69 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float64\")"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 2.60 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "floatexp", "(\"frexp\", \"subnorm\", \"Float32\")"]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 0.99 (30%)  | Inf (1%) :x: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 1.04 (30%)  | Inf (1%) :x: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 1.01 (30%)  | Inf (1%) :x: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 1.00 (30%)  | Inf (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.01 (30%)  | 5.00 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 1.00 (30%)  | 5.00 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.01 (30%)  | 2.33 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 1.06 (30%)  | 2.33 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.00 (30%)  | 8.00 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 1.02 (30%)  | 8.00 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 1.01 (30%)  | 3.33 (1%) :x: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 1.06 (30%)  | 3.33 (1%) :x: |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 6.15 (30%) :x: | Inf (1%) :x: |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 1.09 (30%)  | Inf (1%) :x: |
| `["sort", "issorted", "(\"reverse\", \"ones\")"]` | 1.02 (30%)  | Inf (1%) :x: |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 6.51 (30%) :x: | Inf (1%) :x: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ascending\")"]` | 0.89 (30%)  | Inf (1%) :x: |
| `["sort", "quicksort", "(\"sort! reverse\", \"descending\")"]` | 0.91 (30%)  | Inf (1%) :x: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ones\")"]` | 1.00 (30%)  | Inf (1%) :x: |
| `["sort", "quicksort", "(\"sort! reverse\", \"random\")"]` | 1.00 (30%)  | Inf (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.00 (30%)  | 5.00 (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"descending\")"]` | 1.00 (30%)  | 5.00 (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 1.00 (30%)  | 2.33 (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 1.02 (30%)  | 2.33 (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.00 (30%)  | 8.00 (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"descending\")"]` | 1.00 (30%)  | 8.00 (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 1.00 (30%)  | 3.33 (1%) :x: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 1.02 (30%)  | 3.33 (1%) :x: |
| `["union", "array", "(\"perf_countequals\", \"Union{Nothing, Bool}Union{Nothing, Bool}\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3425
Commit 741ccfa (2018-01-16 19:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  113930105 s          0 s   20071471 s  5029829067 s        100 s
       #2  3501 MHz  483881550 s          0 s   12614482 s  4679498892 s         24 s
       #3  3501 MHz   94050389 s          0 s   10747361 s  5071711351 s         84 s
       #4  3501 MHz   90046452 s          0 s   10947909 s  5075502638 s         21 s
       
  Memory: 31.383651733398438 GB (4621.515625 MB free)
  Uptime: 5.1789499e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3420
Commit aea9155 (2018-01-16 17:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  114043345 s          0 s   20081897 s  5030665146 s        100 s
       #2  3501 MHz  484767804 s          0 s   12624769 s  4679565019 s         24 s
       #3  3501 MHz   94139802 s          0 s   10755318 s  5072576514 s         84 s
       #4  3501 MHz   90127747 s          0 s   10955704 s  5076376294 s         21 s
       
  Memory: 31.383651733398438 GB (4252.5234375 MB free)
  Uptime: 5.1799132e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
