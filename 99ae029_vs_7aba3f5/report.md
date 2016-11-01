# Benchmark Report

## Job Properties

*Commit(s):* [jw3126/julia@99ae02919015770eb55ca6cbbd5f15623177b563](https://github.com/jw3126/julia/commit/99ae02919015770eb55ca6cbbd5f15623177b563) vs [JuliaLang/julia@7aba3f57bcd370c7bda2a3df4ba6cecf3553df33](https://github.com/JuliaLang/julia/commit/7aba3f57bcd370c7bda2a3df4ba6cecf3553df33)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18931#issuecomment-257678282)

*Tag Predicate:* `"linalg"`

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
| `["linalg","arithmetic",("cumsum!",Float32,1024)]` | 1.03 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Float32,256)]` | 1.10 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Float64,1024)]` | 1.02 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Float64,256)]` | 1.09 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Int32,1024)]` | 0.66 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Int32,256)]` | 0.90 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Int64,1024)]` | 0.63 (45%)  | Inf (1%) :x: |
| `["linalg","arithmetic",("cumsum!",Int64,256)]` | 0.86 (45%)  | Inf (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1181
Commit 99ae029 (2016-11-01 17:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11934.5078125 MB free)
Uptime: 1.367961e7 sec
Load Avg:  1.0029296875  0.9853515625  0.92626953125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20944374 s          0 s    4623662 s  1338474679 s         42 s
#2  3501 MHz   60429366 s          0 s    2862557 s  1303819221 s          6 s
#3  3501 MHz   20288500 s          0 s    2521119 s  1344502248 s         29 s
#4  3501 MHz   17559646 s          0 s    2526207 s  1347218187 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1172
Commit 7aba3f5 (2016-11-01 17:23 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (11916.93359375 MB free)
Uptime: 1.3683268e7 sec
Load Avg:  1.0029296875  0.9853515625  0.94140625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20985062 s          0 s    4630045 s  1338792402 s         42 s
#2  3501 MHz   60531247 s          0 s    2869036 s  1304076314 s          6 s
#3  3501 MHz   20325854 s          0 s    2527294 s  1344823796 s         29 s
#4  3501 MHz   17715136 s          0 s    2537726 s  1347416536 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
