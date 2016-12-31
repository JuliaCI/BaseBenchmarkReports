# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ed8525a56fe7430928c5d46fc0309cbb99fb538a](https://github.com/JuliaLang/julia/commit/ed8525a56fe7430928c5d46fc0309cbb99fb538a) vs [JuliaLang/julia@ab984a5b44ddb1b9af45ea66f2b8cb01df7f25a0](https://github.com/JuliaLang/julia/commit/ab984a5b44ddb1b9af45ea66f2b8cb01df7f25a0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269836342)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.99 (15%)  | 0.79 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.96 (15%)  | 0.75 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 1.00 (15%)  | 0.92 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 1.01 (15%)  | 0.79 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.99 (15%)  | 0.90 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.98 (15%)  | 0.75 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.99 (15%)  | 0.78 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.99 (15%)  | 0.78 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.99 (15%)  | 0.78 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.58 (15%) :white_check_mark: | 0.63 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.73 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["io","read","readstring"]` | 1.41 (15%) :x: | 1.33 (1%) :x: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.29 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.38 (15%) :white_check_mark: | 1.11 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 1.47 (45%) :x: | 1.00 (1%)  |
| `["micro","parseint"]` | 0.94 (15%)  | 1.14 (1%) :x: |
| `["micro","randmatstat"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 0.97 (15%)  | 0.76 (1%) :white_check_mark: |
| `["problem","imdb","centrality"]` | 0.75 (15%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.74 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.60 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["shootout","fasta"]` | 0.97 (15%)  | 0.90 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.63 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["shootout","regex_dna"]` | 1.02 (15%)  | 1.79 (1%) :x: |
| `["shootout","revcomp"]` | 1.02 (25%)  | 0.97 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.32 (20%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.91 (40%)  | 1.74 (1%) :x: |
| `["string","replace"]` | 0.83 (15%) :white_check_mark: | 1.81 (1%) :x: |

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
Memory: 31.383651733398438 GB (4456.53515625 MB free)
Uptime: 1.8795526e7 sec
Load Avg:  1.00439453125  1.0146484375  1.02001953125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26251748 s          0 s    6113846 s  1841811788 s         59 s
#2  3501 MHz   83869658 s          0 s    3736185 s  1790826900 s          8 s
#3  3501 MHz   24974420 s          0 s    3216245 s  1850493415 s         40 s
#4  3501 MHz   22562247 s          0 s    3309855 s  1852793806 s          7 s

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
Memory: 31.383651733398438 GB (4494.34375 MB free)
Uptime: 1.8801794e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   26394930 s          0 s    6124735 s  1842282706 s         59 s
#2  3501 MHz   84226321 s          0 s    3744382 s  1791088221 s          8 s
#3  3501 MHz   25014643 s          0 s    3223126 s  1851072223 s         40 s
#4  3501 MHz   22616456 s          0 s    3317275 s  1853358407 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
