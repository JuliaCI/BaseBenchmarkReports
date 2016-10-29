# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c55037a0fecb608c67d7de3f4fd4325f7402e576](https://github.com/JuliaLang/julia/commit/c55037a0fecb608c67d7de3f4fd4325f7402e576)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/c55037a0fecb608c67d7de3f4fd4325f7402e576#commitcomment-19620004)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-10-29 vs 2016-10-28

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
| `["array","cat",("hcat",5)]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 2.18 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 1.76 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 2.02 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("prerend!",2048)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 1.47 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.51 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.47 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.50 (45%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",100)]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 2.41 (30%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1146
Commit c55037a (2016-10-28 19:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12045.3671875 MB free)
Uptime: 1.336543e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20734702 s          0 s    4512677 s  1307489324 s         39 s
#2  3501 MHz   59427228 s          0 s    2816568 s  1273457843 s          6 s
#3  3501 MHz   19870944 s          0 s    2471827 s  1313560879 s         29 s
#4  3501 MHz   17079576 s          0 s    2479120 s  1316333177 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
