# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3afedd0d8f7d487354932f63c61affca9384f9a6](https://github.com/JuliaLang/julia/commit/3afedd0d8f7d487354932f63c61affca9384f9a6) vs [JuliaLang/julia@35ce0fdb962c34fcb7f4086854c6742c009050c5](https://github.com/JuliaLang/julia/commit/35ce0fdb962c34fcb7f4086854c6742c009050c5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20726#issuecomment-281563412)

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
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.63 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 1.65 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 1.49 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 1.66 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 1.47 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2899
Commit 3afedd0 (2017-02-22 04:08 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8581.60546875 MB free)
Uptime: 2.3388341e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   47924982 s          0 s    7393924 s  2278601595 s         69 s
#2  3501 MHz  157830767 s          0 s    7927908 s  2169247094 s         24 s
#3  3501 MHz   39030322 s          0 s    4631570 s  2294109545 s         38 s
#4  3501 MHz   34925674 s          0 s    4568531 s  2298495542 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2897
Commit 35ce0fd (2017-02-22 00:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8349.953125 MB free)
Uptime: 2.3394543e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   48020324 s          0 s    7403808 s  2279114402 s         69 s
#2  3501 MHz  158393556 s          0 s    7936320 s  2169295471 s         24 s
#3  3501 MHz   39113032 s          0 s    4639840 s  2294637976 s         38 s
#4  3501 MHz   35010303 s          0 s    4576629 s  2299022513 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
