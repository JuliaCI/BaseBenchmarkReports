# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3a311556050ee70e71c43c3ca6bc86165174da77](https://github.com/JuliaLang/julia/commit/3a311556050ee70e71c43c3ca6bc86165174da77)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/3a311556050ee70e71c43c3ca6bc86165174da77#commitcomment-19062968)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-09-17 vs 2016-09-16

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
| `["array","cat",("catnd",5)]` | 1.50 (15%) :x: | 1.10 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.02 (15%)  | 1.03 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 1.04 (15%)  | 1.03 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.04 (15%)  | 1.03 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 1.02 (40%)  | 1.08 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 0.98 (40%)  | 1.03 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 1.04 (40%)  | 1.07 (1%) :x: |
| `["array","index",("sumvector","BitArray{2}")]` | 1.04 (40%)  | 1.11 (1%) :x: |
| `["io","read","readstring"]` | 1.21 (15%) :x: | 1.17 (1%) :x: |
| `["micro","parseint"]` | 1.05 (15%)  | 1.11 (1%) :x: |
| `["parallel","remotecall",("identity",1024)]` | 1.03 (15%)  | 1.03 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.02 (15%)  | 1.04 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.02 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.04 (15%)  | 1.03 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.03 (15%)  | 1.04 (1%) :x: |
| `["problem","go","go_game"]` | 1.05 (15%)  | 1.12 (1%) :x: |
| `["problem","imdb","centrality"]` | 1.05 (15%)  | 1.03 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["shootout","fannkuch"]` | 1.03 (15%)  | 1.05 (1%) :x: |
| `["shootout","k_nucleotide"]` | 0.99 (15%)  | 1.13 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["shootout","nbody"]` | 1.00 (15%)  | 1.04 (1%) :x: |
| `["shootout","nbody_vec"]` | 1.10 (15%)  | 1.07 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 1.02 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 0.96 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 0.93 (15%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.02 (15%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.03 (15%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.00 (15%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 1.00 (15%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 0.98 (15%)  | 1.10 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 0.96 (15%)  | 1.10 (1%) :x: |
| `["sort","issorted",("forwards","ascending")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 0.96 (30%)  | 1.17 (1%) :x: |
| `["sort","issorted",("reverse","descending")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","issorted",("reverse","ones")]` | 1.00 (30%)  | 1.17 (1%) :x: |
| `["sort","issorted",("reverse","random")]` | 0.98 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.17 (15%) :x: | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.15 (15%) :x: | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 1.00 (15%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 1.00 (15%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.01 (15%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.00 (15%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 1.00 (15%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.00 (15%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 0.99 (15%)  | 1.10 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 0.99 (15%)  | 1.10 (1%) :x: |
| `["sparse","index",("spmat","array",10)]` | 1.01 (25%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","col","array",10)]` | 1.05 (15%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","col","array",100)]` | 1.03 (15%)  | 1.03 (1%) :x: |
| `["sparse","index",("spmat","col","logical",10)]` | 1.19 (15%) :x: | 1.13 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 0.99 (15%)  | 1.05 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 1.24 (15%) :x: | 1.13 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 1.27 (15%) :x: | 1.11 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 1.13 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","logical",10)]` | 1.15 (25%)  | 1.12 (1%) :x: |
| `["sparse","index",("spmat","logical",100)]` | 1.05 (25%)  | 1.01 (1%) :x: |
| `["sparse","index",("spmat","range",10)]` | 1.17 (25%)  | 1.05 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.12 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.95 (15%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 1.18 (25%)  | 1.15 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 1.04 (25%)  | 1.15 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.99 (25%)  | 1.09 (1%) :x: |
| `["sparse","index",("spvec","logical",1000)]` | 1.08 (15%)  | 1.02 (1%) :x: |
| `["sparse","index",("spvec","range",1000)]` | 1.11 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spvec","range",10000)]` | 1.18 (15%) :x: | 1.02 (1%) :x: |

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
Julia Version 0.6.0-dev.677
Commit 3a31155 (2016-09-16 21:18 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16432.09375 MB free)
Uptime: 9.734614e6 sec
Load Avg:  1.0078125  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16298521 s          0 s    3386962 s  950995694 s         30 s
#2  3501 MHz   42556763 s          0 s    2110558 s  928157014 s          4 s
#3  3501 MHz   14938469 s          0 s    1845839 s  956209433 s         20 s
#4  3501 MHz   12704235 s          0 s    1847608 s  958427224 s          3 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
