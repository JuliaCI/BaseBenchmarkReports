# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@37383e4a8d2146df79a8641cabacaf3a3d6d156f](https://github.com/JuliaLang/julia/commit/37383e4a8d2146df79a8641cabacaf3a3d6d156f) vs [JuliaLang/julia@b3241d7845f136d1f400f7283ae37128250d2883](https://github.com/JuliaLang/julia/commit/b3241d7845f136d1f400f7283ae37128250d2883)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23939#issuecomment-333821569)

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
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 1.16 (15%) :x: | 3.00 (1%) :x: |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",10)]` | 52.35 (15%) :x: | 2.10 (1%) :x: |
| `["broadcast","typeargs",("array",3)]` | 65.34 (15%) :x: | 2.57 (1%) :x: |
| `["broadcast","typeargs",("array",5)]` | 69.78 (15%) :x: | 2.38 (1%) :x: |
| `["broadcast","typeargs",("tuple",10)]` | 19.27 (15%) :x: | Inf (1%) :x: |
| `["broadcast","typeargs",("tuple",3)]` | 55.14 (15%) :x: | Inf (1%) :x: |
| `["broadcast","typeargs",("tuple",5)]` | 27.42 (15%) :x: | Inf (1%) :x: |
| `["io","read","readstring"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 2.78 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 5.15 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 2.71 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 5.15 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 2.53 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 5.08 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 2.76 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 5.04 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 2.65 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 5.19 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 2.59 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 5.09 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 2.81 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 5.07 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 2.51 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 5.15 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 2.77 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 5.08 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 2.54 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 5.19 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 2.61 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 5.14 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 2.79 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 5.10 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 2.04 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 3.34 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.91 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 3.31 (45%) :x: | 1.08 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 2.09 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 3.41 (45%) :x: | 1.08 (1%) :x: |
| `["problem","raytrace","raytrace"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sparse","constructors",("Bidiagonal",1000)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.92 (40%) :x: | 1.00 (1%)  |

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
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
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
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","atan2"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2043
Commit 37383e4 (2017-10-03 06:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88092604 s          0 s   13686813 s  4157206681 s        177 s
       #2  3501 MHz  355157062 s          0 s   14681152 s  3891194251 s         62 s
       #3  3501 MHz   73704134 s          0 s    8421596 s  4184574951 s         84 s
       #4  3501 MHz   69019920 s          0 s    8297086 s  4189785026 s         30 s
       
  Memory: 31.383651733398438 GB (3504.17578125 MB free)
  Uptime: 4.2685296e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2039
Commit b3241d7 (2017-10-03 06:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88175156 s          0 s   13696428 s  4157774692 s        177 s
       #2  3501 MHz  355752833 s          0 s   14692919 s  3891248685 s         62 s
       #3  3501 MHz   73806977 s          0 s    8429270 s  4185126419 s         84 s
       #4  3501 MHz   69100382 s          0 s    8304899 s  4190358887 s         30 s
       
  Memory: 31.383651733398438 GB (3075.890625 MB free)
  Uptime: 4.2691924e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
