# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@8829433fc4c38be9eac6f4f3203b65f6f9b618b8](https://github.com/pabloferz/julia/commit/8829433fc4c38be9eac6f4f3203b65f6f9b618b8) vs [JuliaLang/julia@466da651c058b2a0d55cc42efe6c7d4c5ee8270a](https://github.com/JuliaLang/julia/commit/466da651c058b2a0d55cc42efe6c7d4c5ee8270a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16865#issuecomment-225304673)

*Tag Predicate:* `"problem"`

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

- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem"]`
- `["problem","seismic"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4663
Commit 8829433 (2016-06-10 20:40 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28021.265625 MB free)
Uptime: 1.243932e6 sec
Load Avg:  0.97900390625  0.9326171875  0.8857421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     642079 s          0 s     265792 s  123172752 s          4 s
#2  3501 MHz    2339638 s          0 s     168223 s  121811153 s          0 s
#3  3501 MHz    1077382 s          0 s     177138 s  123068824 s          0 s
#4  3501 MHz    1021371 s          0 s     161018 s  123148574 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4660
Commit 466da65 (2016-06-10 20:39 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28010.1171875 MB free)
Uptime: 1.247175e6 sec
Load Avg:  0.99169921875  0.94287109375  0.92822265625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     678250 s          0 s     271409 s  123454289 s          4 s
#2  3501 MHz    2411631 s          0 s     175317 s  122055958 s          0 s
#3  3501 MHz    1124972 s          0 s     182558 s  123339367 s          0 s
#4  3501 MHz    1161403 s          0 s     171158 s  123322306 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
