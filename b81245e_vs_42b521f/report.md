# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b81245e7679779626b5506771929213d9402c02c](https://github.com/JuliaLang/julia/commit/b81245e7679779626b5506771929213d9402c02c) vs [JuliaLang/julia@42b521fcf76bf241cbb6e7493d3a6631994dc2e6](https://github.com/JuliaLang/julia/commit/42b521fcf76bf241cbb6e7493d3a6631994dc2e6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23035#issuecomment-320119928)

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
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",1024)]` | 20.07 (45%) :x: | 12.44 (1%) :x: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 15.24 (45%) :x: | 10.89 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1232
Commit b81245e (2017-08-03 23:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77722490 s          0 s   12030918 s  3647282271 s        129 s
       #2  3501 MHz  305842636 s          0 s   12973111 s  3419719680 s         45 s
       #3  3501 MHz   65825102 s          0 s    7573596 s  3670196157 s         61 s
       #4  3501 MHz   61200924 s          0 s    7500116 s  3675244412 s         21 s
       
  Memory: 31.383651733398438 GB (4361.2890625 MB free)
  Uptime: 3.7452372e7 sec
  Load Avg:  1.0029296875  1.12451171875  1.45361328125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1230
Commit 42b521f (2017-08-03 23:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77798276 s          0 s   12038576 s  3647394538 s        129 s
       #2  3501 MHz  305997523 s          0 s   12980970 s  3419752967 s         45 s
       #3  3501 MHz   65907278 s          0 s    7580557 s  3670302988 s         61 s
       #4  3501 MHz   61282701 s          0 s    7507328 s  3675351485 s         21 s
       
  Memory: 31.383651733398438 GB (4297.21875 MB free)
  Uptime: 3.7454339e7 sec
  Load Avg:  0.9970703125  1.12841796875  1.62939453125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
