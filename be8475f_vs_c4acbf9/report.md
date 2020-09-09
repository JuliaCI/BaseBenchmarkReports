# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@be8475f41a8c97c08a551d49fc2375fcc7825900](https://github.com/JuliaLang/julia/commit/be8475f41a8c97c08a551d49fc2375fcc7825900) vs [JuliaLang/julia@c4acbf93fbdd0ad113559992323336271d8c6b81](https://github.com/JuliaLang/julia/commit/c4acbf93fbdd0ad113559992323336271d8c6b81)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/37210#issuecomment-689410445)

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
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"BitArray\")"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 8)"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 8)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 256)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "26942"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["dates", "string", "DateTime"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"50-50\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 0.39 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 256)"]` | 2.54 (45%) :x: | 1.00 (1%)  |
| `["linalg", "small exp #29116"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "20517"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["misc", "allocation elision view", "conditional"]` | 0.65 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "allocation elision view", "no conditional"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "iterators", "zip(1:1, 1:1, 1:1)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["misc", "parse", "Float64"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 24, 1)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_devec"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["problem", "ziggurat", "ziggurat"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"UInt64\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigInt\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float64\")"]` | 1.38 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float32\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.19 (5%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float32\")"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"zero\", \"Float32\")"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["string", "repeat", "repeat char 2"]` | 1.76 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 1.56 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 0.85 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 1.63 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.31 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 1.37 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.42 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.73 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.68 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Nothing, Int8}, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |

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
- `["broadcast"]`
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
- `["io", "array_limit"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["io"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`
- `["micro"]`
- `["misc"]`
- `["misc", "23042"]`
- `["misc", "afoldl"]`
- `["misc", "allocation elision view"]`
- `["misc", "bitshift"]`
- `["misc", "issue 12165"]`
- `["misc", "iterators"]`
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
- `["sparse", "sparse matvec"]`
- `["sparse", "sparse solves"]`
- `["sparse", "transpose"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["string", "repeat"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "misc"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.5.2-pre.25
Commit be8475f (2020-09-09 06:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  158356681 s       5069 s   17521753 s  7556133283 s         39 s
       #2  3501 MHz  1205430769 s        220 s   24538759 s  6512655762 s         29 s
       #3  3501 MHz  143942698 s       3325 s   10606879 s  7586726807 s         40 s
       #4  3501 MHz  134667099 s         43 s   15488461 s  7589429017 s         28 s
       
  Memory: 31.383651733398438 GB (14543.1171875 MB free)
  Uptime: 7.7486429e7 sec
  Load Avg:  1.01318359375  1.0205078125  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.5.2-pre.0
Commit c4acbf9 (2020-08-26 10:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  158504862 s       5069 s   17531781 s  7557336499 s         39 s
       #2  3501 MHz  1206689874 s        220 s   24565747 s  6512734284 s         29 s
       #3  3501 MHz  144097048 s       3325 s   10613386 s  7587929014 s         40 s
       #4  3501 MHz  134818682 s         43 s   15495023 s  7590634274 s         28 s
       
  Memory: 31.383651733398438 GB (14132.1640625 MB free)
  Uptime: 7.7500078e7 sec
  Load Avg:  0.9970703125  1.01416015625  1.044921875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
