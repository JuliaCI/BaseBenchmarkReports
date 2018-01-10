# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1b36159a16cdd7e41c3618f70e765d04261c0775](https://github.com/JuliaLang/julia/commit/1b36159a16cdd7e41c3618f70e765d04261c0775) vs [JuliaLang/julia@6a45619a22c668237fac959225a5700a31b7da5f](https://github.com/JuliaLang/julia/commit/6a45619a22c668237fac959225a5700a31b7da5f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24774#issuecomment-356473514)

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
| `["dates", "arithmetic", "(\"DateTime\", \"Hour\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Millisecond\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Minute\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["find", "(\"Array{Bool,1}\", \"50-50\")"]` | 2.79 (15%) :x: | 2.10 (1%) :x: |
| `["find", "(\"Base.Generator{Array{Bool,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##3#6\\\"))}\", \"50-50\")"]` | 2.97 (15%) :x: | 2.10 (1%) :x: |
| `["find", "(\"Base.Generator{BitArray{1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##3#6\\\"))}\", \"10-90\")"]` | 1.54 (15%) :x: | 2.75 (1%) :x: |
| `["find", "(\"Base.Generator{BitArray{1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##3#6\\\"))}\", \"90-10\")"]` | 3.92 (15%) :x: | 2.31 (1%) :x: |
| `["find", "(\"ispos\", \"Array{Bool,1}\")"]` | 0.99 (15%)  | 0.69 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.00 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{Float64,1}\")"]` | 1.04 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{Int64,1}\")"]` | 1.03 (15%)  | 0.80 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{Int8,1}\")"]` | 0.96 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{UInt64,1}\")"]` | 0.99 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Array{UInt8,1}\")"]` | 0.99 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Bool,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 0.98 (15%)  | 0.69 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Float32,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 1.36 (15%) :x: | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Float64,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 1.25 (15%) :x: | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Int64,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 1.04 (15%)  | 0.80 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Base.Generator{Array{Int8,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 1.10 (15%)  | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Base.Generator{Array{UInt64,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 1.18 (15%) :x: | 0.68 (1%) :white_check_mark: |
| `["find", "(\"ispos\", \"Base.Generator{Array{UInt8,1},getfield(BaseBenchmarks.FindBenchmarks, Symbol(\\\"##16#17\\\"))}\")"]` | 1.20 (15%) :x: | 0.68 (1%) :white_check_mark: |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["io", "read", "readstring"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 2.44 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["misc", "parse", "Int"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 1.10 (30%)  | 1.29 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 1.43 (30%) :x: | 1.42 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 1.82 (30%) :x: | 1.35 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 1.30 (30%) :x: | 1.55 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 100)"]` | 1.11 (30%)  | 1.23 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"logical\", 1000)"]` | 1.09 (30%)  | 1.06 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 1.11 (30%)  | 1.50 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.31 (30%) :x: | 1.81 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 1.71 (30%) :x: | 1.82 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 2.02 (30%) :x: | 1.91 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"logical\", 10000)"]` | 1.68 (30%) :x: | 3.26 (1%) :x: |
| `["sparse", "index", "(\"spvec\", \"logical\", 100000)"]` | 1.65 (30%) :x: | 2.60 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 1.00 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 1.03 (30%)  | 1.01 (1%) :x: |
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
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3365
Commit 1b36159 (2018-01-09 22:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101835179 s          0 s   15800613 s  4991385436 s        248 s
       #2  3501 MHz  403861591 s          0 s   17173619 s  4690433191 s         82 s
       #3  3501 MHz   82447627 s          0 s    9338026 s  5026692025 s        110 s
       #4  3501 MHz   77670926 s          0 s    9272326 s  5031940060 s         45 s
       
  Memory: 31.383651733398438 GB (5327.92578125 MB free)
  Uptime: 5.1205119e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.3360
Commit 6a45619 (2018-01-09 22:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  101923919 s          0 s   15811954 s  4992256742 s        248 s
       #2  3501 MHz  404762772 s          0 s   17184454 s  4690495459 s         82 s
       #3  3501 MHz   82536352 s          0 s    9346336 s  5027569050 s        110 s
       #4  3501 MHz   77778557 s          0 s    9280564 s  5032798601 s         45 s
       
  Memory: 31.383651733398438 GB (5206.77734375 MB free)
  Uptime: 5.121487e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
