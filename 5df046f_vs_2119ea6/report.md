# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5df046f14e025971be997c9918e586dcaadb18b2](https://github.com/JuliaLang/julia/commit/5df046f14e025971be997c9918e586dcaadb18b2) vs [JuliaLang/julia@2119ea6ff7c2e25ac5f587fad67241c6ecc1a8eb](https://github.com/JuliaLang/julia/commit/2119ea6ff7c2e25ac5f587fad67241c6ecc1a8eb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16260#issuecomment-225730304)

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
| `["array","bool","bitarray_true_load!"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",5)]` | 1.01 (15%)  | 1.01 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.03 (15%)  | 1.13 (1%) :x: |
| `["array","cat",("vcat",5)]` | 1.03 (15%)  | 1.12 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.10 (15%)  | 1.13 (1%) :x: |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("prerend!",8)]` | 0.59 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.76 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.04 (40%)  | 0.97 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.57 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.56 (40%) :white_check_mark: | 0.59 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.50 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.50 (40%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["array","setindex!",("setindex!",3)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",4)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.67 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.58 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.67 (30%) :white_check_mark: | 0.99 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.65 (30%) :white_check_mark: | 0.99 (1%)  |
| `["problem","go","go_game"]` | 1.12 (15%)  | 1.22 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Float32}")]` | 1.92 (50%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.04 (25%)  | 0.99 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","array",10)]` | 1.05 (15%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",10)]` | 1.13 (15%)  | 1.11 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.05 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.01 (15%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.08 (15%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.03 (15%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","splogical",10)]` | 1.13 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",100)]` | 1.03 (25%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","splogical",1000)]` | 1.01 (25%)  | 1.05 (1%) :x: |
| `["string","replace"]` | 1.47 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.0-dev+4752
Commit 5df046f (2016-06-13 22:20 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27979.5859375 MB free)
Uptime: 1.50759e6 sec
Load Avg:  0.9697265625  1.01171875  0.9619140625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1188129 s          0 s     366425 s  148820236 s          4 s
#2  3501 MHz    3848076 s          0 s     237773 s  146582322 s          0 s
#3  3501 MHz    1830724 s          0 s     250608 s  148593434 s          0 s
#4  3501 MHz    1547297 s          0 s     225860 s  148909429 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4707
Commit 2119ea6 (2016-06-13 18:26 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27680.30859375 MB free)
Uptime: 1.512198e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1301329 s          0 s     375693 s  149157337 s          4 s
#2  3501 MHz    4070006 s          0 s     245854 s  146812682 s          0 s
#3  3501 MHz    1880327 s          0 s     256512 s  148997969 s          1 s
#4  3501 MHz    1594415 s          0 s     231818 s  149316565 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
