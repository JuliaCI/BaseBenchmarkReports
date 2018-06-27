# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@bf89ccef4b2ecf2fc3071e2e8a00b6296a1073c0](https://github.com/JuliaLang/julia/commit/bf89ccef4b2ecf2fc3071e2e8a00b6296a1073c0) vs [JuliaLang/julia@feb9260680fd5f271de9e188e66e043ff257360f](https://github.com/JuliaLang/julia/commit/feb9260680fd5f271de9e188e66e043ff257360f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27711#issuecomment-400398686)

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
| `["array", "cat", "(\"vcat\", 5)"]` | 1.80 (15%) :x: | 1.03 (1%) :x: |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"Array{Float32,2}\")"]` | 5.45 (50%) :x: | 1.84 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"Array{Int32,2}\")"]` | 5.31 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.34 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 1.29 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 5.59 (50%) :x: | 1.84 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 5.47 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 5.61 (50%) :x: | 1.84 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 5.24 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 1.70 (50%) :x: | 1.34 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.32 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 5.55 (50%) :x: | 1.84 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.28 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 34.26 (50%) :x: | 19.93 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 134.97 (50%) :x: | 48.33 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 5.51 (50%) :x: | 1.84 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 4.63 (50%) :x: | 1.84 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.31 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 5.26 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.34 (50%)  | 1.24 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 33.90 (50%) :x: | 21.31 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 142.36 (50%) :x: | 57.87 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 5.30 (50%) :x: | 1.85 (1%) :x: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 4.96 (50%) :x: | 1.85 (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Float64\")"]` | 63.98 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 93.16 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Float64\")"]` | 63.69 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 92.84 (15%) :x: | Inf (1%) :x: |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter!\")"]` | 1.36 (25%) :x: | 1.00 (1%)  |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"iterator\")"]` | 0.99 (25%)  | 1.04 (1%) :x: |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"iterator\")"]` | 1.00 (25%)  | 1.03 (1%) :x: |
| `["collection", "optimizations", "(\"BitSet\", \"Int8\")"]` | 1.00 (25%)  | 1.10 (1%) :x: |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"setindex!\", \"new\")"]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\")"]` | 1.03 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Set\")"]` | 0.99 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Vector\")"]` | 1.02 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Set\")"]` | 1.02 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Vector\")"]` | 1.04 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"Set\")"]` | 1.00 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"Vector\")"]` | 1.01 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\")"]` | 1.06 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.01 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.02 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 1.01 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.01 (25%)  | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.02 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.09 (25%)  | 1.17 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Set\")"]` | 1.07 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Vector\")"]` | 1.02 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\")"]` | 1.04 (25%)  | 1.05 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.02 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\")"]` | 1.18 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.13 (25%)  | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\")"]` | 1.02 (25%)  | 1.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.05 (25%)  | 1.07 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 1.00 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Set\")"]` | 0.99 (25%)  | Inf (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Vector\")"]` | 1.00 (25%)  | Inf (1%) :x: |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "exp2", "(\"very small\", \"negative argument\", \"Float32\")"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta.40
Commit bf89cce (2018-06-26 20:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   35669055 s        278 s    3735016 s  747487401 s          7 s
       #2  3501 MHz  163748080 s          0 s    2258413 s  622898964 s          4 s
       #3  3501 MHz   22003897 s       2377 s    1823280 s  764749153 s         11 s
       #4  3501 MHz   20554623 s          0 s    2100770 s  766064055 s          8 s
       
  Memory: 31.383651733398438 GB (5342.9921875 MB free)
  Uptime: 7.893742e6 sec
  Load Avg:  0.9697265625  1.01171875  1.04248046875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.33
Commit feb9260 (2018-06-26 17:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   35819404 s        278 s    3746486 s  748299833 s          7 s
       #2  3501 MHz  164624828 s          0 s    2269765 s  622987866 s          4 s
       #3  3501 MHz   22117580 s       2377 s    1832113 s  765602914 s         11 s
       #4  3501 MHz   20671078 s          0 s    2109874 s  766915566 s          8 s
       
  Memory: 31.383651733398438 GB (4480.17578125 MB free)
  Uptime: 7.90352e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
