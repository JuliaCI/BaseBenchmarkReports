# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@437f4f339dc7c90e53fcc5877396b12cffdbe429](https://github.com/JuliaLang/julia/commit/437f4f339dc7c90e53fcc5877396b12cffdbe429)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/437f4f339dc7c90e53fcc5877396b12cffdbe429#commitcomment-18584669)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-10 vs 2016-08-04

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
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.82 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.82 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",2)]` | 0.87 (15%)  | 1.02 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 0.87 (15%)  | 1.02 (1%) :x: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.07 (15%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.04 (25%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","descending")]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.135
Commit 437f4f3 (2016-08-10 03:10 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19576.3359375 MB free)
Uptime: 6.451523e6 sec
Load Avg:  1.0703125  1.0302734375  1.00732421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9052164 s          0 s    2067857 s  632165770 s         22 s
#2  3501 MHz   22555318 s          0 s    1163447 s  620983533 s          2 s
#3  3501 MHz    8420152 s          0 s    1057491 s  635378463 s         11 s
#4  3501 MHz    6833436 s          0 s    1035466 s  636974772 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
