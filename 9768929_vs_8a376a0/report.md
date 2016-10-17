# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@97689293ce7d5b5e803d041202b33767bef99a74](https://github.com/JuliaLang/julia/commit/97689293ce7d5b5e803d041202b33767bef99a74) vs [JuliaLang/julia@8a376a00729bb7a30a2f921c9c1f78e04810eb56](https://github.com/JuliaLang/julia/commit/8a376a00729bb7a30a2f921c9c1f78e04810eb56)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18929#issuecomment-254111796)

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
Julia Version 0.6.0-dev.995
Commit 9768929 (2016-10-17 00:47 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13038.8828125 MB free)
Uptime: 1.2328756e7 sec
Load Avg:  1.1630859375  1.0185546875  0.955078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20690304 s          0 s    3432288 s  1206174590 s         40 s
#2  3501 MHz   54261011 s          0 s    3809597 s  1173022150 s         12 s
#3  3501 MHz   18236871 s          0 s    2297774 s  1211742981 s         19 s
#4  3501 MHz   15021436 s          0 s    2211804 s  1215152325 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.978
Commit 8a376a0 (2016-10-15 15:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13015.68359375 MB free)
Uptime: 1.2332385e7 sec
Load Avg:  0.9970703125  0.97607421875  0.94580078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20738104 s          0 s    3439281 s  1206481721 s         40 s
#2  3501 MHz   54361039 s          0 s    3817017 s  1173277039 s         12 s
#3  3501 MHz   18373958 s          0 s    2307555 s  1211958223 s         19 s
#4  3501 MHz   15068913 s          0 s    2218274 s  1215460509 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
