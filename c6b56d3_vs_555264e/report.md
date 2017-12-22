# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c6b56d3360ae3512dd866eb4b3ea72aa74ff59f6](https://github.com/JuliaLang/julia/commit/c6b56d3360ae3512dd866eb4b3ea72aa74ff59f6) vs [JuliaLang/julia@555264e1f005eb390ad22c29c26cf14c662b0677](https://github.com/JuliaLang/julia/commit/555264e1f005eb390ad22c29c26cf14c662b0677)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21527#issuecomment-353435647)

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
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 1.25 (25%) :x: | 2.37 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 1.00 (25%)  | 0.98 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 6.62 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 13.40 (25%) :x: | 0.72 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\")"]` | 0.75 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.11 (25%)  | 1.57 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 0.92 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.12 (25%)  | 2.67 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 1.00 (25%)  | 0.95 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 5.22 (25%) :x: | 10.02 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.11 (25%)  | 1.57 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 148.38 (25%) :x: | 174.74 (1%) :x: |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 182.01 (25%) :x: | 174.74 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 3.21 (25%) :x: | 0.99 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 3.20 (25%) :x: | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 5.22 (25%) :x: | 0.99 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 4.69 (25%) :x: | 0.97 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 13.78 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 6.08 (25%) :x: | 0.36 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"BitSet\")"]` | 13.92 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Set\")"]` | 14.06 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Vector\")"]` | 18.52 (25%) :x: | 1.70 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\")"]` | 0.11 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 1.82 (25%) :x: | 1.93 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 1.83 (25%) :x: | 1.94 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 1.91 (25%) :x: | 1.95 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 1.87 (25%) :x: | 1.96 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 2.05 (25%) :x: | 2.54 (1%) :x: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 1.92 (25%) :x: | 2.62 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 0.10 (25%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.04 (25%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.03 (25%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\")"]` | 0.09 (25%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.07 (25%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\")"]` | 0.18 (25%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.18 (25%) :white_check_mark: | 0.02 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"BitSet\")"]` | 0.88 (25%)  | 1.04 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 0.81 (25%)  | 1.03 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.87 (25%)  | 1.04 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 0.01 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\")"]` | 2.42 (25%) :x: | 7.13 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 2.42 (25%) :x: | 7.11 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 2.71 (25%) :x: | 7.14 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 2.52 (25%) :x: | 7.15 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 3.33 (25%) :x: | 9.44 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 3.35 (25%) :x: | 9.59 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 1.85 (25%) :x: | 1.46 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\")"]` | 2.09 (25%) :x: | 1.46 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 1.99 (25%) :x: | 1.46 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 2.00 (25%) :x: | 1.46 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 1.83 (25%) :x: | 1.46 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 1.96 (25%) :x: | 1.46 (1%) :x: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 1.90 (25%) :x: | 1.46 (1%) :x: |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 1024)"]` | 0.03 (45%) :white_check_mark: | 0.07 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 256)"]` | 0.25 (45%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "fib"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "splatting", "(3, 3, 3)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 1.16 (15%) :x: | 1.00 (1%)  |

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

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3109
Commit c6b56d3 (2017-12-19 19:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100891204 s          0 s   15608243 s  4826179779 s        235 s
       #2  3501 MHz  397009481 s          0 s   16687182 s  4531495701 s         80 s
       #3  3501 MHz   81561725 s          0 s    9216676 s  4861095510 s        106 s
       #4  3501 MHz   76735620 s          0 s    9139382 s  4866403931 s         44 s
       
  Memory: 31.383651733398438 GB (3820.0 MB free)
  Uptime: 4.9538708e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3137
Commit 555264e (2017-12-20 23:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100982536 s          0 s   15619152 s  4826912992 s        236 s
       #2  3501 MHz  397796500 s          0 s   16697449 s  4531536338 s         80 s
       #3  3501 MHz   81646570 s          0 s    9225041 s  4861840132 s        107 s
       #4  3501 MHz   76821140 s          0 s    9147244 s  4867148570 s         44 s
       
  Memory: 31.383651733398438 GB (3624.30859375 MB free)
  Uptime: 4.9547096e7 sec
  Load Avg:  0.88916015625  0.9814453125  1.03466796875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
