# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8619307ca94e5a30f5be0a3aaeabf6f64f5a6e7a](https://github.com/JuliaLang/julia/commit/8619307ca94e5a30f5be0a3aaeabf6f64f5a6e7a) vs [JuliaLang/julia@6445c82d0060dbe82b88436f0f4371a4ee64d918](https://github.com/JuliaLang/julia/commit/6445c82d0060dbe82b88436f0f4371a4ee64d918)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/8619307ca94e5a30f5be0a3aaeabf6f64f5a6e7a#commitcomment-22015180)

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
| `["array","cat",("hcat",5)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 0.46 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.55 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 0.52 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.84 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.61 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.50 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 1.55 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.46 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.48 (45%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 2.03 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 2.07 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.20 (20%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.45 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.2-pre+11
Commit 8619307 (2017-05-02 18:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8418.2109375 MB free)
Uptime: 2.9547726e7 sec
Load Avg:  1.0029296875  1.0146484375  1.13623046875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60515791 s          0 s   11488432 s  2874167311 s         77 s
#2  3501 MHz  244753830 s          0 s    7176422 s  2701109518 s         12 s
#3  3501 MHz   54012219 s          0 s    6378036 s  2892958365 s         62 s
#4  3501 MHz   51158846 s          0 s    6532513 s  2895657111 s         13 s

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
Memory: 31.383651733398438 GB (8987.40625 MB free)
Uptime: 2.9552015e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60603128 s          0 s   11497637 s  2874498000 s         77 s
#2  3501 MHz  245122670 s          0 s    7191988 s  2701153574 s         12 s
#3  3501 MHz   54091162 s          0 s    6386246 s  2893299506 s         62 s
#4  3501 MHz   51233886 s          0 s    6540151 s  2896002821 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
