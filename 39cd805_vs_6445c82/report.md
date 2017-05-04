# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@39cd805589d02016191b4b3b7c8407d01aaf624a](https://github.com/JuliaLang/julia/commit/39cd805589d02016191b4b3b7c8407d01aaf624a) vs [JuliaLang/julia@6445c82d0060dbe82b88436f0f4371a4ee64d918](https://github.com/JuliaLang/julia/commit/6445c82d0060dbe82b88436f0f4371a4ee64d918)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/39cd805589d02016191b4b3b7c8407d01aaf624a#commitcomment-22016958)

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
| `["array","growth",("push_multiple!",2048)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["array","index","6d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","7d"]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 2.16 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.73 (20%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.5.2-pre+14
Commit 39cd805 (2017-05-02 18:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9309.09375 MB free)
Uptime: 2.9555992e7 sec
Load Avg:  1.0830078125  1.03125  1.11279296875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60682209 s          0 s   11506523 s  2874806098 s         77 s
#2  3501 MHz  245430423 s          0 s    7200861 s  2701234025 s         12 s
#3  3501 MHz   54180025 s          0 s    6394698 s  2893599221 s         62 s
#4  3501 MHz   51307556 s          0 s    6547938 s  2896318460 s         13 s

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
Memory: 31.383651733398438 GB (9193.0859375 MB free)
Uptime: 2.9559596e7 sec
Load Avg:  1.0029296875  1.0146484375  1.10400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60761902 s          0 s   11515901 s  2875075989 s         77 s
#2  3501 MHz  245742296 s          0 s    7209344 s  2701273580 s         12 s
#3  3501 MHz   54259668 s          0 s    6402751 s  2893871378 s         62 s
#4  3501 MHz   51384166 s          0 s    6555762 s  2896593937 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
