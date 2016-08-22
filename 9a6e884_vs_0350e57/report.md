# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9a6e884f9f1bcee065fdb2705a687d521f2e4aa6](https://github.com/JuliaLang/julia/commit/9a6e884f9f1bcee065fdb2705a687d521f2e4aa6) vs [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/9a6e884f9f1bcee065fdb2705a687d521f2e4aa6#commitcomment-18718506)

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
| `["array","cat",("catnd",5)]` | 0.88 (15%)  | 0.94 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.42 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.61 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.83 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc2+33
Commit 9a6e884 (2016-08-20 06:56 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20737.71875 MB free)
Uptime: 7.475015e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12024432 s          0 s    2518110 s  730820568 s         24 s
#2  3501 MHz   30455900 s          0 s    1524023 s  715007312 s          3 s
#3  3501 MHz   10588847 s          0 s    1340492 s  735214443 s         14 s
#4  3501 MHz    9118328 s          0 s    1340882 s  736673993 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-rc2+0
Commit 0350e57 (2016-08-12 11:25 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20480.9453125 MB free)
Uptime: 7.479676e6 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12073939 s          0 s    2524926 s  731228975 s         24 s
#2  3501 MHz   30665298 s          0 s    1531044 s  715256624 s          3 s
#3  3501 MHz   10626085 s          0 s    1346625 s  735636439 s         14 s
#4  3501 MHz    9257706 s          0 s    1351516 s  736989642 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
