# Benchmark Report

## Job Properties

*Commit(s):* [alyst/julia@b84bf49f05eb4d3da4e3c6723476788d995cea02](https://github.com/alyst/julia/commit/b84bf49f05eb4d3da4e3c6723476788d995cea02) vs [JuliaLang/julia@0e8408f884778a3e8b2d2dc0368967c29dd556c9](https://github.com/JuliaLang/julia/commit/0e8408f884778a3e8b2d2dc0368967c29dd556c9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22038#issuecomment-305036389)

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
| `["array","bool","boolarray_true_load!"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",2048)]` | 1.01 (15%)  | 0.80 (1%) :white_check_mark: |
| `["array","growth",("append!",256)]` | 1.12 (15%)  | 1.26 (1%) :x: |
| `["array","growth",("append!",8)]` | 1.15 (15%)  | 1.25 (1%) :x: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.61 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","DateFormat")]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["io","serialization",("serialize","Matrix{Float64}")]` | 0.99 (15%)  | 0.95 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.98 (15%)  | 0.89 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["shootout","revcomp"]` | 0.97 (25%)  | 1.04 (1%) :x: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.30 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",100)]` | 1.10 (30%)  | 1.46 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.13 (30%)  | 1.24 (1%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.10 (30%)  | 1.07 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.12 (30%)  | 1.79 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.07 (30%)  | 1.25 (1%) :x: |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.24 (40%)  | 1.22 (1%) :x: |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.411
Commit b84bf49 (2017-05-30 22:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2844.01171875 MB free)
Uptime: 3.1837635e7 sec
Load Avg:  1.00341796875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   67277269 s          0 s   10327858 s  3099305827 s         91 s
#2  3501 MHz  261348474 s          0 s   11270834 s  2905366058 s         36 s
#3  3501 MHz   57535623 s          0 s    6677226 s  3118104483 s         48 s
#4  3501 MHz   53065786 s          0 s    6628197 s  3122917297 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.403
Commit 0e8408f (2017-05-30 19:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2653.92578125 MB free)
Uptime: 3.1842953e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   67362944 s          0 s   10337488 s  3099740306 s         91 s
#2  3501 MHz  261825897 s          0 s   11279801 s  2905410862 s         36 s
#3  3501 MHz   57619767 s          0 s    6685729 s  3118542980 s         48 s
#4  3501 MHz   53159634 s          0 s    6636840 s  3123346045 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
