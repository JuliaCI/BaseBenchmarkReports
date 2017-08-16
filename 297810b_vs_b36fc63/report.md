# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@297810b01a3c378784be67a69bac17ffa89cdb18](https://github.com/pkofod/julia/commit/297810b01a3c378784be67a69bac17ffa89cdb18) vs [JuliaLang/julia@b36fc63257313e45a4d63458b0cfa51dda80d9d5](https://github.com/JuliaLang/julia/commit/b36fc63257313e45a4d63458b0cfa51dda80d9d5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23283#issuecomment-322873216)

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
| `["array","convert",("Int","Complex{Float64}")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.99 (25%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","acos",("one","negative argument","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("small","negative argument","Float32")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("small","positive argument","Float32")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("small","positive argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("zero","Float32")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("zero","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float64","sin_kernel")]` | 1.86 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(4,4))]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(8,8))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
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
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1366
Commit 297810b (2017-08-16 18:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   80386824 s          0 s   12379944 s  3755276085 s        138 s
       #2  3501 MHz  321919108 s          0 s   13513340 s  3514146668 s         49 s
       #3  3501 MHz   68546970 s          0 s    7832823 s  3778422997 s         66 s
       #4  3501 MHz   63881530 s          0 s    7770818 s  3783505129 s         23 s
       
  Memory: 31.383651733398438 GB (5565.875 MB free)
  Uptime: 3.8564921e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1364
Commit b36fc63 (2017-08-16 18:55 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   80466418 s          0 s   12389296 s  3755888907 s        141 s
       #2  3501 MHz  322546436 s          0 s   13524273 s  3514212426 s         49 s
       #3  3501 MHz   68623723 s          0 s    7840377 s  3779042590 s         66 s
       #4  3501 MHz   63977575 s          0 s    7778049 s  3784105962 s         23 s
       
  Memory: 31.383651733398438 GB (4991.1796875 MB free)
  Uptime: 3.8571968e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
