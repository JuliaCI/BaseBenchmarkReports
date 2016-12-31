# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ed8525a56fe7430928c5d46fc0309cbb99fb538a](https://github.com/JuliaLang/julia/commit/ed8525a56fe7430928c5d46fc0309cbb99fb538a) vs [JuliaLang/julia@ab984a5b44ddb1b9af45ea66f2b8cb01df7f25a0](https://github.com/JuliaLang/julia/commit/ab984a5b44ddb1b9af45ea66f2b8cb01df7f25a0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269833204)

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
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.85 (30%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",2048)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.93 (15%)  | 0.79 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.93 (15%)  | 0.75 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.97 (15%)  | 0.92 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.92 (15%)  | 0.79 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.96 (15%)  | 0.90 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.92 (15%)  | 0.75 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.92 (15%)  | 0.78 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.92 (15%)  | 0.78 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.93 (15%)  | 0.78 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.59 (15%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.68 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["io","read","readstring"]` | 1.39 (15%) :x: | 1.33 (1%) :x: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.29 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.36 (15%) :white_check_mark: | 1.11 (1%) :x: |
| `["micro","parseint"]` | 0.95 (15%)  | 1.14 (1%) :x: |
| `["misc","parse","DateTime"]` | 0.85 (15%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["misc","parse","Int"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 0.68 (15%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.72 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["problem","spellcheck","spellcheck"]` | 0.56 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["shootout","fasta"]` | 0.92 (15%)  | 0.90 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.59 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 1.02 (15%)  | 1.79 (1%) :x: |
| `["shootout","revcomp"]` | 1.01 (25%)  | 0.97 (1%) :white_check_mark: |
| `["string","join"]` | 0.94 (40%)  | 1.74 (1%) :x: |
| `["string","replace"]` | 0.82 (15%) :white_check_mark: | 1.81 (1%) :x: |

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
Julia Version 0.6.0-dev.1792
Commit ed8525a (2016-12-30 15:08 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2494.484375 MB free)
Uptime: 1.8791341e7 sec
Load Avg:  0.9228515625  0.9853515625  0.95654296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   31624968 s          0 s    5093282 s  1838611871 s         55 s
#2  3501 MHz   95434392 s          0 s    6117459 s  1774455265 s         20 s
#3  3501 MHz   26945185 s          0 s    3413478 s  1847913484 s         31 s
#4  3501 MHz   22918246 s          0 s    3320445 s  1852191945 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1797
Commit ab984a5 (2016-12-30 17:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3553.4609375 MB free)
Uptime: 1.8797974e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   31693925 s          0 s    5102027 s  1839195525 s         55 s
#2  3501 MHz   95803656 s          0 s    6124906 s  1774740992 s         20 s
#3  3501 MHz   27044646 s          0 s    3422420 s  1848467640 s         31 s
#4  3501 MHz   23010412 s          0 s    3329669 s  1852753287 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
