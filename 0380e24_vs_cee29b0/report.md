# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0380e248dfbd792f156890aa3cff8b348786ac8f](https://github.com/JuliaLang/julia/commit/0380e248dfbd792f156890aa3cff8b348786ac8f) vs [JuliaLang/julia@cee29b014105a8408f4d2f6de459aba80d403d3c](https://github.com/JuliaLang/julia/commit/cee29b014105a8408f4d2f6de459aba80d403d3c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20343#issuecomment-279323444)

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
| `["array","cat",("hvcat_setind",5)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.11 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.11 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2809
Commit 0380e24 (2017-02-13 07:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13802.64453125 MB free)
Uptime: 2.2626789e7 sec
Load Avg:  1.076171875  1.03076171875  1.05029296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   46064024 s          0 s    7166129 s  2204674735 s         67 s
#2  3501 MHz  147955880 s          0 s    7603148 s  2103460894 s         22 s
#3  3501 MHz   37444848 s          0 s    4475648 s  2219720455 s         38 s
#4  3501 MHz   33394656 s          0 s    4404432 s  2224056281 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2805
Commit cee29b0 (2017-02-13 07:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13679.38671875 MB free)
Uptime: 2.2632519e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   46147922 s          0 s    7175716 s  2205152129 s         67 s
#2  3501 MHz  148475482 s          0 s    7611497 s  2103505367 s         22 s
#3  3501 MHz   37537830 s          0 s    4484061 s  2220191330 s         38 s
#4  3501 MHz   33476108 s          0 s    4412448 s  2224539249 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
