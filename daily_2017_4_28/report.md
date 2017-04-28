# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d7c00faca48484adfb46db2b5b7fdfdb114a710f](https://github.com/JuliaLang/julia/commit/d7c00faca48484adfb46db2b5b7fdfdb114a710f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/d7c00faca48484adfb46db2b5b7fdfdb114a710f#commitcomment-21943645)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-04-28 vs 2017-04-27

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.60 (15%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.70 (15%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",1024)]` | 1.02 (15%)  | 0.65 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 1.03 (15%)  | 0.50 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 1.01 (15%)  | 0.81 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 1.01 (15%)  | 0.59 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.02 (15%)  | 0.52 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.20 (15%) :x: | 1.00 (1%)  |

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
- `["scalar","intfuncs"]`
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
Julia Version 0.6.0-pre.beta.392
Commit d7c00fa (2017-04-27 21:32 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2358.7421875 MB free)
Uptime: 2.9002648e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   57574216 s          0 s   11114916 s  2823137463 s         77 s
#2  3501 MHz  233694522 s          0 s    6910216 s  2657964949 s         11 s
#3  3501 MHz   51687716 s          0 s    6139382 s  2841044859 s         59 s
#4  3501 MHz   48943958 s          0 s    6285680 s  2843645797 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
