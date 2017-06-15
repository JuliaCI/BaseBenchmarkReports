# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7e190bfc9dcdde443e4c84b1a389ef7af2a6461c](https://github.com/JuliaLang/julia/commit/7e190bfc9dcdde443e4c84b1a389ef7af2a6461c) vs [JuliaLang/julia@1a3391f9c849ea812990f63f1619f1a244963c44](https://github.com/JuliaLang/julia/commit/1a3391f9c849ea812990f63f1619f1a244963c44)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21728#issuecomment-308857958)

*Tag Predicate:* `"broadcast" && "dotop"`

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

- `["broadcast","dotop"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.601
Commit 7e190bf (2017-06-15 18:20 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   69288273 s          0 s   10679811 s  3233530995 s         92 s
       #2  3501 MHz  271756664 s          0 s   11698608 s  3031156299 s         38 s
       #3  3501 MHz   59582628 s          0 s    6933453 s  3252602434 s         49 s
       #4  3501 MHz   55053467 s          0 s    6851630 s  3257534506 s         17 s
       
  Memory: 31.383651733398438 GB (2996.171875 MB free)
  Uptime: 3.320628e7 sec
  Load Avg:  1.0029296875  1.75830078125  1.9189453125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.598
Commit 1a3391f (2017-06-15 18:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   69384333 s          0 s   10688572 s  3233578888 s         92 s
       #2  3501 MHz  271855203 s          0 s   11706914 s  3031202278 s         38 s
       #3  3501 MHz   59667745 s          0 s    6941934 s  3252661506 s         49 s
       #4  3501 MHz   55138382 s          0 s    6860160 s  3257593847 s         17 s
       
  Memory: 31.383651733398438 GB (2891.3828125 MB free)
  Uptime: 3.3207814e7 sec
  Load Avg:  1.0029296875  1.7578125  2.2578125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
