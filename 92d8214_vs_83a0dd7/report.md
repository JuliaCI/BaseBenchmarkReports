# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@92d82148418e45bbfbf8c7205509e4ebee62d14b](https://github.com/JuliaLang/julia/commit/92d82148418e45bbfbf8c7205509e4ebee62d14b) vs [JuliaLang/julia@83a0dd79cd39ff2f62c6f353f6daa7110a73d2c4](https://github.com/JuliaLang/julia/commit/83a0dd79cd39ff2f62c6f353f6daa7110a73d2c4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27495#issuecomment-396421468)

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
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3darray\")"]` | 7.15 (50%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 6.83 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 7.09 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 5.44 (15%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 6.87 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 5.69 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 4.02 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 3.52 (15%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"in\", \"false\")"]` | 1.61 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 1.45 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"<\", \"Set\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["dates", "accessor", "hour"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 2.34 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 3.12 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 1024)"]` | 2.26 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 256)"]` | 3.07 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 2.31 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 3.12 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 2.35 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 3.08 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 1024)"]` | 2.36 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 256)"]` | 3.17 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 2.36 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 3.14 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.43 (45%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int16\", \"1:1\")"]` | 1.78 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:1)\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967295)\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967297)\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int16\", \"RangeGenerator(1:1)\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float32\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float32\")"]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float32\")"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float32\")"]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float32\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.54 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-alpha.82
Commit 92d8214 (2018-06-11 21:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   10125712 s        256 s    1949287 s  646556683 s          5 s
       #2  3501 MHz   47399152 s          0 s     823188 s  611660919 s          4 s
       #3  3501 MHz    6478437 s       2388 s     980048 s  652565670 s          9 s
       #4  3501 MHz    6268860 s          4 s     665238 s  653414452 s          2 s
       
  Memory: 31.383651733398438 GB (1546.36328125 MB free)
  Uptime: 6.606123e6 sec
  Load Avg:  0.97412109375  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.79
Commit 83a0dd7 (2018-06-11 21:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   10253100 s        256 s    1961538 s  647546161 s          5 s
       #2  3501 MHz   48463118 s          0 s     834244 s  611719208 s          4 s
       #3  3501 MHz    6592090 s       2388 s     989112 s  653575515 s          9 s
       #4  3501 MHz    6380883 s          4 s     674353 s  654426236 s          2 s
       
  Memory: 31.383651733398438 GB (3253.79296875 MB free)
  Uptime: 6.617463e6 sec
  Load Avg:  0.9814453125  1.0126953125  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
