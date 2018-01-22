# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3bccded84d14bbfbbbdb345101738b593b0d894f](https://github.com/JuliaLang/julia/commit/3bccded84d14bbfbbbdb345101738b593b0d894f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3bccded84d14bbfbbbdb345101738b593b0d894f#commitcomment-27010546)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-01-22 vs 2018-01-18

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
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"getindex\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"specified\")"]` | 1.35 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"first\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 14.39 (15%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 11.53 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 16.74 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 16.04 (15%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svd\", \"UpperTriangular\", 1024)"]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svdfact\", \"LowerTriangular\", 1024)"]` | 1.78 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svdfact\", \"Matrix\", 1024)"]` | 1.49 (45%) :x: | 1.00 (1%)  |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.07 (15%)  | 1.02 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.08 (15%)  | 1.04 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.06 (15%)  | 1.01 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.08 (15%)  | 1.04 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.09 (15%)  | 1.03 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:170141183460469231731687303715884105728\")"]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float32\")"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"UInt64\")"]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 1.83 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 1.67 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 1.94 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 2.05 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 2.00 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 1.99 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.90 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 2.04 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 2.08 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 1.86 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 2.28 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 2.34 (50%) :x: | 1.00 (1%)  |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 2.42 (50%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 2.40 (40%) :x: | 1.00 (1%)  |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 2.32 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 1000)"]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", \"Array{Union{Nothing, BigFloat},1}\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3501
Commit 3bccded (2018-01-21 20:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  115227442 s          0 s   20258900 s  5074472140 s        100 s
       #2  3501 MHz  492826496 s          0 s   12733736 s  4716670606 s         24 s
       #3  3501 MHz   95033949 s          0 s   10842509 s  5116872244 s         85 s
       #4  3501 MHz   90906493 s          0 s   11041876 s  5120788967 s         22 s
       
  Memory: 31.383651733398438 GB (4989.140625 MB free)
  Uptime: 5.2252115e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
