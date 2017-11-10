# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9b29fe016cf84a31aff5f4a7874226d302f3066b](https://github.com/JuliaLang/julia/commit/9b29fe016cf84a31aff5f4a7874226d302f3066b) vs [JuliaLang/julia@247087d94c1414d83e28d721f263ba4bf050f854](https://github.com/JuliaLang/julia/commit/247087d94c1414d83e28d721f263ba4bf050f854)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24519#issuecomment-343567313)

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
| `["array", "cat", "(\"catnd\", 5)"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 1.84 (50%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.64 (50%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 1.14 (30%)  | 1.92 (1%) :x: |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.92 (30%)  | 0.53 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.09 (30%)  | 1.94 (1%) :x: |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.94 (30%)  | 1.92 (1%) :x: |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 0.90 (30%)  | 0.52 (1%) :white_check_mark: |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 0.90 (30%)  | 0.53 (1%) :white_check_mark: |

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
Julia Version 0.6.2-pre.36
Commit 9b29fe0 (2017-11-10 19:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11381.48828125 MB free)
Uptime: 4.5995765e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   92957451 s          0 s   14429968 s  4481902644 s        203 s
#2  3501 MHz  370636222 s          0 s   15654700 s  4205156523 s         70 s
#3  3501 MHz   76562115 s          0 s    8725531 s  4512384935 s         91 s
#4  3501 MHz   71741237 s          0 s    8592948 s  4517755590 s         36 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.2-pre.2
Commit 247087d (2017-10-30 18:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10805.3515625 MB free)
Uptime: 4.6002366e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   93057195 s          0 s   14440694 s  4482449564 s        203 s
#2  3501 MHz  371237426 s          0 s   15664370 s  4205204871 s         70 s
#3  3501 MHz   76650032 s          0 s    8734015 s  4512947801 s         92 s
#4  3501 MHz   71824863 s          0 s    8601359 s  4518322930 s         36 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
