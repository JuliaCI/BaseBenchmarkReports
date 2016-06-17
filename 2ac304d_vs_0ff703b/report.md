# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@2ac304dfba75fad148d4070ef4f8a2e400c305bb](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb) vs [JuliaLang/julia@0ff703b40afddf9b705bd6a06d3a59cb4c089ea5](https://github.com/JuliaLang/julia/commit/0ff703b40afddf9b705bd6a06d3a59cb4c089ea5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb#commitcomment-17907704)

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
| `["array","bool","bitarray_bool_load!"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","bool","bitarray_true_load!"]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 5.75 (15%) :x: | 1.03 (1%) :x: |
| `["array","cat",("vcat",5)]` | 3.95 (15%) :x: | 1.14 (1%) :x: |
| `["array","growth",("push_multiple!",2048)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",1024)]` | 0.81 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 0.65 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",1024)]` | 0.09 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",256)]` | 0.17 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",1024)]` | 0.84 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 0.66 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",1024)]` | 0.09 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",256)]` | 0.16 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",1024)]` | 0.74 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 0.73 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",1024)]` | 0.76 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.76 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",1024)]` | 0.71 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 0.66 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","Vector",1024)]` | 0.25 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","Vector",256)]` | 0.45 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",1024)]` | 0.71 (30%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 0.67 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","Vector",1024)]` | 0.28 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","Vector",256)]` | 0.44 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","blas","dot"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["linalg","blas","dotc"]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dotu"]` | 0.47 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gbmv!"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","gbmv"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","sbmv!"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","sbmv"]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","symv!"]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","symv"]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","trmm!"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","trsm!"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.85 (15%)  | 0.96 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.85 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.84 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.83 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.82 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["problem","spellcheck"]` | 0.74 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |

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
Julia Version 0.4.5
Commit 2ac304d (2016-03-18 00:58 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27492.734375 MB free)
Uptime: 1.790424e6 sec
Load Avg:  1.0185546875  1.02294921875  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1127143 s          0 s     347321 s  177160519 s          4 s
#2  3501 MHz    3011286 s          0 s     282380 s  175600242 s          1 s
#3  3501 MHz    1346382 s          0 s     235076 s  177354140 s          1 s
#4  3501 MHz     859668 s          0 s     204924 s  177899270 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

#### Comparison Build

```
Julia Version 0.4.0
Commit 0ff703b (2015-10-08 06:20 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27357.50390625 MB free)
Uptime: 1.793703e6 sec
Load Avg:  1.0029296875  1.0146484375  1.04736328125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1207254 s          0 s     355200 s  177399213 s          5 s
#2  3501 MHz    3200850 s          0 s     288950 s  175731267 s          1 s
#3  3501 MHz    1402481 s          0 s     240629 s  177619564 s          1 s
#4  3501 MHz     901713 s          0 s     210393 s  178178963 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
