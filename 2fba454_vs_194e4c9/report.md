# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@2fba454060836686ded45e498fc85f49b9e6bc6e](https://github.com/pabloferz/julia/commit/2fba454060836686ded45e498fc85f49b9e6bc6e) vs [JuliaLang/julia@194e4c96fec2e3ff8203cae1c9d8ffaf3dc3e61c](https://github.com/JuliaLang/julia/commit/194e4c96fec2e3ff8203cae1c9d8ffaf3dc3e61c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19639#issuecomment-268135568)

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
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.85 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 1.02 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 0.99 (15%)  | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.81 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.80 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.95 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.94 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.95 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 0.60 (45%)  | 0.33 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.80 (45%)  | 0.32 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 0.60 (45%)  | 0.33 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.80 (45%)  | 0.32 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.66 (45%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 0.84 (45%)  | 0.68 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.72 (45%)  | 0.72 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 0.87 (45%)  | 0.72 (1%) :white_check_mark: |
| `["scalar","floatexp",("exponent","norm","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 0.89 (15%)  | 0.86 (1%) :white_check_mark: |

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
Julia Version 0.6.0-dev.1630
Commit 2fba454 (2016-12-20 01:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9613.828125 MB free)
Uptime: 1.7851752e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27890457 s          0 s    4629399 s  1749040184 s         54 s
#2  3501 MHz   82513382 s          0 s    5652213 s  1694051905 s         20 s
#3  3501 MHz   24649397 s          0 s    3133208 s  1756579097 s         29 s
#4  3501 MHz   20628895 s          0 s    3043074 s  1760833665 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1626
Commit 194e4c9 (2016-12-20 00:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9390.43359375 MB free)
Uptime: 1.7857695e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27996102 s          0 s    4639678 s  1749516875 s         54 s
#2  3501 MHz   82870016 s          0 s    5660598 s  1694280543 s         20 s
#3  3501 MHz   24701337 s          0 s    3140328 s  1757113535 s         29 s
#4  3501 MHz   20677272 s          0 s    3049825 s  1761372210 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
