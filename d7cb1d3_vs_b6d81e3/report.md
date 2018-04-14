# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d7cb1d314230b9e07d940615071c1243303d577d](https://github.com/JuliaLang/julia/commit/d7cb1d314230b9e07d940615071c1243303d577d) vs [JuliaLang/julia@b6d81e36bb150dca75755bad3a49c038e1630ea4](https://github.com/JuliaLang/julia/commit/b6d81e36bb150dca75755bad3a49c038e1630ea4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26784#issuecomment-381302170)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 0.96 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 0.93 (15%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int8\")"]` | 1.80 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float16\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "acosh", "(\"one\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"zero\", \"Float32\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{UInt64}\")"]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 1.62 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isequal\", \"Float32\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 1.31 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.4885
Commit d7cb1d3 (2018-04-14 03:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    1574092 s        239 s     292903 s  149740089 s          2 s
       #2  3501 MHz   12498450 s          0 s     253472 s  138903802 s          2 s
       #3  3501 MHz    1615055 s       2385 s     288596 s  149789228 s          4 s
       #4  3501 MHz    1519704 s          2 s     202883 s  150090315 s          0 s
       
  Memory: 31.383651733398438 GB (17679.54296875 MB free)
  Uptime: 1.519108e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4881
Commit b6d81e3 (2018-04-13 22:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz    1667069 s        239 s     302875 s  150508313 s          2 s
       #2  3501 MHz   13301569 s          0 s     263019 s  138964485 s          2 s
       #3  3501 MHz    1715808 s       2385 s     296030 s  150554678 s          4 s
       #4  3501 MHz    1605978 s          2 s     210279 s  150870370 s          0 s
       
  Memory: 31.383651733398438 GB (17255.734375 MB free)
  Uptime: 1.527851e6 sec
  Load Avg:  1.009765625  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
