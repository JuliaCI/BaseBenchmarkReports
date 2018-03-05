# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@bbc3220ecfdb9d316307ddf4ed24fc2a3bc1801b](https://github.com/JuliaLang/julia/commit/bbc3220ecfdb9d316307ddf4ed24fc2a3bc1801b) vs [JuliaLang/julia@f569ebe9bcfdeeae94952d9105c33dbf6b545da7](https://github.com/JuliaLang/julia/commit/f569ebe9bcfdeeae94952d9105c33dbf6b545da7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26322#issuecomment-370473219)

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
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array", "bool", "bitarray_true_fill!"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 0.84 (25%)  | 0.88 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter\")"]` | 0.35 (25%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 0.64 (25%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 0.73 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 0.77 (25%)  | 0.81 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 0.74 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"iterator\")"]` | 0.27 (25%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\")"]` | 0.31 (25%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\", \"sizehint!\")"]` | 0.27 (25%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"String\", \"iterator\")"]` | 0.51 (25%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\")"]` | 0.58 (25%) :white_check_mark: | 0.74 (1%) :white_check_mark: |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\", \"sizehint!\")"]` | 0.52 (25%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Nothing\")"]` | 0.31 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Nothing\")"]` | 0.35 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Bool\")"]` | 0.28 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Int8\")"]` | 0.42 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"UInt16\")"]` | 0.38 (25%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Bool\")"]` | 0.29 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Int8\")"]` | 0.42 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"UInt16\")"]` | 0.38 (25%) :white_check_mark: | 0.30 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"specified\")"]` | 1.00 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"new\")"]` | 1.00 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 1.00 (25%)  | 0.50 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"specified\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"push!\", \"new\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"push!\", \"overwrite\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"specified\")"]` | 0.87 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"new\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"overwrite\")"]` | 1.00 (25%)  | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 0.64 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.39 (25%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.44 (25%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 0.47 (25%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.40 (25%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.41 (25%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.47 (25%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"BitSet\")"]` | 0.59 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Set\")"]` | 0.48 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Vector\")"]` | 0.48 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\")"]` | 0.28 (25%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.30 (25%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\")"]` | 0.28 (25%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.28 (25%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\")"]` | 0.30 (25%) :white_check_mark: | 0.78 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.30 (25%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 0.48 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\")"]` | 0.47 (25%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 0.48 (25%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\")"]` | 0.51 (25%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 0.51 (25%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\")"]` | 0.54 (25%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 0.53 (25%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"BitSet\")"]` | 0.46 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 0.49 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 0.47 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 0.66 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\")"]` | 0.75 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 0.65 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 0.70 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 0.69 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 0.69 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 0.65 (25%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 0.51 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\")"]` | 0.48 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 0.50 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 0.47 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 0.49 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 0.44 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 0.53 (25%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Millisecond\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Second\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.41 (45%) :x: | 1.00 (1%)  |
| `["problem", "imdb", "centrality"]` | 0.76 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["problem", "spellcheck", "spellcheck"]` | 1.00 (15%)  | 0.97 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.4467
Commit bbc3220 (2018-03-05 13:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110188148 s          0 s   17148018 s  5451983384 s        284 s
       #2  3501 MHz  448099304 s          0 s   18273501 s  5116218892 s         88 s
       #3  3501 MHz   87366259 s          0 s    9929138 s  5492768848 s        130 s
       #4  3501 MHz   82589280 s          0 s    9931349 s  5497944012 s         53 s
       
  Memory: 31.383651733398438 GB (5862.3359375 MB free)
  Uptime: 5.5922555e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.4465
Commit f569ebe (2018-03-04 15:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  110305048 s          0 s   17158869 s  5452794979 s        284 s
       #2  3501 MHz  448966265 s          0 s   18284079 s  5116282826 s         88 s
       #3  3501 MHz   87451174 s          0 s    9937332 s  5493617808 s        130 s
       #4  3501 MHz   82675693 s          0 s    9939313 s  5498792036 s         53 s
       
  Memory: 31.383651733398438 GB (5101.17578125 MB free)
  Uptime: 5.5931985e7 sec
  Load Avg:  0.9716796875  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
