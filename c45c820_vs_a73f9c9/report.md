# Benchmark Report

## Job Properties

*Commit(s):* [YingboMa/julia@c45c82066116a0be1c813c49e44264b6f05c2217](https://github.com/YingboMa/julia/commit/c45c82066116a0be1c813c49e44264b6f05c2217) vs [JuliaLang/julia@a73f9c9a6d9c6563878e951e9998785ef8411c3e](https://github.com/JuliaLang/julia/commit/a73f9c9a6d9c6563878e951e9998785ef8411c3e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24833#issuecomment-348001470)

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
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Bool}()\")"]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 0.66 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 0.68 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 1.51 (30%) :x: | 1.00 (1%)  |
| `["tuple", "linear algebra", "(\"matmat\", (16, 16), (16, 16))"]` | 1.62 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2702
Commit c45c820 (2017-11-29 21:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  104954114 s          0 s   18584946 s  4627045192 s         98 s
       #2  3501 MHz  448465603 s          0 s   11882433 s  4301361568 s         22 s
       #3  3501 MHz   88730635 s          0 s   10159837 s  4663292612 s         81 s
       #4  3501 MHz   84896755 s          0 s   10348107 s  4666929964 s         21 s
       
  Memory: 31.383651733398438 GB (3197.82421875 MB free)
  Uptime: 4.7644634e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2699
Commit a73f9c9 (2017-11-29 21:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  105059854 s          0 s   18594453 s  4627670943 s         98 s
       #2  3501 MHz  449140553 s          0 s   11891987 s  4301420220 s         22 s
       #3  3501 MHz   88813091 s          0 s   10167798 s  4663945220 s         81 s
       #4  3501 MHz   84980246 s          0 s   10355697 s  4667582101 s         21 s
       
  Memory: 31.383651733398438 GB (3141.9921875 MB free)
  Uptime: 4.7652072e7 sec
  Load Avg:  0.8837890625  0.9814453125  1.03466796875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
