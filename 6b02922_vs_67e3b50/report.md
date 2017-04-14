# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6b02922d9c3b14904632d942022bdad1306821ac](https://github.com/JuliaLang/julia/commit/6b02922d9c3b14904632d942022bdad1306821ac) vs [JuliaLang/julia@67e3b50bc4ffd35ff30e73224554d0c8338c3e98](https://github.com/JuliaLang/julia/commit/67e3b50bc4ffd35ff30e73224554d0c8338c3e98)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21377#issuecomment-294203851)

*Tag Predicate:* `"array" || "io"`

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
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["misc","repeat",(200,1,24)]` | 0.37 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","repeat",(200,24,1)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 0.05 (15%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.06 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.07 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.07 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.06 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.04 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.04 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.04 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.04 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.16 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.16 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.17 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.17 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 0.02 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 0.04 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 0.09 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 0.03 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 0.08 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 0.49 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",1000)]` | 0.49 (30%) :white_check_mark: | 1.00 (1%)  |

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
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["parallel","remotecall"]`
- `["problem","laplacian"]`
- `["simd"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.137
Commit 6b02922 (2017-04-14 16:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4520.30078125 MB free)
Uptime: 2.784223e7 sec
Load Avg:  1.0029296875  1.0146484375  1.11669921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   56936684 s          0 s    8820444 s  2712491075 s         82 s
#2  3501 MHz  212219276 s          0 s    9671951 s  2557180874 s         30 s
#3  3501 MHz   47690817 s          0 s    5575144 s  2729709208 s         44 s
#4  3501 MHz   43268341 s          0 s    5522155 s  2734442101 s         15 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.134
Commit 67e3b50 (2017-04-14 16:54 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4570.29296875 MB free)
Uptime: 2.7845656e7 sec
Load Avg:  1.0029296875  1.0146484375  1.1357421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   57016839 s          0 s    8829514 s  2712743135 s         82 s
#2  3501 MHz  212521842 s          0 s    9680240 s  2557212068 s         30 s
#3  3501 MHz   47777085 s          0 s    5583903 s  2729956110 s         44 s
#4  3501 MHz   43347674 s          0 s    5530702 s  2734696278 s         15 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
