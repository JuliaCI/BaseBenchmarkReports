# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f8afb93e83514325fecef0cedf9ffba18fe5261f](https://github.com/JuliaLang/julia/commit/f8afb93e83514325fecef0cedf9ffba18fe5261f) vs [JuliaLang/julia@6b2ae3665e59d1aeb4032915c98e2add14ee22c9](https://github.com/JuliaLang/julia/commit/6b2ae3665e59d1aeb4032915c98e2add14ee22c9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21684#issuecomment-298837515)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",2048)]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["io","read","readstring"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",1024)]` | 0.40 (45%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",256)]` | 0.38 (45%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["nullable","basic",("get2","Nullable{Float32}()")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_devec"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.2-pre+51
Commit f8afb93 (2017-05-03 06:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3547.359375 MB free)
Uptime: 2.944709e7 sec
Load Avg:  1.0830078125  1.03125  1.05078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60433616 s          0 s    9332231 s  2868654893 s         85 s
#2  3501 MHz  228013104 s          0 s   10302745 s  2700925927 s         34 s
#3  3501 MHz   51284373 s          0 s    5978666 s  2886128368 s         45 s
#4  3501 MHz   46817481 s          0 s    5920337 s  2890930024 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.2-pre+2
Commit 6b2ae36 (2017-05-03 02:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3279.46484375 MB free)
Uptime: 2.9452513e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60508101 s          0 s    9342066 s  2869110818 s         85 s
#2  3501 MHz  228503561 s          0 s   10311496 s  2700968399 s         34 s
#3  3501 MHz   51365487 s          0 s    5986482 s  2886581033 s         45 s
#4  3501 MHz   46904297 s          0 s    5928602 s  2891376676 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
