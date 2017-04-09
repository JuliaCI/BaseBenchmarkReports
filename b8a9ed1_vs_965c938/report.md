# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@b8a9ed1c76eaf4c54f57c2850ce73c9ebc37fece](https://github.com/pabloferz/julia/commit/b8a9ed1c76eaf4c54f57c2850ce73c9ebc37fece) vs [JuliaLang/julia@965c938eb933f9850f55dcebf12198952ba34b62](https://github.com/JuliaLang/julia/commit/965c938eb933f9850f55dcebf12198952ba34b62)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21331#issuecomment-292756446)

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
| `["array","bool","boolarray_true_load!"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.41 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.62 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 0.35 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 0.38 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 0.39 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 0.59 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",10)]` | 0.73 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",3)]` | 0.39 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",5)]` | 0.70 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.beta.85
Commit b8a9ed1 (2017-04-08 22:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2694.9765625 MB free)
Uptime: 2.7351283e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52928644 s          0 s   10342013 s  2663914517 s         74 s
#2  3501 MHz  210486074 s          0 s    6354543 s  2516694305 s         11 s
#3  3501 MHz   46875460 s          0 s    5621027 s  2681322870 s         57 s
#4  3501 MHz   44319834 s          0 s    5756358 s  2683748766 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.83
Commit 965c938 (2017-04-08 21:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2435.91015625 MB free)
Uptime: 2.7356596e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53013005 s          0 s   10351466 s  2664350053 s         74 s
#2  3501 MHz  210960640 s          0 s    6363190 s  2516741807 s         11 s
#3  3501 MHz   46959354 s          0 s    5629283 s  2681761360 s         57 s
#4  3501 MHz   44411689 s          0 s    5764539 s  2684179514 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
