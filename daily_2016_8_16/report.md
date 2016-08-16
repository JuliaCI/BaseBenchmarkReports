# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f73e6e126b1d48a0968694ee2f972270dbf2292a](https://github.com/JuliaLang/julia/commit/f73e6e126b1d48a0968694ee2f972270dbf2292a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/f73e6e126b1d48a0968694ee2f972270dbf2292a#commitcomment-18650650)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-08-16 vs 2016-08-15

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
| `["array","cat",("catnd",5)]` | 0.90 (15%)  | 0.94 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 1.03 (15%)  | 0.99 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 0.88 (15%)  | 0.89 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.97 (15%)  | 0.90 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.80 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumeach","100000000:-1:1")]` | 2.14 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","1:100000000")]` | 6.75 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","1:100000000")]` | 9.33 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","100000000:-1:1")]` | 2.14 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear","1:100000000")]` | 7.00 (40%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 0.57 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.56 (15%) :white_check_mark: | 0.99 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 1.12 (30%)  | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.52 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 3.87 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 9.13 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 4.14 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 9.87 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 2.97 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 5.99 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 4.11 (30%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 9.40 (30%) :x: | 1.25 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 3.94 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 9.28 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.50 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 7.84 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 3.99 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 9.24 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 2.89 (30%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 5.93 (30%) :x: | 1.12 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 3.98 (30%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 9.30 (30%) :x: | 1.25 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 3.86 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 9.20 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.47 (30%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 7.78 (30%) :x: | 1.18 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 3.90 (30%) :x: | 1.06 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 9.07 (30%) :x: | 1.24 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.31 (25%) :x: | 1.02 (1%) :x: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.31 (25%) :x: | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 5.13 (15%) :x: | 1.19 (1%) :x: |
| `["problem","go","go_game"]` | 0.86 (15%)  | 0.82 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 1.33 (15%) :x: | 1.02 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.27 (15%) :x: | 1.01 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 116.66 (15%) :x: | 5.40 (1%) :x: |
| `["simd",("sum_reduce","Float32",4095)]` | 1.27 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 1.23 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",10)]` | 62.65 (15%) :x: | 3.20 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 60.23 (15%) :x: | 2.74 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 32.70 (15%) :x: | 1.58 (1%) :x: |

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
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
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
Julia Version 0.6.0-dev.231
Commit f73e6e1 (2016-08-15 23:34 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (18277.5234375 MB free)
Uptime: 6.969867e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   10956948 s          0 s    2320913 s  681710599 s         22 s
#2  3501 MHz   27693008 s          0 s    1380741 s  667426883 s          3 s
#3  3501 MHz    9667628 s          0 s    1224571 s  685762184 s         12 s
#4  3501 MHz    8226358 s          0 s    1217450 s  687201568 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
