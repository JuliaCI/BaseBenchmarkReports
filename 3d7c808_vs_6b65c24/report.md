# Benchmark Report

## Job Properties

*Commit(s):* [abraunst/julia@3d7c808cdad457ea1cf18ac0faf76cbde7c81412](https://github.com/abraunst/julia/commit/3d7c808cdad457ea1cf18ac0faf76cbde7c81412) vs [JuliaLang/julia@6b65c24def7aaac9b4f238c17d5f69924298def5](https://github.com/JuliaLang/julia/commit/6b65c24def7aaac9b4f238c17d5f69924298def5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30676#issuecomment-470414167)

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
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 1.12 (5%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 0.86 (5%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 0.87 (5%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.40 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "small exp #29116"]` | 1.26 (5%) :x: | 1.00 (1%)  |
| `["misc", "repeat", "(200, 24, 1)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.12 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 0.23 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.63 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.97 (30%)  | 0.45 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 0.53 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.62 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.19 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 0.33 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 0.68 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 0.90 (30%)  | 0.46 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.95 (30%)  | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.87 (30%)  | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 0.62 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 0.46 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.64 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.97 (30%)  | 0.45 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 0.23 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.12 (30%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 1.59 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 0.99 (30%)  | 0.45 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.92 (30%)  | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 0.72 (30%)  | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 0.57 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 0.68 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 0.90 (30%)  | 0.46 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 0.33 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 0.62 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 0.19 (30%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 0.52 (30%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 0.92 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 0.76 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 1.24 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 1.09 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 1.05 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 0.88 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 1.27 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 1.10 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 1.07 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 0.71 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 0.82 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 1.06 (5%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float32}, true)"]` | 0.80 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", sum, Union{Missing, Float64}, true)"]` | 0.89 (5%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"sort\", Union{Nothing, Int8}, false)"]` | 1.15 (5%) :x: | 1.00 (1%)  |

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
Julia Version 1.2.0-DEV.454
Commit 3d7c808 (2019-03-07 07:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   44786349 s       2430 s    9260840 s  2914903177 s         12 s
       #2  3501 MHz  254250368 s         14 s    4584796 s  2717050633 s         18 s
       #3  3501 MHz   35791647 s       3153 s    4354051 s  2935487947 s         27 s
       #4  3501 MHz   34497439 s         14 s    3268844 s  2939229211 s         24 s
       
  Memory: 31.383651733398438 GB (4752.73046875 MB free)
  Uptime: 2.9781511e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.2.0-DEV.435
Commit 6b65c24 (2019-03-07 07:08 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   44908807 s       2430 s    9269584 s  2915487480 s         12 s
       #2  3501 MHz  254897722 s         14 s    4593456 s  2717112146 s         18 s
       #3  3501 MHz   35907537 s       3153 s    4361221 s  2936082341 s         27 s
       #4  3501 MHz   34610384 s         14 s    3276084 s  2939826673 s         24 s
       
  Memory: 31.383651733398438 GB (4531.98828125 MB free)
  Uptime: 2.9788693e7 sec
  Load Avg:  1.3232421875  1.0810546875  1.06689453125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
