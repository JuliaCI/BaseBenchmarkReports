# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@510feeabecbd8fbac6d554b4760138d0f9c0c1b1](https://github.com/JuliaLang/julia/commit/510feeabecbd8fbac6d554b4760138d0f9c0c1b1) vs [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18156#issuecomment-241286883)

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
| `["array","cat",("catnd",5)]` | 0.89 (15%)  | 0.94 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 1.01 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.74 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.92 (15%)  | 0.90 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.82 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.54 (15%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.62 (25%) :white_check_mark: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 0.94 (15%)  | 0.82 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.34 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","integer",100000)]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["string","join"]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc2+111
Commit 510feea (2016-08-21 22:38 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20713.2421875 MB free)
Uptime: 7.473875e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12415924 s          0 s    2226949 s  731041646 s         24 s
#2  3501 MHz   29387590 s          0 s    1887643 s  715287009 s          6 s
#3  3501 MHz   10551236 s          0 s    1357341 s  735084986 s         12 s
#4  3501 MHz    8359398 s          0 s    1319663 s  737376440 s          2 s

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
Memory: 31.383651733398438 GB (20384.2734375 MB free)
Uptime: 7.478559e6 sec
Load Avg:  0.9228515625  0.998046875  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12471722 s          0 s    2234201 s  731445619 s         24 s
#2  3501 MHz   29577392 s          0 s    1894118 s  715558397 s          6 s
#3  3501 MHz   10678648 s          0 s    1367139 s  735415482 s         12 s
#4  3501 MHz    8424251 s          0 s    1327103 s  737771961 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
