# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@05e0e59ba3a9e6e64a537ba2c00fec9a87d0b7bf](https://github.com/mbauman/julia/commit/05e0e59ba3a9e6e64a537ba2c00fec9a87d0b7bf) vs [JuliaLang/julia@9cd522c948b4c1e4d4d75eeaa402dbfbe7d1ebe7](https://github.com/JuliaLang/julia/commit/9cd522c948b4c1e4d4d75eeaa402dbfbe7d1ebe7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19958#issuecomment-271602361)

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
| `["array","index",("sumcolon","1.0:1.0:100000.0")]` | 2.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","100000:-1:1")]` | 17.38 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","1:100000")]` | 2.95 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000)")]` | 1.80 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 1.70 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","100000:-1:1")]` | 4.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","1:100000")]` | 1.72 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000)")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:100000.0")]` | 2.35 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000:-1:1")]` | 17.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1:100000")]` | 3.08 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","linspace(1.0,2.0,10000)")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.95 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.98 (15%)  | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 1.01 (15%)  | 0.89 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.95 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.00 (15%)  | 0.87 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.97 (15%)  | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.96 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.96 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.97 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.54 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.69 (15%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.37 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.42 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["micro","parseint"]` | 0.88 (15%)  | 0.86 (1%) :white_check_mark: |
| `["misc","parse","DateTime"]` | 0.98 (15%)  | 0.73 (1%) :white_check_mark: |
| `["misc","parse","Int"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 0.90 (15%)  | 0.84 (1%) :white_check_mark: |
| `["problem","imdb","centrality"]` | 0.77 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.78 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_devec"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.61 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["scalar","floatexp",("exp","normal path, k = 2","Float 64")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","fasta"]` | 0.94 (15%)  | 0.90 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.61 (15%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.97 (15%)  | 1.05 (1%) :x: |
| `["shootout","revcomp"]` | 1.05 (25%)  | 0.97 (1%) :white_check_mark: |
| `["string","replace"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

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
?
```

#### Comparison Build

```
Julia Version 0.6.0-dev.1944
Commit 9cd522c (2017-01-07 17:37 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2081.71484375 MB free)
Uptime: 1.9721722e7 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   30622366 s          0 s    6718684 s  1929184476 s         61 s
#2  3501 MHz  101443750 s          0 s    4131927 s  1865424672 s          8 s
#3  3501 MHz   28066548 s          0 s    3562711 s  1939617309 s         42 s
#4  3501 MHz   25892401 s          0 s    3674923 s  1941669041 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
