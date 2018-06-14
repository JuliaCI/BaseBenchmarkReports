# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b68efd34e7e3827c1c63d92d3551b57ab90ec378](https://github.com/JuliaLang/julia/commit/b68efd34e7e3827c1c63d92d3551b57ab90ec378) vs [JuliaLang/julia@0658a119725d7347513b4cc7e1111d961cd7eb51](https://github.com/JuliaLang/julia/commit/0658a119725d7347513b4cc7e1111d961cd7eb51)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b68efd34e7e3827c1c63d92d3551b57ab90ec378#commitcomment-29355867)

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
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"first\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"specified\")"]` | 1.69 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 3.24 (15%) :x: | 1.00 (1%)  |
| `["problem", "fem", "sparse_fem"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 2.03 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Float64}\")"]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"positive argument\", \"Float64\")"]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 7.88 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 8.35 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4095)"]` | 3.33 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4096)"]` | 3.42 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4095)"]` | 6.85 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 7.10 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4095)"]` | 1.55 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4096)"]` | 1.54 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 1.91 (20%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 1.99 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-alpha.122
Commit b68efd3 (2018-06-13 22:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   11859179 s        256 s    2110612 s  660966020 s          5 s
       #2  3501 MHz   58517711 s          0 s     969390 s  616755306 s          4 s
       #3  3501 MHz    8051920 s       2388 s    1107091 s  667217463 s         10 s
       #4  3501 MHz    7799217 s          4 s     786194 s  668121863 s          2 s
       
  Memory: 31.383651733398438 GB (4216.90234375 MB free)
  Uptime: 6.769823e6 sec
  Load Avg:  1.02783203125  1.02490234375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.121
Commit 0658a11 (2018-06-13 15:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   12006786 s        256 s    2122788 s  661932718 s          5 s
       #2  3501 MHz   59550252 s          0 s     980798 s  616841224 s          4 s
       #3  3501 MHz    8165043 s       2388 s    1116044 s  668224489 s         10 s
       #4  3501 MHz    7917499 s          4 s     794714 s  669124999 s          2 s
       
  Memory: 31.383651733398438 GB (4577.37890625 MB free)
  Uptime: 6.781129e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
