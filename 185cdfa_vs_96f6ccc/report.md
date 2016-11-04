# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@185cdfac1db6a424450ce3f8198b0ec969479db6](https://github.com/pabloferz/julia/commit/185cdfac1db6a424450ce3f8198b0ec969479db6) vs [JuliaLang/julia@96f6cccbc35f0a8aa2e7c9fe6103bcba1c254bbd](https://github.com/JuliaLang/julia/commit/96f6cccbc35f0a8aa2e7c9fe6103bcba1c254bbd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18642#issuecomment-258522167)

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
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.35 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.81 (15%) :white_check_mark: | 1.13 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 1.15 (45%)  | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.51 (45%) :x: | 1.27 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 3.47 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 8.00 (45%) :x: | 1.27 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 3.59 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 8.77 (45%) :x: | 1.27 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.32 (45%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.33 (45%)  | 1.02 (1%) :x: |
| `["micro","randmatstat"]` | 4.62 (15%) :x: | 1.22 (1%) :x: |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 1.27 (15%) :x: | 1.01 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.25 (15%) :x: | 1.01 (1%)  |
| `["shootout","nbody_vec"]` | 63.04 (15%) :x: | 3.64 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 60.37 (30%) :x: | 3.47 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 57.58 (30%) :x: | 2.95 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 34.09 (30%) :x: | 1.65 (1%) :x: |

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
Julia Version 0.6.0-dev.1190
Commit 185cdfa (2016-11-04 18:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12146.97265625 MB free)
Uptime: 1.3937909e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22226257 s          0 s    3724174 s  1364950256 s         45 s
#2  3501 MHz   59760854 s          0 s    4244155 s  1327730421 s         14 s
#3  3501 MHz   19265275 s          0 s    2473897 s  1371384964 s         22 s
#4  3501 MHz   16108370 s          0 s    2403640 s  1374732593 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1186
Commit 96f6ccc (2016-11-04 14:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11847.10546875 MB free)
Uptime: 1.3943696e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22352561 s          0 s    3734868 s  1365390268 s         45 s
#2  3501 MHz   60078596 s          0 s    4251596 s  1327983040 s         14 s
#3  3501 MHz   19307808 s          0 s    2480300 s  1371913929 s         22 s
#4  3501 MHz   16169023 s          0 s    2410795 s  1375242904 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
