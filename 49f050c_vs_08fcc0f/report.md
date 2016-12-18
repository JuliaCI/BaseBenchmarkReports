# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@49f050c5d52e9dc2be1b00844f07bf53959d7083](https://github.com/pabloferz/julia/commit/49f050c5d52e9dc2be1b00844f07bf53959d7083) vs [JuliaLang/julia@08fcc0fb90b555cef6b4ffa8540f62bade7cc57f](https://github.com/JuliaLang/julia/commit/08fcc0fb90b555cef6b4ffa8540f62bade7cc57f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19639#issuecomment-267818210)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","index","5d"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.85 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 1.00 (15%)  | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 0.99 (15%)  | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.82 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.81 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.90 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.90 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.91 (45%)  | 0.99 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 1.09 (15%)  | 0.99 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.69 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",100)]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.73 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1608
Commit 49f050c (2016-12-18 02:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9695.44921875 MB free)
Uptime: 1.7715221e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27543183 s          0 s    4575300 s  1735818364 s         53 s
#2  3501 MHz   80598954 s          0 s    5585839 s  1682398452 s         20 s
#3  3501 MHz   24372387 s          0 s    3093904 s  1743251593 s         29 s
#4  3501 MHz   20293963 s          0 s    2999578 s  1747565290 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1606
Commit 08fcc0f (2016-12-18 02:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9380.46875 MB free)
Uptime: 1.772197e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27581683 s          0 s    4582861 s  1736445037 s         53 s
#2  3501 MHz   81067900 s          0 s    5599536 s  1682590208 s         20 s
#3  3501 MHz   24430679 s          0 s    3100633 s  1743860583 s         29 s
#4  3501 MHz   20367725 s          0 s    3008114 s  1748157351 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
