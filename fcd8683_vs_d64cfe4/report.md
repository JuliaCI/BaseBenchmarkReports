# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@fcd86837262c2b1111fb8207d16a0aab0f28baad](https://github.com/pabloferz/julia/commit/fcd86837262c2b1111fb8207d16a0aab0f28baad) vs [JuliaLang/julia@d64cfe4d30fb9b179d148a4efa6882480f2047ce](https://github.com/JuliaLang/julia/commit/d64cfe4d30fb9b179d148a4efa6882480f2047ce)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17929#issuecomment-238714003)

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
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 0.91 (30%)  | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 0.62 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 0.10 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 0.34 (30%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 0.17 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 0.26 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 0.28 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 0.13 (30%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 0.26 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 0.34 (30%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 0.16 (30%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 0.24 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 0.28 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 0.13 (30%) :white_check_mark: | 0.85 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 0.25 (30%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 0.11 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.74 (25%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.74 (25%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["micro","randmatstat"]` | 0.19 (15%) :white_check_mark: | 0.84 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.63 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.63 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["shootout","nbody_vec"]` | 0.01 (15%) :white_check_mark: | 0.19 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",10)]` | 0.01 (15%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.02 (15%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.03 (15%) :white_check_mark: | 0.63 (1%) :white_check_mark: |

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
Julia Version 0.6.0-dev.119
Commit fcd8683 (2016-08-09 22:27 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21848.23828125 MB free)
Uptime: 6.432315e6 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    8961550 s          0 s    1772538 s  630995038 s         21 s
#2  3501 MHz   18981840 s          0 s    1324918 s  622284691 s          5 s
#3  3501 MHz    6672118 s          0 s     948639 s  635281972 s         10 s
#4  3501 MHz    4865220 s          0 s     918524 s  637162914 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.117
Commit d64cfe4 (2016-08-09 22:08 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21434.83203125 MB free)
Uptime: 6.437036e6 sec
Load Avg:  0.9228515625  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9090586 s          0 s    1783662 s  631325774 s         21 s
#2  3501 MHz   19190613 s          0 s    1332594 s  622539564 s          5 s
#3  3501 MHz    6731045 s          0 s     954903 s  635688008 s         10 s
#4  3501 MHz    4909095 s          0 s     924871 s  637584121 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
