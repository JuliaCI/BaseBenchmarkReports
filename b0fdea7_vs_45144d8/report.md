# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b0fdea708a3c3514730ceed1d95aba9fe8c0d3bc](https://github.com/JuliaLang/julia/commit/b0fdea708a3c3514730ceed1d95aba9fe8c0d3bc) vs [JuliaLang/julia@45144d811aedf9e705e2081c3ae582b76a2edd26](https://github.com/JuliaLang/julia/commit/45144d811aedf9e705e2081c3ae582b76a2edd26)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23117#issuecomment-320338860)

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
| `["array","cat",("catnd",5)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 0.36 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.32 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","readstring"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","julia",("macroexpand","evalpoly")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 0.03 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 2.86 (50%) :x: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 0.88 (15%)  | 0.98 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.92 (25%)  | 0.98 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.93 (25%)  | 1.02 (1%) :x: |
| `["random","types",("rand","RandomDevice","Int64")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randexp","RandomDevice","Float64")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn","MersenneTwister","Complex{Float32}")]` | 0.56 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn","MersenneTwister","Complex{Float64}")]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn","MersenneTwister","Float64")]` | 2.22 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randn","RandomDevice","Float64")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","BigInt")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","Bool")]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","Int64")]` | 1.51 (40%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","UInt64")]` | 0.52 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","Bool","Int64")]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","Int64","Int64")]` | 0.52 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","UInt64","UInt64")]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","cos_kernel")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 6π/4","positive argument","Float32","cos_kernel")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","arithmetic"]`
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
Julia Version 0.7.0-DEV.1240
Commit b0fdea7 (2017-08-04 18:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82520060 s          0 s   14911202 s  3644455917 s         86 s
       #2  3501 MHz  338312156 s          0 s    9350996 s  3403002052 s         13 s
       #3  3501 MHz   71702701 s          0 s    8276526 s  3671075584 s         73 s
       #4  3501 MHz   68398015 s          0 s    8468574 s  3674171129 s         17 s
       
  Memory: 31.383651733398438 GB (2814.1640625 MB free)
  Uptime: 3.7528512e7 sec
  Load Avg:  1.0205078125  1.0283203125  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1238
Commit 45144d8 (2017-08-04 18:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82610454 s          0 s   14920193 s  3644948238 s         86 s
       #2  3501 MHz  338847337 s          0 s    9361828 s  3403049411 s         13 s
       #3  3501 MHz   71781182 s          0 s    8283694 s  3671583262 s         73 s
       #4  3501 MHz   68476648 s          0 s    8475632 s  3674678876 s         17 s
       
  Memory: 31.383651733398438 GB (2434.51953125 MB free)
  Uptime: 3.7534451e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
