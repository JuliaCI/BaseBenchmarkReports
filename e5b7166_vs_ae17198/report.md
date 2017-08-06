# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e5b716626079620a836f7bff5ef482052b582b9d](https://github.com/JuliaLang/julia/commit/e5b716626079620a836f7bff5ef482052b582b9d) vs [JuliaLang/julia@ae1719872092b594228a9bfeedfc3fa8e91c9529](https://github.com/JuliaLang/julia/commit/ae1719872092b594228a9bfeedfc3fa8e91c9529)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23154)

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
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 0.80 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 0.79 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 0.79 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 0.76 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.51 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.51 (45%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1259
Commit e5b7166 (2017-08-06 13:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78224838 s          0 s   12089954 s  3668964314 s        131 s
       #2  3501 MHz  307549075 s          0 s   13075165 s  3440144924 s         46 s
       #3  3501 MHz   66343316 s          0 s    7623898 s  3691903572 s         62 s
       #4  3501 MHz   61682586 s          0 s    7549177 s  3696993677 s         21 s
       
  Memory: 31.383651733398438 GB (5558.01953125 MB free)
  Uptime: 3.7675229e7 sec
  Load Avg:  1.017578125  1.15478515625  1.48291015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1257
Commit ae17198 (2017-08-06 00:04 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78305195 s          0 s   12097526 s  3669079549 s        131 s
       #2  3501 MHz  307692549 s          0 s   13082738 s  3440197185 s         46 s
       #3  3501 MHz   66426444 s          0 s    7630782 s  3692016800 s         62 s
       #4  3501 MHz   61777977 s          0 s    7556786 s  3697094034 s         21 s
       
  Memory: 31.383651733398438 GB (5417.69140625 MB free)
  Uptime: 3.7677269e7 sec
  Load Avg:  1.0029296875  1.10205078125  1.58935546875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
