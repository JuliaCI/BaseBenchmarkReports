# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a984951cbdedd9e1cdf56cd4426b7f07fa502109](https://github.com/JuliaLang/julia/commit/a984951cbdedd9e1cdf56cd4426b7f07fa502109) vs [JuliaLang/julia@333ea8c3f2c3f4d858c4b431ca6c63fc1ffc3d48](https://github.com/JuliaLang/julia/commit/333ea8c3f2c3f4d858c4b431ca6c63fc1ffc3d48)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27670#issuecomment-398567909)

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
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 5)"]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.63 (50%)  | 0.83 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.31 (50%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 0.65 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.30 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"start\")"]` | 0.64 (25%) :white_check_mark: | 0.92 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"start\")"]` | 0.96 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"start\")"]` | 0.95 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Dict\", \"String\", \"start\")"]` | 0.94 (25%)  | 0.97 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"Any\", \"start\")"]` | 0.92 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"Int\", \"start\")"]` | 0.93 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Set\", \"String\", \"start\")"]` | 0.94 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"start\")"]` | 0.93 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"next\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"start\")"]` | 0.92 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "iteration", "(\"Vector\", \"String\", \"start\")"]` | 0.91 (25%)  | 0.96 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 2.02 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "asinh", "(\"zero\", \"Float64\")"]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "fastmath", "(\"add\", \"Complex{Float64}\")"]` | 1.79 (40%) :x: | 1.00 (1%)  |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 1.90 (15%) :x: | 1.00 (1%)  |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float64\")"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 7.65 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 8.14 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4095)"]` | 3.39 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4096)"]` | 3.39 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4095)"]` | 6.90 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 7.08 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4095)"]` | 1.56 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4096)"]` | 1.57 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 1.69 (20%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 0.30 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 0.29 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 1.01 (15%)  | 0.94 (1%) :white_check_mark: |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 0.99 (15%)  | 0.94 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 0.55 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.52 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 1.00 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 0.98 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 0.98 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 0.82 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 0.99 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 0.97 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 0.99 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 0.99 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 0.55 (30%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-alpha.210
Commit a984951 (2018-06-19 23:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   30457870 s        277 s    3273794 s  693773969 s          6 s
       #2  3501 MHz  135401522 s          0 s    1874458 s  592111879 s          4 s
       #3  3501 MHz   17731604 s       2375 s    1504006 s  709836929 s          9 s
       #4  3501 MHz   16624741 s          0 s    1773226 s  710807978 s          6 s
       
  Memory: 31.383651733398438 GB (3976.99609375 MB free)
  Uptime: 7.298037e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.203
Commit 333ea8c (2018-06-19 21:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   30602490 s        277 s    3286068 s  694732227 s          6 s
       #2  3501 MHz  136433428 s          0 s    1885550 s  592187437 s          4 s
       #3  3501 MHz   17847669 s       2375 s    1512872 s  710829610 s          9 s
       #4  3501 MHz   16732184 s          0 s    1781922 s  711810237 s          6 s
       
  Memory: 31.383651733398438 GB (4253.953125 MB free)
  Uptime: 7.309228e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
