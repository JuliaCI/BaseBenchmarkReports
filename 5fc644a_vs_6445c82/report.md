# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5fc644a714055c45f289bd4f1b3159a6b485c230](https://github.com/JuliaLang/julia/commit/5fc644a714055c45f289bd4f1b3159a6b485c230) vs [JuliaLang/julia@6445c82d0060dbe82b88436f0f4371a4ee64d918](https://github.com/JuliaLang/julia/commit/6445c82d0060dbe82b88436f0f4371a4ee64d918)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/5fc644a714055c45f289bd4f1b3159a6b485c230#commitcomment-22016969)

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
| `["array","cat",("hcat",5)]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 0.48 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.83 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.93 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.70 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 2.16 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 2.20 (15%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.65 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.47 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |

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
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["problem","laplacian"]`
- `["simd"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.2-pre+13
Commit 5fc644a (2017-05-02 18:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9059.265625 MB free)
Uptime: 2.9555881e7 sec
Load Avg:  0.94775390625  1.00830078125  1.13671875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61066086 s          0 s    9419865 s  2878782431 s         86 s
#2  3501 MHz  231832781 s          0 s   10401243 s  2707872941 s         35 s
#3  3501 MHz   51954232 s          0 s    6049230 s  2896258707 s         45 s
#4  3501 MHz   47486821 s          0 s    5989762 s  2901063536 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.1
Commit 6445c82 (2017-03-05 13:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9023.7109375 MB free)
Uptime: 2.9560204e7 sec
Load Avg:  1.0029296875  1.0146484375  1.0458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61155560 s          0 s    9429312 s  2879114127 s         86 s
#2  3501 MHz  232201264 s          0 s   10417135 s  2707920303 s         35 s
#3  3501 MHz   52034631 s          0 s    6057210 s  2896601960 s         45 s
#4  3501 MHz   47565482 s          0 s    5998390 s  2901407992 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
