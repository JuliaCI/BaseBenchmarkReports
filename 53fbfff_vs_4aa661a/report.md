# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@53fbfffdd6279565c97bf5256a8b385edb324b48](https://github.com/JuliaLang/julia/commit/53fbfffdd6279565c97bf5256a8b385edb324b48) vs [JuliaLang/julia@4aa661a0c1b6361bb254cbf974a79cdec0c08d2e](https://github.com/JuliaLang/julia/commit/4aa661a0c1b6361bb254cbf974a79cdec0c08d2e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23670#issuecomment-334878279)

*Tag Predicate:* `"misc"`

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
| `["misc","repeat",(200,1,24)]` | 0.83 (15%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["misc","repeat",(200,24,1)]` | 0.31 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.1-pre.92
Commit 53fbfff (2017-10-06 22:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3590.890625 MB free)
Uptime: 4.2977169e7 sec
Load Avg:  1.01220703125  1.5966796875  1.99560546875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   89086342 s          0 s   13812142 s  4185209388 s        180 s
#2  3501 MHz  360876368 s          0 s   14860093 s  3914419818 s         64 s
#3  3501 MHz   74833064 s          0 s    8519734 s  4212522432 s         84 s
#4  3501 MHz   70038396 s          0 s    8396512 s  4217843334 s         31 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.1-pre.3
Commit 4aa661a (2017-09-14 17:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3576.53515625 MB free)
Uptime: 4.2978794e7 sec
Load Avg:  1.02099609375  1.7021484375  2.21240234375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   89171373 s          0 s   13820822 s  4185277373 s        180 s
#2  3501 MHz  360979489 s          0 s   14868958 s  3914469528 s         65 s
#3  3501 MHz   74920934 s          0 s    8528612 s  4212587217 s         85 s
#4  3501 MHz   70135019 s          0 s    8405012 s  4217900067 s         31 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
