# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@48d36ba3c95068f0c6909fe583899c392754c2a1](https://github.com/JuliaLang/julia/commit/48d36ba3c95068f0c6909fe583899c392754c2a1) vs [JuliaLang/julia@e4d4529552fe6a780a58fe1d5d8563ee727c43b2](https://github.com/JuliaLang/julia/commit/e4d4529552fe6a780a58fe1d5d8563ee727c43b2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25736#issuecomment-361014942)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 1.61 (25%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Minute\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 24.86 (15%) :x: | 8.23 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 22.36 (15%) :x: | 6.49 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 23.83 (15%) :x: | 8.23 (1%) :x: |
| `["dates", "string", "Date"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["io", "read", "readstring"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 8.93 (15%) :x: | 7.71 (1%) :x: |
| `["problem", "spellcheck", "spellcheck"]` | 38.98 (15%) :x: | 11.76 (1%) :x: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int16}\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int8}\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt8}\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float16\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "k_nucleotide"]` | 5.39 (15%) :x: | 4.57 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 2.25 (40%) :x: | 1.02 (1%) :x: |

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
Julia Version 0.7.0-DEV.3601
Commit 48d36ba (2018-01-27 20:59 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  106518744 s          0 s   16385458 s  5139610109 s        264 s
       #2  3501 MHz  417472050 s          0 s   17562712 s  4830109242 s         84 s
       #3  3501 MHz   84186521 s          0 s    9543404 s  5178582310 s        114 s
       #4  3501 MHz   79436391 s          0 s    9452531 s  5183860336 s         47 s
       
  Memory: 31.383651733398438 GB (4158.1796875 MB free)
  Uptime: 5.2744041e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3597
Commit e4d4529 (2018-01-27 17:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  106609415 s          0 s   16396266 s  5140465222 s        264 s
       #2  3501 MHz  418381148 s          0 s   17573655 s  4830148606 s         84 s
       #3  3501 MHz   84275568 s          0 s    9551739 s  5179444272 s        115 s
       #4  3501 MHz   79520677 s          0 s    9460970 s  5184727159 s         47 s
       
  Memory: 31.383651733398438 GB (3858.109375 MB free)
  Uptime: 5.2753644e7 sec
  Load Avg:  1.01220703125  1.02001953125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
