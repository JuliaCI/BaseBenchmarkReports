# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8d99c3af595a7f3b5ffc85b12483588dd166b30a](https://github.com/JuliaLang/julia/commit/8d99c3af595a7f3b5ffc85b12483588dd166b30a) vs [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18156#issuecomment-241189452)

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
| `["array","cat",("catnd_setind",5)]` | 1.01 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.81 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.93 (15%)  | 0.90 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.81 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumeach","100000000:-1:1")]` | 2.14 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000000")]` | 6.75 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","1:100000000")]` | 8.67 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 2.07 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000000")]` | 6.75 (40%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.55 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.55 (15%) :white_check_mark: | 0.99 (1%)  |
| `["problem","go","go_game"]` | 0.94 (15%)  | 0.82 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.31 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 1.26 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.36 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","integer",100000)]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",1000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
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
Julia Version 0.5.0-rc2+96
Commit 8d99c3a (2016-08-20 09:22 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10938.9296875 MB free)
Uptime: 7.33527e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11663847 s          0 s    2455396 s  717305328 s         23 s
#2  3501 MHz   29135726 s          0 s    1467493 s  702419162 s          3 s
#3  3501 MHz   10080229 s          0 s    1288646 s  721808567 s         14 s
#4  3501 MHz    8670633 s          0 s    1287446 s  723210966 s          2 s

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
Memory: 31.383651733398438 GB (10878.078125 MB free)
Uptime: 7.339935e6 sec
Load Avg:  1.0029296875  0.994140625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11705860 s          0 s    2461706 s  717721899 s         23 s
#2  3501 MHz   29404420 s          0 s    1477308 s  702606659 s          3 s
#3  3501 MHz   10163567 s          0 s    1296281 s  722183338 s         14 s
#4  3501 MHz    8713095 s          0 s    1293850 s  723627986 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
