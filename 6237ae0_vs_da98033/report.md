# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6237ae022add7d0ec6866a2176105f06eb54fcc9](https://github.com/JuliaLang/julia/commit/6237ae022add7d0ec6866a2176105f06eb54fcc9) vs [JuliaLang/julia@da98033388f8519606452550fc83daecb4e0d180](https://github.com/JuliaLang/julia/commit/da98033388f8519606452550fc83daecb4e0d180)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25890#issuecomment-367754076)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_fill!"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "boolarray_true_fill!"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 7.98 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 8.68 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 8.11 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 7.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 8.62 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 8.31 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"BitArray{2}\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.07 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 7.88 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 7.61 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 5.90 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 8.13 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 7.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.01 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.57 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.40 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 6.70 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 7.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 7.07 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 8.36 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 7.35 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 8.33 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 4.63 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 8.04 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.47 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 4.34 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.58 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.96 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 3.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 3.80 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 3.33 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 3.83 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 3.97 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 4.11 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 3.44 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.94 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 4.37 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 3.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.78 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.42 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "2d"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.04 (15%)  | 1.14 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.03 (15%)  | 1.01 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.04 (15%)  | 1.05 (1%) :x: |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.04 (15%)  | 1.02 (1%) :x: |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 2.65 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 2.47 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.46 (45%) :x: | 1.00 (1%)  |
| `["micro", "parseint"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 1.40 (15%) :x: | 2.06 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 5.89 (15%) :x: | 3857.59 (1%) :x: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Bool\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.49 (30%) :x: | 1.00 (1%)  |
| `["string", "findfirst", "String"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.4071
Commit 6237ae0 (2018-02-22 16:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109244674 s          0 s   16921428 s  5358873366 s        276 s
       #2  3501 MHz  442919827 s          0 s   18136665 s  5026947866 s         88 s
       #3  3501 MHz   86801750 s          0 s    9864625 s  5398747779 s        127 s
       #4  3501 MHz   82016019 s          0 s    9804924 s  5404027862 s         51 s
       
  Memory: 31.383651733398438 GB (5824.5234375 MB free)
  Uptime: 5.4975869e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4055
Commit da98033 (2018-02-22 09:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  109338914 s          0 s   16932594 s  5359699585 s        276 s
       #2  3501 MHz  443782987 s          0 s   18147072 s  5027008223 s         88 s
       #3  3501 MHz   86886205 s          0 s    9873055 s  5399589340 s        127 s
       #4  3501 MHz   82121408 s          0 s    9813242 s  5404848729 s         51 s
       
  Memory: 31.383651733398438 GB (5521.1796875 MB free)
  Uptime: 5.4985222e7 sec
  Load Avg:  1.03857421875  1.02685546875  1.04638671875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
