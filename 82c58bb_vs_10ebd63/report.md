# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@82c58bb0e4cfe64ff98dfcd64e0069110ef4606d](https://github.com/JuliaLang/julia/commit/82c58bb0e4cfe64ff98dfcd64e0069110ef4606d) vs [JuliaLang/julia@10ebd63343a3c57ea40ccfb62efcee78c2869885](https://github.com/JuliaLang/julia/commit/10ebd63343a3c57ea40ccfb62efcee78c2869885)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23642#issuecomment-348755898)

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
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequa lArray{Float32,1}\")"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Millisecond\")"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"DateTime\", \"Month\")"]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"DateTime\", \"Year\")"]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "arithmetic", "(\"Date\", \"Year\")"]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["dates", "construction", "Date"]` | 0.74 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "construction", "DateTime"]` | 0.80 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 1.35 (15%) :x: | 1.19 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 2.00 (15%) :x: | 12.00 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 3.90 (15%) :x: | 7.79 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 3.33 (15%) :x: | 4.17 (1%) :x: |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 3.80 (15%) :x: | 7.79 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 1.10 (15%)  | 1.16 (1%) :x: |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 3.58 (15%) :x: | 23.50 (1%) :x: |
| `["dates", "parse", "Date"]` | 26.12 (15%) :x: | 23.50 (1%) :x: |
| `["dates", "parse", "DateTime"]` | 8.49 (15%) :x: | 12.00 (1%) :x: |
| `["io", "read", "readstring"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["micro", "mandel"]` | 3.48 (15%) :x: | 47.56 (1%) :x: |
| `["misc", "parse", "DateTime"]` | 9.05 (15%) :x: | 11.95 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 1.05 (15%)  | 1.09 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.05 (15%)  | 1.16 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.06 (15%)  | 1.04 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.05 (15%)  | 1.12 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.04 (15%)  | 1.16 (1%) :x: |
| `["problem", "spellcheck", "spellcheck"]` | 2.52 (15%) :x: | 2.12 (1%) :x: |

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
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2740
Commit 82c58bb (2017-12-03 10:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96301344 s          0 s   14991634 s  4673093219 s        220 s
       #2  3501 MHz  383392897 s          0 s   16185271 s  4387132415 s         77 s
       #3  3501 MHz   78743808 s          0 s    8939654 s  4705531729 s         99 s
       #4  3501 MHz   73906085 s          0 s    8849391 s  4710860360 s         42 s
       
  Memory: 31.383651733398438 GB (1630.82421875 MB free)
  Uptime: 4.7951592e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2732
Commit 10ebd63 (2017-12-03 06:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96391572 s          0 s   15001500 s  4673667261 s        220 s
       #2  3501 MHz  383997572 s          0 s   16195652 s  4387193337 s         77 s
       #3  3501 MHz   78846450 s          0 s    8947741 s  4706097003 s         99 s
       #4  3501 MHz   73991340 s          0 s    8856928 s  4711443772 s         42 s
       
  Memory: 31.383651733398438 GB (2546.9921875 MB free)
  Uptime: 4.7958361e7 sec
  Load Avg:  0.8837890625  0.9814453125  1.03466796875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
