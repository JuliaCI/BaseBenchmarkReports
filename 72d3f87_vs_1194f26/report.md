# Benchmark Report

## Job Properties

*Commit(s):* [alyst/julia@72d3f87d11c5f1a830b78d7943902fc745acab8e](https://github.com/alyst/julia/commit/72d3f87d11c5f1a830b78d7943902fc745acab8e) vs [JuliaLang/julia@1194f26db4204ef6a8651f007f3b7461e850ce58](https://github.com/JuliaLang/julia/commit/1194f26db4204ef6a8651f007f3b7461e850ce58)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21938#issuecomment-302474183)

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
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","read"]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Hermitian",256)]` | 0.99 (45%)  | 1.03 (1%) :x: |
| `["linalg","factorization",("eig","Matrix",256)]` | 0.99 (45%)  | 1.03 (1%) :x: |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 1.00 (45%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 1.00 (45%)  | 1.07 (1%) :x: |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 0.99 (45%)  | 1.03 (1%) :x: |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 1.00 (45%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 1.00 (45%)  | 1.07 (1%) :x: |
| `["linalg","factorization",("schur","Matrix",1024)]` | 1.01 (45%)  | 1.01 (1%) :x: |
| `["linalg","factorization",("schur","Matrix",256)]` | 0.99 (45%)  | 1.05 (1%) :x: |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 0.97 (45%)  | 1.01 (1%) :x: |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 0.99 (45%)  | 1.05 (1%) :x: |
| `["linalg","factorization",("svd","LowerTriangular",1024)]` | 0.98 (45%)  | 1.12 (1%) :x: |
| `["linalg","factorization",("svd","LowerTriangular",256)]` | 1.00 (45%)  | 1.12 (1%) :x: |
| `["linalg","factorization",("svd","Matrix",1024)]` | 0.99 (45%)  | 1.14 (1%) :x: |
| `["linalg","factorization",("svd","Matrix",256)]` | 1.00 (45%)  | 1.14 (1%) :x: |
| `["linalg","factorization",("svd","UpperTriangular",1024)]` | 0.99 (45%)  | 1.12 (1%) :x: |
| `["linalg","factorization",("svd","UpperTriangular",256)]` | 1.00 (45%)  | 1.12 (1%) :x: |
| `["linalg","factorization",("svdfact","LowerTriangular",1024)]` | 0.98 (45%)  | 1.14 (1%) :x: |
| `["linalg","factorization",("svdfact","LowerTriangular",256)]` | 1.00 (45%)  | 1.14 (1%) :x: |
| `["linalg","factorization",("svdfact","Matrix",1024)]` | 0.98 (45%)  | 1.17 (1%) :x: |
| `["linalg","factorization",("svdfact","Matrix",256)]` | 1.00 (45%)  | 1.16 (1%) :x: |
| `["linalg","factorization",("svdfact","UpperTriangular",1024)]` | 1.02 (45%)  | 1.14 (1%) :x: |
| `["linalg","factorization",("svdfact","UpperTriangular",256)]` | 1.00 (45%)  | 1.14 (1%) :x: |
| `["simd",("sum_reduce","Float32",4096)]` | 1.33 (20%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.237
Commit 72d3f87 (2017-05-18 16:14 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7881.1640625 MB free)
Uptime: 3.0778116e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   64287282 s          0 s    9916892 s  2997001121 s         89 s
#2  3501 MHz  249433984 s          0 s   10909099 s  2811831779 s         36 s
#3  3501 MHz   55198632 s          0 s    6421343 s  3014798604 s         47 s
#4  3501 MHz   50786771 s          0 s    6368015 s  3019547527 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.234
Commit 1194f26 (2017-05-18 16:11 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7675.015625 MB free)
Uptime: 3.0783282e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   64371916 s          0 s    9926852 s  2997421201 s         89 s
#2  3501 MHz  249891732 s          0 s   10918134 s  2811880974 s         36 s
#3  3501 MHz   55296102 s          0 s    6429884 s  3015208481 s         47 s
#4  3501 MHz   50875489 s          0 s    6376539 s  3019966265 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
