# Benchmark Report

## Job Properties

*Commit(s):* [abraunst/julia@f0b14abb4c44c02bfb31bb5cc5baa92130345592](https://github.com/abraunst/julia/commit/f0b14abb4c44c02bfb31bb5cc5baa92130345592) vs [JuliaLang/julia@585feb0df87c0dfbea5ad42206c168709bcff4f5](https://github.com/JuliaLang/julia/commit/585feb0df87c0dfbea5ad42206c168709bcff4f5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30676#issuecomment-459698421)

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
| `["array", "accumulate", "(\"accumulate\", \"Int\")"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim2\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.46 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.25 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 1.39 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 256)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"append!\", 8)"]` | 0.78 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.72 (45%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 1.16 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 100)"]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 1000)"]` | 0.59 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.12 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 0.23 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.59 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.91 (30%)  | 0.45 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 0.54 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.63 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.19 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 0.33 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.70 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.92 (30%)  | 0.46 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.98 (30%)  | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.89 (30%)  | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 0.63 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 0.46 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.60 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.90 (30%)  | 0.45 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 0.23 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.12 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.99 (30%)  | 0.45 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.92 (30%)  | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 0.71 (30%)  | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 0.56 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.70 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.92 (30%)  | 0.46 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 0.33 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.63 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.19 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 0.54 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse", "sparse matvec", "adjoint"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["sparse", "sparse matvec", "non-adjoint"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 1.20 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 0.91 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 0.75 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.81 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 0.84 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.22 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Int64, false)"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Union{Nothing, BigFloat}, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Complex{Float64}}, true)"]` | 1.14 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Bool}, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Int8}, false)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |

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
- `["io", "array_limit"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`
- `["misc", "julia"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
- `["problem", "laplacian"]`
- `["simd"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "sparse matvec"]`
- `["sparse", "sparse solves"]`
- `["sparse", "transpose"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.2.0-DEV.260
Commit f0b14ab (2019-02-01 08:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   74612392 s       5014 s    8309711 s  2596558425 s         23 s
       #2  3501 MHz  436928039 s        203 s    7192053 s  2239807039 s         19 s
       #3  3501 MHz   57713066 s       3226 s    4872437 s  2621234786 s         26 s
       #4  3501 MHz   54091020 s          2 s    6335698 s  2622728561 s         17 s
       
  Memory: 31.383651733398438 GB (5757.671875 MB free)
  Uptime: 2.6860621e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.2.0-DEV.243
Commit 585feb0 (2019-02-01 07:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   74737970 s       5014 s    8318900 s  2597144151 s         23 s
       #2  3501 MHz  437578292 s        203 s    7199796 s  2239871663 s         19 s
       #3  3501 MHz   57829602 s       3226 s    4879825 s  2621833491 s         26 s
       #4  3501 MHz   54206065 s          2 s    6342938 s  2623328947 s         17 s
       
  Memory: 31.383651733398438 GB (5409.46484375 MB free)
  Uptime: 2.6867853e7 sec
  Load Avg:  1.05908203125  1.029296875  1.048828125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
