# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@e75cca57f84404572014c6cf8d4b4dc5b6f8c50e](https://github.com/pkofod/julia/commit/e75cca57f84404572014c6cf8d4b4dc5b6f8c50e) vs [JuliaLang/julia@a2e4f16a43eb76e4b464f0af03593f3d0d5ec59d](https://github.com/JuliaLang/julia/commit/a2e4f16a43eb76e4b464f0af03593f3d0d5ec59d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25948#issuecomment-365745701)

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
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((10000000,), 2)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\", \"sizehint!\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Second\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 256)"]` | 0.33 (45%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"'a':'z'\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Bool\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3989
Commit e75cca5 (2018-02-14 20:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  108857263 s          0 s   16796328 s  5291885635 s        273 s
       #2  3501 MHz  439439252 s          0 s   18044795 s  4962815343 s         88 s
       #3  3501 MHz   86407036 s          0 s    9788592 s  5331485191 s        122 s
       #4  3501 MHz   81666851 s          0 s    9721774 s  5336736641 s         50 s
       
  Memory: 31.383651733398438 GB (5582.20703125 MB free)
  Uptime: 5.4298269e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3979
Commit a2e4f16 (2018-02-14 20:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  108943131 s          0 s   16807518 s  5292712528 s        273 s
       #2  3501 MHz  440294243 s          0 s   18055361 s  4962876210 s         88 s
       #3  3501 MHz   86516573 s          0 s    9796947 s  5332294019 s        122 s
       #4  3501 MHz   81756312 s          0 s    9730110 s  5337565662 s         50 s
       
  Memory: 31.383651733398438 GB (5256.98828125 MB free)
  Uptime: 5.4307545e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
