# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@03db8fcf597e59472337cddf87f2f4a5c2e623a5](https://github.com/JuliaLang/julia/commit/03db8fcf597e59472337cddf87f2f4a5c2e623a5) vs [JuliaLang/julia@2ac304dfba75fad148d4070ef4f8a2e400c305bb](https://github.com/JuliaLang/julia/commit/2ac304dfba75fad148d4070ef4f8a2e400c305bb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/03db8fcf597e59472337cddf87f2f4a5c2e623a5#commitcomment-17923251)

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
| `["io","read"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dotc"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dotu"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort forwards","ones")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort reverse","ones")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ones")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 1.46 (40%) :x: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 1.62 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.4.6-pre+83
Commit 03db8fc (2016-06-18 12:55 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27138.0703125 MB free)
Uptime: 1.903718e6 sec
Load Avg:  0.9228515625  0.998046875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1874726 s          0 s     443848 s  187615087 s          6 s
#2  3501 MHz    5592636 s          0 s     380044 s  184235759 s          1 s
#3  3501 MHz    2283287 s          0 s     326614 s  187641866 s          2 s
#4  3501 MHz    1496555 s          0 s     288593 s  188496918 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

#### Comparison Build

```
Julia Version 0.4.5
Commit 2ac304d (2016-03-18 00:58 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27009.40625 MB free)
Uptime: 1.906963e6 sec
Load Avg:  1.02001953125  1.03173828125  1.05615234375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1971016 s          0 s     451948 s  187833977 s          6 s
#2  3501 MHz    5778331 s          0 s     386438 s  184367385 s          1 s
#3  3501 MHz    2322812 s          0 s     332329 s  187920194 s          2 s
#4  3501 MHz    1543702 s          0 s     294542 s  188767687 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
