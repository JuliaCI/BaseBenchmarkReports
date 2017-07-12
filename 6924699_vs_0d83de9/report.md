# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6924699e00a701d3042ea0b9ea10c6396c6023a5](https://github.com/JuliaLang/julia/commit/6924699e00a701d3042ea0b9ea10c6396c6023a5) vs [JuliaLang/julia@0d83de93eb208e71aa5701329551939715268658](https://github.com/JuliaLang/julia/commit/0d83de93eb208e71aa5701329551939715268658)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22612#issuecomment-314742438)

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
| `["array","convert",("Complex{Float64}","Int")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 0.99 (30%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","logical",10)]` | 1.01 (30%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 1.04 (30%)  | 1.05 (1%) :x: |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.08 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 0.99 (30%)  | 1.10 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 1.07 (30%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.96 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.98 (30%)  | 1.77 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.13 (30%)  | 1.19 (1%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.17 (30%)  | 1.14 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.05 (30%)  | 1.64 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 0.98 (30%)  | 1.77 (1%) :x: |

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
Julia Version 0.7.0-DEV.923
Commit 6924699 (2017-07-12 09:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   73447019 s          0 s   11231681 s  3458779028 s        113 s
       #2  3501 MHz  290244398 s          0 s   12495927 s  3241816699 s         41 s
       #3  3501 MHz   63081627 s          0 s    7311008 s  3479057819 s         56 s
       #4  3501 MHz   58491839 s          0 s    7242906 s  3484051198 s         19 s
       
  Memory: 31.383651733398438 GB (21402.984375 MB free)
  Uptime: 3.5510461e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.921
Commit 0d83de9 (2017-07-12 08:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   73525644 s          0 s   11240946 s  3459228056 s        113 s
       #2  3501 MHz  290728060 s          0 s   12504220 s  3241863262 s         41 s
       #3  3501 MHz   63160363 s          0 s    7318579 s  3479509792 s         57 s
       #4  3501 MHz   58586215 s          0 s    7250670 s  3484487570 s         19 s
       
  Memory: 31.383651733398438 GB (20976.84765625 MB free)
  Uptime: 3.5515852e7 sec
  Load Avg:  1.2431640625  1.064453125  1.0615234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
