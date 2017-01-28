# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@3bec97ad02e3096e54e396a43fb8545d7e1a9c6c](https://github.com/stevengj/julia/commit/3bec97ad02e3096e54e396a43fb8545d7e1a9c6c) vs [JuliaLang/julia@78448fa8cbba354ea7786bfb5ff19f8e17630430](https://github.com/JuliaLang/julia/commit/78448fa8cbba354ea7786bfb5ff19f8e17630430)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16305#issuecomment-275830470)

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
| `["array","cat",("hcat",5)]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.78 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",2048)]` | 1.19 (15%) :x: | 0.99 (1%) :white_check_mark: |
| `["array","growth",("append!",256)]` | 1.78 (15%) :x: | 1.71 (1%) :x: |
| `["array","growth",("append!",8)]` | 1.43 (15%) :x: | 2.12 (1%) :x: |
| `["array","growth",("prerend!",2048)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",2048)]` | 1.26 (15%) :x: | 2.03 (1%) :x: |
| `["array","growth",("push_multiple!",256)]` | 1.11 (15%)  | 1.04 (1%) :x: |
| `["array","growth",("push_multiple!",8)]` | 1.31 (15%) :x: | 2.14 (1%) :x: |
| `["array","growth",("push_single!",2048)]` | 0.97 (15%)  | 0.92 (1%) :white_check_mark: |
| `["array","growth",("push_single!",256)]` | 0.97 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.56 (15%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.21 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","array",100)]` | 1.03 (30%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.09 (30%)  | 1.69 (1%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.05 (30%)  | 1.08 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.01 (30%)  | 1.29 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.06 (30%)  | 1.14 (1%) :x: |

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
Julia Version 0.6.0-dev.2433
Commit 3bec97a (2017-01-28 06:18 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20049.79296875 MB free)
Uptime: 2.1235372e7 sec
Load Avg:  1.05419921875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33527554 s          0 s    7277320 s  2076658291 s         64 s
#2  3501 MHz  115433047 s          0 s    4500476 s  2002344040 s          8 s
#3  3501 MHz   31226337 s          0 s    3913102 s  2087391388 s         46 s
#4  3501 MHz   29194776 s          0 s    4053504 s  2089272876 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2430
Commit 78448fa (2017-01-28 02:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19887.06640625 MB free)
Uptime: 2.1240979e7 sec
Load Avg:  0.9228515625  0.998046875  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   33589516 s          0 s    7286618 s  2077146031 s         64 s
#2  3501 MHz  115745803 s          0 s    4509557 s  2002582429 s          8 s
#3  3501 MHz   31344355 s          0 s    3921703 s  2087824624 s         46 s
#4  3501 MHz   29230588 s          0 s    4059508 s  2089791124 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
