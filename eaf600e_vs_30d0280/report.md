# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@eaf600ec306955df9e83f3f8054c5417fb88dac8](https://github.com/JuliaLang/julia/commit/eaf600ec306955df9e83f3f8054c5417fb88dac8) vs [JuliaLang/julia@30d0280a6e03655c71050a3d2495dd7f96fdf145](https://github.com/JuliaLang/julia/commit/30d0280a6e03655c71050a3d2495dd7f96fdf145)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20374#issuecomment-278872325)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.11 (15%)  | 1.11 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.18 (15%) :x: | 1.14 (1%) :x: |
| `["io","serialization",("serialize","Vector{String}")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",1024)]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["shootout","fasta"]` | 1.26 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2747
Commit eaf600e (2017-02-10 06:59 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14040.5078125 MB free)
Uptime: 2.2363694e7 sec
Load Avg:  1.0029296875  1.0146484375  0.98681640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   45543730 s          0 s    7074582 s  2179042121 s         66 s
#2  3501 MHz  144737501 s          0 s    7522911 s  2080484181 s         22 s
#3  3501 MHz   36898721 s          0 s    4417560 s  2194028321 s         38 s
#4  3501 MHz   32901657 s          0 s    4349417 s  2198304894 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2739
Commit 30d0280 (2017-02-10 04:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13772.20703125 MB free)
Uptime: 2.2371616e7 sec
Load Avg:  1.0029296875  1.0146484375  0.99755859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   45635914 s          0 s    7085177 s  2179729006 s         66 s
#2  3501 MHz  145251492 s          0 s    7531256 s  2080753214 s         22 s
#3  3501 MHz   36985901 s          0 s    4424849 s  2194725112 s         38 s
#4  3501 MHz   32968440 s          0 s    4356861 s  2199022220 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
