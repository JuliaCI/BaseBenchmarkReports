# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@9e1151c9e13eef09ff3f50c6ec11c551992b4441](https://github.com/mbauman/julia/commit/9e1151c9e13eef09ff3f50c6ec11c551992b4441) vs [JuliaLang/julia@934ad48a453945a0b5e0535328039649f30215e7](https://github.com/JuliaLang/julia/commit/934ad48a453945a0b5e0535328039649f30215e7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15558#issuecomment-265461067)

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
| `["array","cat",("vcat",5)]` | 1.03 (15%)  | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 1.31 (50%)  | 1.61 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 1.29 (50%)  | 1.52 (1%) :x: |
| `["broadcast","sparse",((1000,1000),1)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("cumsum!",Float32,1024)]` | 1.40 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Float32,256)]` | 1.33 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Float64,1024)]` | 1.34 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Float64,256)]` | 1.35 (45%)  | Inf (1%) :x: |

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
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1410
Commit 9e1151c (2016-12-07 09:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14937.3046875 MB free)
Uptime: 1.6770993e7 sec
Load Avg:  1.0029296875  1.001953125  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22169042 s          0 s    5338232 s  1644782149 s         50 s
#2  3501 MHz   67404742 s          0 s    3205838 s  1605485213 s          7 s
#3  3501 MHz   21854413 s          0 s    2792025 s  1651685576 s         33 s
#4  3501 MHz   18859063 s          0 s    2827687 s  1654630459 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1408
Commit 934ad48 (2016-12-07 01:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14823.7109375 MB free)
Uptime: 1.6775333e7 sec
Load Avg:  1.0029296875  0.99462890625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22222204 s          0 s    5345294 s  1645154545 s         50 s
#2  3501 MHz   67580859 s          0 s    3213354 s  1605735091 s          7 s
#3  3501 MHz   21971334 s          0 s    2801236 s  1651992693 s         33 s
#4  3501 MHz   18915564 s          0 s    2835448 s  1654999565 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
