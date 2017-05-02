# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8915e9f1ab9c7a23933df583429ae857030e747c](https://github.com/JuliaLang/julia/commit/8915e9f1ab9c7a23933df583429ae857030e747c) vs [JuliaLang/julia@970a7427b62cf710db216432518290c24a465465](https://github.com/JuliaLang/julia/commit/970a7427b62cf710db216432518290c24a465465)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21670#issuecomment-298765738)

*Tag Predicate:* `"array" && "bool" || "simd"`

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
| `["array","bool","boolarray_true_load!"]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.46 (50%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.46 (50%) :white_check_mark: | 0.76 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","index"]`
- `["problem","seismic"]`
- `["simd"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.8
Commit 8915e9f (2017-05-02 21:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (1809.328125 MB free)
Uptime: 2.9408526e7 sec
Load Avg:  0.9228515625  1.02099609375  1.3193359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60270651 s          0 s    9312755 s  2864988526 s         85 s
#2  3501 MHz  227291255 s          0 s   10276682 s  2697826352 s         34 s
#3  3501 MHz   51108728 s          0 s    5961522 s  2882466684 s         45 s
#4  3501 MHz   46647720 s          0 s    5903288 s  2887262010 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.6
Commit 970a742 (2017-05-02 21:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (1819.33984375 MB free)
Uptime: 2.9410933e7 sec
Load Avg:  1.0029296875  1.0390625  1.43359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60356206 s          0 s    9321267 s  2865134119 s         85 s
#2  3501 MHz  227475386 s          0 s   10285292 s  2697873755 s         34 s
#3  3501 MHz   51194494 s          0 s    5970048 s  2882612328 s         45 s
#4  3501 MHz   46739412 s          0 s    5911945 s  2887401734 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
