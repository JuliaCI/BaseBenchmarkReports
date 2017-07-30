# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@3fb750268f8286d7c1f52f4a2750b180b053f5c2](https://github.com/musm/julia/commit/3fb750268f8286d7c1f52f4a2750b180b053f5c2) vs [JuliaLang/julia@1ce3c8e60e82fffccfbd65d5d8a58c9314571915](https://github.com/JuliaLang/julia/commit/1ce3c8e60e82fffccfbd65d5d8a58c9314571915)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23046#issuecomment-318923101)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 0.98 (25%)  | 1.01 (1%) :x: |
| `["random","types",("rand","MersenneTwister","Int16")]` | 1.28 (25%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1166
Commit 3fb7502 (2017-07-30 19:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   76747194 s          0 s   11905943 s  3612860024 s        126 s
       #2  3501 MHz  299365960 s          0 s   12772371 s  3390869420 s         42 s
       #3  3501 MHz   64777270 s          0 s    7475365 s  3635756092 s         60 s
       #4  3501 MHz   60194983 s          0 s    7407993 s  3640750457 s         21 s
       
  Memory: 31.383651733398438 GB (5310.6640625 MB free)
  Uptime: 3.7096355e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1164
Commit 1ce3c8e (2017-07-29 16:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   76829015 s          0 s   11915274 s  3613444845 s        126 s
       #2  3501 MHz  299996816 s          0 s   12783407 s  3390905496 s         42 s
       #3  3501 MHz   64858165 s          0 s    7482910 s  3636345352 s         60 s
       #4  3501 MHz   60274119 s          0 s    7415327 s  3641341928 s         21 s
       
  Memory: 31.383651733398438 GB (4939.7578125 MB free)
  Uptime: 3.7103141e7 sec
  Load Avg:  1.05419921875  1.02880859375  1.04833984375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
