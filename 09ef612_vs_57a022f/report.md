# Benchmark Report

## Job Properties

*Commit(s):* [tkf/julia@09ef6124382c757e8a053832383e8822f7ddf30b](https://github.com/tkf/julia/commit/09ef6124382c757e8a053832383e8822f7ddf30b) vs [JuliaLang/julia@57a022f74ca7ace45df3eb5d0940201a297c270b](https://github.com/JuliaLang/julia/commit/57a022f74ca7ace45df3eb5d0940201a297c270b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/29634#issuecomment-521379846)

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

- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`

## Version Info

#### Primary Build

```
Julia Version 1.3.0-alpha.159
Commit 09ef612 (2019-08-14 18:24 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96382928 s       5041 s   11178248 s  4246760195 s         27 s
       #2  3501 MHz  646909915 s        208 s   11091270 s  3703215039 s         24 s
       #3  3501 MHz   79847419 s       3245 s    6633138 s  4274767712 s         32 s
       #4  3501 MHz   74901487 s         22 s    9394778 s  4275187631 s         22 s
       
  Memory: 31.383651733398438 GB (14994.15625 MB free)
  Uptime: 4.3644413e7 sec
  Load Avg:  0.9970703125  1.0361328125  1.3193359375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.3.0-alpha.112
Commit 57a022f (2019-08-14 18:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   96484868 s       5041 s   11183308 s  4246904191 s         27 s
       #2  3501 MHz  647092804 s        208 s   11096034 s  3703278723 s         24 s
       #3  3501 MHz   79957543 s       3245 s    6637872 s  4274904045 s         32 s
       #4  3501 MHz   75005620 s         22 s    9399298 s  4275330258 s         22 s
       
  Memory: 31.383651733398438 GB (14935.5625 MB free)
  Uptime: 4.3646929e7 sec
  Load Avg:  0.9228515625  1.02099609375  1.4033203125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
