# Benchmark Report

## Job Properties

*Commit(s):* [jlapeyre/julia@56b504a1f8ffbbbbefb0dc9cd4f180948ace47ba](https://github.com/jlapeyre/julia/commit/56b504a1f8ffbbbbefb0dc9cd4f180948ace47ba) vs [JuliaLang/julia@c05fd201baedb6681947cc212e0a9f49564d1568](https://github.com/JuliaLang/julia/commit/c05fd201baedb6681947cc212e0a9f49564d1568)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28376#issuecomment-409869255)

*Tag Predicate:* `"array"`

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
| `["array", "accumulate", "(\"accumulate\", \"Int\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim1\")"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim2\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"catnd\", 5)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"hvcat\", 500)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat\", 500)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"push_single!\", 8)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "index", "5d"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "6d"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "7d"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 256)"]` | 1.54 (45%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 1, 24)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["sparse", "arithmetic", "(\"unary minus\", (20000, 20000))"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"integer\", 10000)"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spvec\", \"integer\", 100000)"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x4000, dense 4000x40 -> dense 400x40\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x500, dense 500x5 -> dense 50x5\")"]` | 1.54 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 1.30 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 200x2000 -> dense 20x200\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 1.36 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", BigInt, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", BigInt, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.23 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.70 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, BigInt, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 1.18 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 0.47 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, true)"]` | 1.29 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigInt, false)"]` | 1.13 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", BigInt, true)"]` | 1.12 (5%) :x: | 1.00 (1%)  |

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
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["misc", "julia"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
- `["problem", "laplacian"]`
- `["simd"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "transpose"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta2.191
Commit 56b504a (2018-08-01 18:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   27925382 s        260 s    3868868 s  1069385218 s          7 s
       #2  3501 MHz  136211770 s          2 s    2270122 s  964850864 s         11 s
       #3  3501 MHz   21068435 s       2397 s    2416543 s  1079853367 s         16 s
       #4  3501 MHz   20200093 s          4 s    1865133 s  1081859482 s          9 s
       
  Memory: 31.383651733398438 GB (4392.2265625 MB free)
  Uptime: 1.1044444e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-rc1.11
Commit c05fd20 (2018-08-01 18:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   28040913 s        260 s    3879310 s  1069985311 s          7 s
       #2  3501 MHz  136868660 s          2 s    2279740 s  964912637 s         11 s
       #3  3501 MHz   21192192 s       2397 s    2426011 s  1080448131 s         16 s
       #4  3501 MHz   20315819 s          4 s    1873854 s  1082463342 s          9 s
       
  Memory: 31.383651733398438 GB (3798.67578125 MB free)
  Uptime: 1.1051733e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
