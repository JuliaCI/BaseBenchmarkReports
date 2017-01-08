# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1dabf759ffb3763ed6bdcc4615951f457e671acf](https://github.com/JuliaLang/julia/commit/1dabf759ffb3763ed6bdcc4615951f457e671acf) vs [JuliaLang/julia@28a11ffd4d2e8451492013f18dad5e9a576233f6](https://github.com/JuliaLang/julia/commit/28a11ffd4d2e8451492013f18dad5e9a576233f6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-271120284)

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
| `["dates","parse","Date"]` | 0.89 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.86 (15%)  | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.96 (15%)  | 0.89 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.90 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.95 (15%)  | 0.87 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.87 (15%)  | 0.73 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.91 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.91 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.90 (15%)  | 0.76 (1%) :white_check_mark: |
| `["dates","string","Date"]` | 0.54 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.69 (15%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.29 (15%) :white_check_mark: | 0.68 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.35 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["micro","parseint"]` | 0.87 (15%)  | 0.86 (1%) :white_check_mark: |
| `["misc","parse","DateTime"]` | 0.89 (15%)  | 0.73 (1%) :white_check_mark: |
| `["misc","parse","Int"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 0.68 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.72 (15%) :white_check_mark: | 0.42 (1%) :white_check_mark: |
| `["problem","spellcheck","spellcheck"]` | 0.62 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["shootout","fasta"]` | 0.94 (15%)  | 0.90 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.60 (15%) :white_check_mark: | 0.32 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.96 (15%)  | 1.05 (1%) :x: |
| `["shootout","revcomp"]` | 0.95 (25%)  | 0.97 (1%) :white_check_mark: |
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
Julia Version 0.6.0-dev.1986
Commit 1dabf75 (2017-01-07 23:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3714.81640625 MB free)
Uptime: 1.9488335e7 sec
Load Avg:  1.0830078125  1.0185546875  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   29467463 s          0 s    6567082 s  1907219301 s         60 s
#2  3501 MHz   96383492 s          0 s    4025978 s  1847266351 s          8 s
#3  3501 MHz   27226384 s          0 s    3468495 s  1917227566 s         41 s
#4  3501 MHz   24914171 s          0 s    3575412 s  1919421396 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1980
Commit 28a11ff (2017-01-07 17:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3577.96484375 MB free)
Uptime: 1.9495678e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   29593725 s          0 s    6578827 s  1907813172 s         60 s
#2  3501 MHz   96821442 s          0 s    4034026 s  1847554088 s          8 s
#3  3501 MHz   27283550 s          0 s    3475338 s  1917896922 s         41 s
#4  3501 MHz   24994033 s          0 s    3582851 s  1920067726 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
