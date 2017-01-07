# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@7521b32f6f17bbfbd721adde91430a56811c9252](https://github.com/pabloferz/julia/commit/7521b32f6f17bbfbd721adde91430a56811c9252) vs [JuliaLang/julia@f4ed16b36bf300fd1192b7a473f9b0270cad816a](https://github.com/JuliaLang/julia/commit/f4ed16b36bf300fd1192b7a473f9b0270cad816a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19913#issuecomment-271053862)

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
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.74 (15%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.63 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.58 (15%) :white_check_mark: | 0.52 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.63 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.72 (15%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.63 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.58 (15%) :white_check_mark: | 0.52 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.63 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.69 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.26 (20%) :x: | 1.00 (1%)  |

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
- `["broadcast","sparse"]`
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

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1975
Commit 7521b32 (2017-01-07 01:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3972.96484375 MB free)
Uptime: 1.9406631e7 sec
Load Avg:  0.93603515625  1.00439453125  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   34935954 s          0 s    5527011 s  1896248993 s         58 s
#2  3501 MHz  108864988 s          0 s    6511657 s  1822067242 s         20 s
#3  3501 MHz   30332392 s          0 s    3746780 s  1905679672 s         33 s
#4  3501 MHz   25847531 s          0 s    3638275 s  1910443572 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1973
Commit f4ed16b (2017-01-06 23:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3528.453125 MB free)
Uptime: 1.941389e7 sec
Load Avg:  1.0029296875  1.0146484375  0.99560546875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   35002636 s          0 s    5536866 s  1896896111 s         58 s
#2  3501 MHz  109377415 s          0 s    6521953 s  1822269787 s         20 s
#3  3501 MHz   30390958 s          0 s    3753001 s  1906339790 s         33 s
#4  3501 MHz   25903134 s          0 s    3646047 s  1911105479 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
