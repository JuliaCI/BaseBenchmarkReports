# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@27b5db9734abd3878333ffa118e8df55e642f115](https://github.com/stevengj/julia/commit/27b5db9734abd3878333ffa118e8df55e642f115) vs [JuliaLang/julia@101dcccc0bd0334ec95cba0c792f783e5ccd54f2](https://github.com/JuliaLang/julia/commit/101dcccc0bd0334ec95cba0c792f783e5ccd54f2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21598#issuecomment-298179463)

*Tag Predicate:* `"linalg" || "problem"`

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
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.11 (45%)  | 1.01 (1%) :x: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.11 (45%)  | 1.01 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
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

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.424
Commit 27b5db9 (2017-04-29 15:26 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2813.4765625 MB free)
Uptime: 2.9131731e7 sec
Load Avg:  1.0029296875  1.12060546875  1.486328125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   59839610 s          0 s    9254937 s  2837841042 s         85 s
#2  3501 MHz  226661320 s          0 s   10173718 s  2670947493 s         33 s
#3  3501 MHz   50679904 s          0 s    5911557 s  2855274382 s         45 s
#4  3501 MHz   46208804 s          0 s    5851011 s  2860080760 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.420
Commit 101dccc (2017-04-29 15:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2797.16015625 MB free)
Uptime: 2.9133805e7 sec
Load Avg:  1.0029296875  1.1162109375  1.61962890625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   59920528 s          0 s    9263554 s  2837958050 s         85 s
#2  3501 MHz  226816108 s          0 s   10182146 s  2670991089 s         33 s
#3  3501 MHz   50764590 s          0 s    5920105 s  2855387869 s         45 s
#4  3501 MHz   46302961 s          0 s    5859415 s  2860185088 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
