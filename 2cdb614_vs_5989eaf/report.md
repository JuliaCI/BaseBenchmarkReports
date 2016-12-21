# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@2cdb614a7a32f0007c26003953742ce70600f12d](https://github.com/stevengj/julia/commit/2cdb614a7a32f0007c26003953742ce70600f12d) vs [JuliaLang/julia@5989eaf04242f567ff31d8172d4755af22b39176](https://github.com/JuliaLang/julia/commit/5989eaf04242f567ff31d8172d4755af22b39176)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19672#issuecomment-268586237)

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

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1647
Commit 2cdb614 (2016-12-21 17:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10842.25390625 MB free)
Uptime: 1.7993881e7 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   23899011 s          0 s    5728290 s  1764610527 s         56 s
#2  3501 MHz   74330071 s          0 s    3471113 s  1720514182 s          8 s
#3  3501 MHz   23252498 s          0 s    3004826 s  1772304761 s         35 s
#4  3501 MHz   20335294 s          0 s    3054468 s  1775155498 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1644
Commit 5989eaf (2016-12-21 15:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (10687.3359375 MB free)
Uptime: 1.7997557e7 sec
Load Avg:  0.9169921875  0.95458984375  0.9326171875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   23944424 s          0 s    5734482 s  1764925435 s         56 s
#2  3501 MHz   74438781 s          0 s    3478519 s  1720765209 s          8 s
#3  3501 MHz   23292001 s          0 s    3011364 s  1772625534 s         35 s
#4  3501 MHz   20478565 s          0 s    3064961 s  1775368804 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
