# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@dbff9fd5c0028571ef1765ce950d34b6d57e3a2a](https://github.com/JuliaLang/julia/commit/dbff9fd5c0028571ef1765ce950d34b6d57e3a2a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/dbff9fd5c0028571ef1765ce950d34b6d57e3a2a#commitcomment-20402472)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-01-09 vs 2017-01-08

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
| `["dates","parse","Date"]` | 0.93 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.92 (15%)  | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.94 (15%)  | 0.89 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.92 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.95 (15%)  | 0.87 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.92 (15%)  | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.91 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.93 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.90 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.55 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.70 (15%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.35 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.35 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["micro","parseint"]` | 0.88 (15%)  | 0.86 (1%) :white_check_mark: |
| `["misc","parse","DateTime"]` | 0.93 (15%)  | 0.73 (1%) :white_check_mark: |
| `["misc","parse","Int"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 0.73 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.69 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["problem","spellcheck","spellcheck"]` | 0.59 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["shootout","fasta"]` | 1.02 (15%)  | 0.90 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.58 (15%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.96 (15%)  | 1.05 (1%) :x: |
| `["shootout","revcomp"]` | 0.99 (25%)  | 0.97 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1997
Commit dbff9fd (2017-01-08 22:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2733.453125 MB free)
Uptime: 1.9590418e7 sec
Load Avg:  1.0029296875  1.0146484375  0.98681640625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   35552273 s          0 s    5610572 s  1913891096 s         58 s
#2  3501 MHz  112518149 s          0 s    6607151 s  1836663247 s         20 s
#3  3501 MHz   30979532 s          0 s    3813288 s  1923335035 s         34 s
#4  3501 MHz   26508490 s          0 s    3709895 s  1928081982 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
