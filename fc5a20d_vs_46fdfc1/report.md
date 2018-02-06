# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fc5a20d2442b873d6cfb5a8201653ac5a628cfcd](https://github.com/JuliaLang/julia/commit/fc5a20d2442b873d6cfb5a8201653ac5a628cfcd) vs [JuliaLang/julia@46fdfc1e426c3111b7e421f8403b90eef97ceb3d](https://github.com/JuliaLang/julia/commit/46fdfc1e426c3111b7e421f8403b90eef97ceb3d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25879#issuecomment-363314677)

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
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"pop!\")"]` | 1.45 (25%) :x: | 1.00 (1%)  |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"iterator\")"]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Minute\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.29 (15%) :white_check_mark: | 0.48 (1%) :white_check_mark: |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 2.59 (15%) :x: | 1.00 (1%)  |
| `["io", "read", "readstring"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["micro", "fib"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 0.82 (30%)  | 0.78 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 0.62 (30%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 0.49 (30%) :white_check_mark: | 0.74 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 0.77 (30%)  | 0.65 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"logical\", 100)"]` | 0.88 (30%)  | 0.81 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"logical\", 1000)"]` | 0.96 (30%)  | 0.94 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 0.90 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 0.71 (30%)  | 0.55 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.52 (30%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 0.47 (30%) :white_check_mark: | 0.52 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"logical\", 10000)"]` | 0.55 (30%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spvec\", \"logical\", 100000)"]` | 0.56 (30%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.41 (30%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3728
Commit fc5a20d (2018-02-06 05:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  108059424 s          0 s   16627397 s  5218392333 s        270 s
       #2  3501 MHz  432214264 s          0 s   17865287 s  4895669837 s         87 s
       #3  3501 MHz   85708003 s          0 s    9690786 s  5257640754 s        119 s
       #4  3501 MHz   80920416 s          0 s    9613356 s  5262943823 s         48 s
       
  Memory: 31.383651733398438 GB (5190.015625 MB free)
  Uptime: 5.3551554e7 sec
  Load Avg:  0.9716796875  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3726
Commit 46fdfc1 (2018-02-06 04:08 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  108157730 s          0 s   16639212 s  5219306699 s        270 s
       #2  3501 MHz  433165699 s          0 s   17876087 s  4895735101 s         87 s
       #3  3501 MHz   85794548 s          0 s    9698944 s  5258573463 s        119 s
       #4  3501 MHz   81023830 s          0 s    9621454 s  5263859961 s         48 s
       
  Memory: 31.383651733398438 GB (4422.79296875 MB free)
  Uptime: 5.3561838e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
