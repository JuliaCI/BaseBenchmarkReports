# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ee07b8cb23e5330d25d0b05accdc0278997a0b3f](https://github.com/JuliaLang/julia/commit/ee07b8cb23e5330d25d0b05accdc0278997a0b3f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/ee07b8cb23e5330d25d0b05accdc0278997a0b3f#commitcomment-29601204)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-07-05 vs 2018-07-04

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
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.90 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.89 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.91 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.91 (50%)  | 0.99 (1%) :white_check_mark: |
| `["array", "index", "(\"sumeach_view\", \"1:100000\")"]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Float64\")"]` | 0.89 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 0.90 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Float64\")"]` | 0.89 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 0.90 (15%)  | 0.98 (1%) :white_check_mark: |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 1.09 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"big\")"]` | 1.96 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 1.52 (25%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float64\")"]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"very small\", \"negative argument\", \"Float64\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 1.73 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 0.74 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string", "join"]` | 0.49 (40%) :white_check_mark: | 1.00 (1%)  |
| `["string", "readuntil", "target length 1000"]` | 1.70 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 2"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["string", "readuntil", "target length 50000"]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matvec\", (16, 16), (16,))"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Int8, false)"]` | 1.15 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-beta.152
Commit ee07b8c (2018-07-04 17:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   38738583 s        278 s    4040788 s  814941526 s          8 s
       #2  3501 MHz  177090947 s          0 s    2490594 s  680260551 s          4 s
       #3  3501 MHz   24276738 s       2379 s    2011441 s  833163403 s         12 s
       #4  3501 MHz   22652168 s          0 s    2324584 s  834656168 s          8 s
       
  Memory: 31.383651733398438 GB (4966.6953125 MB free)
  Uptime: 8.603655e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
