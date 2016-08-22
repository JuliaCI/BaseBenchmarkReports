# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@cc9396a1efadbcf8a2e7daf7e796cf59b19b2077](https://github.com/JuliaLang/julia/commit/cc9396a1efadbcf8a2e7daf7e796cf59b19b2077) vs [JuliaLang/julia@0350e5769b43f56c4c570741b0f5b2edf9399dc7](https://github.com/JuliaLang/julia/commit/0350e5769b43f56c4c570741b0f5b2edf9399dc7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18156#issuecomment-241404159)

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
| `["array","cat",("catnd_setind",5)]` | 1.00 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","cat",("hcat",5)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",500)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 0.73 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 1.00 (15%)  | 0.90 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.82 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumcartesian","BitArray{2}")]` | 1.37 (40%)  | 2.00 (1%) :x: |
| `["array","index",("sumeach","BitArray{2}")]` | 1.44 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumelt","BitArray{2}")]` | 1.48 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 1.41 (40%) :x: | 2.00 (1%) :x: |
| `["array","index",("sumlinear","BitArray{2}")]` | 1.43 (40%) :x: | 2.00 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.50 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.50 (15%) :white_check_mark: | 0.99 (1%)  |
| `["problem","go","go_game"]` | 0.93 (15%)  | 0.82 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{UInt64}")]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{UInt64}")]` | 1.43 (40%) :x: | 1.00 (1%)  |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 1.35 (1%) :x: |
| `["simd",("two_reductions","Int32",4095)]` | 1.35 (20%) :x: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 1.36 (20%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.38 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","integer",100000)]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",10000)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,10000))]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.0-rc2+115
Commit cc9396a (2016-08-22 12:55 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16214.375 MB free)
Uptime: 7.520643e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12737414 s          0 s    2262267 s  735351488 s         24 s
#2  3501 MHz   29908804 s          0 s    1919711 s  719404207 s          6 s
#3  3501 MHz   10899725 s          0 s    1388816 s  739378142 s         12 s
#4  3501 MHz    8545320 s          0 s    1347310 s  741835534 s          2 s

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
Memory: 31.383651733398438 GB (15944.55859375 MB free)
Uptime: 7.525313e6 sec
Load Avg:  1.0029296875  1.01220703125  0.95849609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   12805454 s          0 s    2269308 s  735742025 s         24 s
#2  3501 MHz   30115490 s          0 s    1928102 s  719655395 s          6 s
#3  3501 MHz   10940156 s          0 s    1394398 s  739798286 s         12 s
#4  3501 MHz    8667090 s          0 s    1356746 s  742170835 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
