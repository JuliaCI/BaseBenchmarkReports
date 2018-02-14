# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c37e21c5b439b1c01e288384c6053a24ab6e9950](https://github.com/JuliaLang/julia/commit/c37e21c5b439b1c01e288384c6053a24ab6e9950) vs [JuliaLang/julia@160a46704fd1b349b5425f104a4ac8b323ea85af](https://github.com/JuliaLang/julia/commit/160a46704fd1b349b5425f104a4ac8b323ea85af)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25890#issuecomment-365454824)

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
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 2.10 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 2.27 (15%) :x: | 6.38 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 5.76 (15%) :x: | 6.95 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 7.35 (15%) :x: | 6.78 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 5.58 (15%) :x: | 6.89 (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 3.59 (15%) :x: | 1.00 (1%)  |
| `["micro", "fib"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 9.82 (15%) :x: | 23.00 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 5.70 (15%) :x: | 4104.99 (1%) :x: |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.09 (15%)  | 84.33 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Bool\", \"RangeGenerator(true:true)\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt8\", \"RangeGenerator(1:1)\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"one\", \"Float64\")"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"+\")"]` | 1.55 (40%) :x: | 1.00 (1%)  |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"-\")"]` | 1.58 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "k_nucleotide"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 4.64 (15%) :x: | 25.67 (1%) :x: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.64 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["string", "join"]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.3970
Commit c37e21c (2018-02-14 00:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  118090489 s          0 s   20858480 s  5267666318 s        102 s
       #2  3501 MHz  517967017 s          0 s   13119588 s  4888281893 s         26 s
       #3  3501 MHz   97876161 s          0 s   11160047 s  5310871422 s         86 s
       #4  3501 MHz   93646806 s          0 s   11360222 s  5314889432 s         22 s
       
  Memory: 31.383651733398438 GB (5656.55078125 MB free)
  Uptime: 5.4224584e7 sec
  Load Avg:  1.0341796875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3962
Commit 160a467 (2018-02-13 23:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  118180520 s          0 s   20868677 s  5268484980 s        102 s
       #2  3501 MHz  518813910 s          0 s   13129597 s  4888346644 s         26 s
       #3  3501 MHz   97984340 s          0 s   11167861 s  5311677142 s         86 s
       #4  3501 MHz   93730616 s          0 s   11368208 s  5315719495 s         22 s
       
  Memory: 31.383651733398438 GB (5374.55078125 MB free)
  Uptime: 5.4233808e7 sec
  Load Avg:  1.01220703125  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
