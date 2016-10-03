# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@09356eaf038bcb47e9ed8d27378804f7679e6b2e](https://github.com/JuliaLang/julia/commit/09356eaf038bcb47e9ed8d27378804f7679e6b2e) vs [JuliaLang/julia@d2db55aa94079850f3c53e5910313ebe50a32119](https://github.com/JuliaLang/julia/commit/d2db55aa94079850f3c53e5910313ebe50a32119)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18777#issuecomment-251201252)

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
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000000)")]` | 0.41 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","linspace(1.0,2.0,10000000)")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","linspace(1.0,2.0,10000000)")]` | 0.35 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","linspace(1.0,2.0,10000000)")]` | 0.40 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Complex{Float64}")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 1.16 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
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
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.871
Commit 09356ea (2016-10-03 18:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14286.21875 MB free)
Uptime: 1.1172959e7 sec
Load Avg:  1.0029296875  1.00048828125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18226794 s          0 s    3820800 s  1092085417 s         35 s
#2  3501 MHz   48756092 s          0 s    2429552 s  1065381852 s          5 s
#3  3501 MHz   16886600 s          0 s    2102615 s  1097770897 s         22 s
#4  3501 MHz   14569483 s          0 s    2127396 s  1100034116 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.869
Commit d2db55a (2016-10-03 18:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13961.0703125 MB free)
Uptime: 1.1177625e7 sec
Load Avg:  0.9228515625  0.97802734375  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   18262906 s          0 s    3827473 s  1092507690 s         35 s
#2  3501 MHz   48950802 s          0 s    2436755 s  1065645853 s          5 s
#3  3501 MHz   17040152 s          0 s    2113104 s  1098072764 s         22 s
#4  3501 MHz   14621078 s          0 s    2134030 s  1100441805 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
