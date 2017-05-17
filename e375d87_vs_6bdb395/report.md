# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e375d87093831f5a34abc6dec0b40718ece48076](https://github.com/JuliaLang/julia/commit/e375d87093831f5a34abc6dec0b40718ece48076) vs [JuliaLang/julia@6bdb3950bdf64152](https://github.com/JuliaLang/julia/commit/6bdb3950bdf64152)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21878#issuecomment-302010108)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 2.21 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 2.21 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 2.24 (15%) :x: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","BigInt","+")]` | 0.37 (40%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["scalar","intfuncs",("nextpow2","BigInt","-")]` | 0.22 (40%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","BigInt","+")]` | 0.77 (40%)  | 0.71 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","BigInt","-")]` | 0.41 (40%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-rc1.81
Commit e375d87 (2017-05-17 07:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8209.31640625 MB free)
Uptime: 3.0658002e7 sec
Load Avg:  0.9267578125  1.0  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63397699 s          0 s    9812422 s  2986015559 s         89 s
#2  3501 MHz  246934304 s          0 s   10812452 s  2802431516 s         36 s
#3  3501 MHz   54304525 s          0 s    6329877 s  3003783623 s         46 s
#4  3501 MHz   49884042 s          0 s    6278855 s  3008536763 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-rc1.0
Commit 6bdb395 (2017-05-07 00:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7990.90625 MB free)
Uptime: 3.0663458e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63481259 s          0 s    9822695 s  2986465169 s         89 s
#2  3501 MHz  247421771 s          0 s   10821254 s  2802480190 s         36 s
#3  3501 MHz   54404733 s          0 s    6338430 s  3004219739 s         46 s
#4  3501 MHz   49969994 s          0 s    6287422 s  3008987197 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
