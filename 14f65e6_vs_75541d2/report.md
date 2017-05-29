# Benchmark Report

## Job Properties

*Commit(s):* [jebej/julia@14f65e6c2333b342dbbf1b8c028c70f8579378c8](https://github.com/jebej/julia/commit/14f65e6c2333b342dbbf1b8c028c70f8579378c8) vs [JuliaLang/julia@75541d2008dd95d5e7a6e3201f0995b56588dc99](https://github.com/JuliaLang/julia/commit/75541d2008dd95d5e7a6e3201f0995b56588dc99)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22111#issuecomment-304722425)

*Tag Predicate:* `"sparse"`

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

- `["broadcast","sparse"]`
- `["problem","fem"]`
- `["problem","laplacian"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.389
Commit 14f65e6 (2017-05-29 17:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4002.85546875 MB free)
Uptime: 3.1735333e7 sec
Load Avg:  0.9169921875  1.5107421875  1.77197265625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   66510771 s          0 s   12458307 s  3085316891 s         81 s
#2  3501 MHz  275294183 s          0 s    7859369 s  2888514421 s         12 s
#3  3501 MHz   59684361 s          0 s    6997376 s  3105314857 s         65 s
#4  3501 MHz   56715121 s          0 s    7153476 s  3108125824 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.386
Commit 75541d2 (2017-05-29 17:18 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3950.68359375 MB free)
Uptime: 3.1736934e7 sec
Load Avg:  1.0029296875  1.56396484375  2.1005859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   66596457 s          0 s   12466376 s  3085382517 s         81 s
#2  3501 MHz  275408219 s          0 s    7867614 s  2888551785 s         12 s
#3  3501 MHz   59770642 s          0 s    7005554 s  3105379912 s         65 s
#4  3501 MHz   56796490 s          0 s    7161678 s  3108195711 s         14 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
