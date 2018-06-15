# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@66c57fc2a872e94695ff20eec6a986eca96ab788](https://github.com/JuliaLang/julia/commit/66c57fc2a872e94695ff20eec6a986eca96ab788) vs [JuliaLang/julia@5ba7f20e31062a9f96369a55e6c8790062df1f0b](https://github.com/JuliaLang/julia/commit/5ba7f20e31062a9f96369a55e6c8790062df1f0b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27495#issuecomment-397422188)

*Tag Predicate:* `"array" || ("problem" || "random")`

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
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sum\", \"3darray\")"]` | 5.59 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumelt\", \"1:100000\")"]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 1.47 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"mean\", \"Int64\")"]` | 1.46 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 1.40 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 1.38 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 1.37 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs2\", \"Int64\")"]` | 1.16 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 1.43 (15%) :x: | Inf (1%) :x: |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 1.33 (15%) :x: | Inf (1%) :x: |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 4.11 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 3.47 (15%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float16\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Int64\")"]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 1.15 (15%) :x: | 1.00 (1%)  |

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
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha.142
Commit 66c57fc (2018-06-14 18:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   29058657 s        276 s    3121002 s  650164727 s          6 s
       #2  3501 MHz  124421352 s          0 s    1731819 s  558006883 s          3 s
       #3  3501 MHz   16361212 s       2373 s    1392373 s  666078609 s          9 s
       #4  3501 MHz   15360699 s          0 s    1626152 s  667003802 s          6 s
       
  Memory: 31.383651733398438 GB (5477.10546875 MB free)
  Uptime: 6.845272e6 sec
  Load Avg:  1.03564453125  1.0263671875  1.0458984375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.137
Commit 5ba7f20 (2018-06-14 18:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   29173679 s        276 s    3131616 s  650788069 s          6 s
       #2  3501 MHz  125113936 s          0 s    1742436 s  558055307 s          3 s
       #3  3501 MHz   16476727 s       2373 s    1400986 s  666705851 s          9 s
       #4  3501 MHz   15471655 s          0 s    1634838 s  667635555 s          6 s
       
  Memory: 31.383651733398438 GB (4428.859375 MB free)
  Uptime: 6.852793e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
