# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f59a8330104dbbf6c603715966a641b7cd273a87](https://github.com/JuliaLang/julia/commit/f59a8330104dbbf6c603715966a641b7cd273a87)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f59a8330104dbbf6c603715966a641b7cd273a87#commitcomment-28446108)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-04-06 vs 2018-04-05

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 1.02 (15%)  | 1.10 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 1.04 (15%)  | 1.14 (1%) :x: |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 1.09 (15%)  | 1.13 (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 1.35 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.14 (15%)  | Inf (1%) :x: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 1.13 (15%)  | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 1.90 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 0.57 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"small\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"BitSet\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.44 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"1 <= abs(x) < 2\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"one\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Float32\")"]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.58 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isless\", \"BigFloat\")"]` | 2.20 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.96 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.89 (15%)  | 0.00 (1%) :white_check_mark: |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 0.90 (15%)  | 0.00 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.4770
Commit f59a833 (2018-04-06 03:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    1327945 s        254 s     198732 s   81002605 s          0 s
       #2  3501 MHz   11648889 s          0 s     180664 s   70814182 s          0 s
       #3  3501 MHz    1383670 s       2368 s     139905 s   81037313 s          1 s
       #4  3501 MHz    1311213 s          0 s     193160 s   81099473 s          1 s
       
  Memory: 31.383651733398438 GB (20514.21484375 MB free)
  Uptime: 827042.0 sec
  Load Avg:  1.05419921875  1.02880859375  1.04833984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
