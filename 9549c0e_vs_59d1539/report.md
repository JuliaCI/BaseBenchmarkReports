# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9549c0eba432c703ca51b173f3c31958a4e671d4](https://github.com/JuliaLang/julia/commit/9549c0eba432c703ca51b173f3c31958a4e671d4) vs [JuliaLang/julia@59d153957596c1d798de08427fa97da370119163](https://github.com/JuliaLang/julia/commit/59d153957596c1d798de08427fa97da370119163)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16895)

*Tag Predicate:* `"array"`

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
| `["array","index",("sumcartesian","Array{Float32,2}")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","Array{Int32,2}")]` | 0.20 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.16 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.24 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.16 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.17 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 0.17 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.62 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["problem","laplacian"]`
- `["simd"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4684
Commit 9549c0e (2016-06-12 17:49 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (27640.5390625 MB free)
Uptime: 1.402816e6 sec
Load Avg:  1.0029296875  1.0  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     539112 s          0 s     236646 s  139188482 s          3 s
#2  3501 MHz    1720988 s          0 s     190758 s  138255925 s          1 s
#3  3501 MHz     686866 s          0 s     151668 s  139361844 s          1 s
#4  3501 MHz     436440 s          0 s     138319 s  139645790 s          1 s

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
Memory: 31.383651733398438 GB (27584.5390625 MB free)
Uptime: 1.406622e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     678563 s          0 s     246685 s  139418779 s          3 s
#2  3501 MHz    1852775 s          0 s     198355 s  138496672 s          1 s
#3  3501 MHz     718759 s          0 s     157061 s  139704384 s          1 s
#4  3501 MHz     485066 s          0 s     144127 s  139971443 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
