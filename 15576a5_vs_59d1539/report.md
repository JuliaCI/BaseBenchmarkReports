# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@15576a5aaec7b19a9cb05133e34cd07403cf527c](https://github.com/JuliaLang/julia/commit/15576a5aaec7b19a9cb05133e34cd07403cf527c) vs [JuliaLang/julia@59d153957596c1d798de08427fa97da370119163](https://github.com/JuliaLang/julia/commit/59d153957596c1d798de08427fa97da370119163)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16260#issuecomment-225436119)

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
| `["array","bool","bitarray_true_load!"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 0.99 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat",5)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 1.03 (15%)  | 1.13 (1%) :x: |
| `["array","cat",("vcat",5)]` | 0.85 (15%)  | 1.12 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.09 (15%)  | 1.13 (1%) :x: |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.75 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.91 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumelt","Array{Int32,2}")]` | 0.23 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.80 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.80 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.82 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.51 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.50 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.55 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.55 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.50 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.49 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["array","setindex!",("setindex!",1)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",2)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",3)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",4)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.50 (30%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["problem","go","go_game"]` | 1.09 (15%)  | 1.22 (1%) :x: |
| `["problem","imdb","centrality"]` | 1.03 (15%)  | 1.02 (1%) :x: |
| `["problem","raytrace"]` | 11.63 (15%) :x: | 7.48 (1%) :x: |
| `["problem","spellcheck"]` | 1.15 (15%) :x: | 1.22 (1%) :x: |
| `["shootout","nbody"]` | 1.20 (15%) :x: | 358.50 (1%) :x: |
| `["shootout","nbody_vec"]` | 1.08 (15%)  | 1.02 (1%) :x: |
| `["shootout","revcomp"]` | 0.99 (15%)  | 1.01 (1%) :x: |
| `["sparse","index",("spmat","array",10)]` | 1.02 (25%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.02 (15%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",10)]` | 1.13 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.04 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.98 (15%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.02 (15%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.02 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 1.04 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 1.01 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.00 (25%)  | 1.05 (1%) :x: |
| `["string","replace"]` | 1.63 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["io"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem"]`
- `["problem","seismic"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4721
Commit 15576a5 (2016-06-12 13:33 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27528.22265625 MB free)
Uptime: 1.389617e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     460445 s          0 s     223730 s  137963605 s          3 s
#2  3501 MHz    1350639 s          0 s     174165 s  137324907 s          1 s
#3  3501 MHz     470288 s          0 s     135518 s  138276340 s          1 s
#4  3501 MHz     319837 s          0 s     124495 s  138457558 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4681
Commit 59d1539 (2016-06-12 13:13 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27406.859375 MB free)
Uptime: 1.394219e6 sec
Load Avg:  1.005859375  1.0205078125  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     497105 s          0 s     230074 s  138379369 s          3 s
#2  3501 MHz    1530072 s          0 s     180000 s  137599138 s          1 s
#3  3501 MHz     609862 s          0 s     144636 s  138587117 s          1 s
#4  3501 MHz     395392 s          0 s     132154 s  138834011 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
