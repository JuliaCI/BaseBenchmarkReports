# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@26eb512367936550a0fd1c6414f09215845f6eb1](https://github.com/JuliaLang/julia/commit/26eb512367936550a0fd1c6414f09215845f6eb1) vs [JuliaLang/julia@fce2d689222c10ae735362dc67a8f6b973be55a3](https://github.com/JuliaLang/julia/commit/fce2d689222c10ae735362dc67a8f6b973be55a3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/26eb512367936550a0fd1c6414f09215845f6eb1#commitcomment-25531390)

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
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["dates", "string", "DateTime"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 0.31 (15%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 1024)"]` | 2.33 (45%) :x: | 4.00 (1%) :x: |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 256)"]` | 2.54 (45%) :x: | 4.00 (1%) :x: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 0.69 (45%)  | 0.03 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 1.61 (45%) :x: | 0.10 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 1024)"]` | 0.56 (45%)  | 0.02 (1%) :white_check_mark: |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 256)"]` | 1.31 (45%)  | 0.08 (1%) :white_check_mark: |
| `["micro", "fib"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc", "julia", "(\"macroexpand\", \"evalpoly\")"]` | 0.06 (15%) :white_check_mark: | 1.14 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 1.10 (15%)  | 1.98 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 2.00 (15%) :x: | 7.01 (1%) :x: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 1.07 (15%)  | 1.53 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 0.97 (15%)  | 0.90 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.06 (15%)  | 0.86 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.00 (15%)  | 0.96 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.01 (15%)  | 0.90 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 0.99 (15%)  | 0.86 (1%) :white_check_mark: |
| `["problem", "json", "parse_json"]` | 3.17 (15%) :x: | 2.30 (1%) :x: |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"randexp!\", \"RandomDevice\", \"Float64\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "k_nucleotide"]` | 0.69 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["shootout", "regex_dna"]` | 0.86 (15%)  | 0.77 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 1.33 (30%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 1000)"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.03 (30%)  | 0.72 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 1.62 (30%) :x: | 0.73 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.34 (30%) :x: | 0.69 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.09 (30%)  | 0.65 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 7.81 (30%) :x: | 1.22 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 3.89 (30%) :x: | 1.22 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.55 (30%) :x: | 1.23 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 1.09 (30%)  | 2.66 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 1.01 (30%)  | 0.87 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 1.80 (30%) :x: | 1.52 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.52 (30%) :x: | 1.57 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.06 (30%)  | 0.68 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 4.74 (30%) :x: | 1.68 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 2.82 (30%) :x: | 1.70 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 1.32 (30%) :x: | 1.64 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 1.04 (30%)  | 2.30 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 1.04 (30%)  | 1.41 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.10 (30%)  | 1.23 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.54 (30%) :x: | 1.22 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.96 (30%)  | 0.64 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.01 (30%)  | 0.69 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 2.10 (30%) :x: | 1.22 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 1.14 (30%)  | 0.73 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.01 (30%)  | 0.72 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.51 (30%) :x: | 1.23 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.09 (30%)  | 2.66 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 3.84 (30%) :x: | 1.22 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.33 (30%) :x: | 0.69 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.07 (30%)  | 0.65 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 7.66 (30%) :x: | 1.22 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 1.64 (30%) :x: | 0.73 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.02 (30%)  | 0.72 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 1.02 (30%)  | 1.25 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.09 (30%)  | 1.64 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.43 (30%) :x: | 1.71 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.11 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.11 (30%)  | 0.78 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.75 (30%) :x: | 1.68 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 1.13 (30%)  | 0.76 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.01 (30%)  | 0.87 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 1.33 (30%) :x: | 1.64 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 1.09 (30%)  | 2.30 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 2.83 (30%) :x: | 1.70 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.55 (30%) :x: | 1.57 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.08 (30%)  | 0.68 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 4.75 (30%) :x: | 1.68 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 1.82 (30%) :x: | 1.52 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 1.02 (30%)  | 0.87 (1%) :white_check_mark: |
| `["string", "replace"]` | 0.44 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
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
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
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
- `["nullable", "basic"]`
- `["nullable", "nullablearray"]`
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
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "cos"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "tan"]`
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
Julia Version 0.7.0-DEV.2484
Commit 26eb512 (2017-11-09 21:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92778013 s          0 s   14408163 s  4479709801 s        203 s
       #2  3501 MHz  369418443 s          0 s   15634174 s  4203995930 s         70 s
       #3  3501 MHz   76375537 s          0 s    8709051 s  4510188117 s         91 s
       #4  3501 MHz   71575682 s          0 s    8575854 s  4515538315 s         36 s
       
  Memory: 31.383651733398438 GB (11683.97265625 MB free)
  Uptime: 4.5971746e7 sec
  Load Avg:  1.05908203125  1.029296875  1.048828125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2068
Commit fce2d68 (2017-10-07 21:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92866468 s          0 s   14417842 s  4480284176 s        203 s
       #2  3501 MHz  370024626 s          0 s   15643461 s  4204054853 s         70 s
       #3  3501 MHz   76474076 s          0 s    8716802 s  4510756077 s         91 s
       #4  3501 MHz   71657064 s          0 s    8583637 s  4516123736 s         36 s
       
  Memory: 31.383651733398438 GB (11112.94921875 MB free)
  Uptime: 4.5978499e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
