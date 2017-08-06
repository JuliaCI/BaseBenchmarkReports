# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7c82754d768e28dd49b646562503b70cd4e8a9ca](https://github.com/JuliaLang/julia/commit/7c82754d768e28dd49b646562503b70cd4e8a9ca) vs [JuliaLang/julia@ae1719872092b594228a9bfeedfc3fa8e91c9529](https://github.com/JuliaLang/julia/commit/ae1719872092b594228a9bfeedfc3fa8e91c9529)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23154#issuecomment-320508169)

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
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 0.78 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 0.74 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 0.78 (45%)  | 0.75 (1%) :white_check_mark: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 0.72 (45%)  | 0.75 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1259
Commit 7c82754 (2017-08-06 13:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83030410 s          0 s   14978198 s  3658543326 s         86 s
       #2  3501 MHz  341323884 s          0 s    9419180 s  3414616497 s         13 s
       #3  3501 MHz   72184167 s          0 s    8327804 s  3685236854 s         73 s
       #4  3501 MHz   68896184 s          0 s    8518050 s  3688319361 s         17 s
       
  Memory: 31.383651733398438 GB (5521.82421875 MB free)
  Uptime: 3.7675558e7 sec
  Load Avg:  0.9970703125  1.123046875  1.447265625
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
       #1  3501 MHz   83121325 s          0 s   14985824 s  3658638627 s         86 s
       #2  3501 MHz  341465228 s          0 s    9426226 s  3414662300 s         13 s
       #3  3501 MHz   72265552 s          0 s    8334772 s  3685342573 s         73 s
       #4  3501 MHz   68970637 s          0 s    8525332 s  3688431746 s         17 s
       
  Memory: 31.383651733398438 GB (5408.21484375 MB free)
  Uptime: 3.7677504e7 sec
  Load Avg:  0.9228515625  1.10888671875  1.625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
