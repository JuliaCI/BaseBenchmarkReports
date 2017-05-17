# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@be004c1bfebb585932c78c8922b06bde049fb2cb](https://github.com/JuliaLang/julia/commit/be004c1bfebb585932c78c8922b06bde049fb2cb) vs [JuliaLang/julia@6bdb3950bdf64152](https://github.com/JuliaLang/julia/commit/6bdb3950bdf64152)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/be004c1bfebb585932c78c8922b06bde049fb2cb#commitcomment-22178786)

*Tag Predicate:* `"parse"`

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

- `["dates","parse"]`
- `["micro"]`
- `["misc","parse"]`
- `["problem","json"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-rc1.80
Commit be004c1 (2017-05-17 07:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8274.453125 MB free)
Uptime: 3.0687308e7 sec
Load Avg:  0.99365234375  1.650390625  2.17626953125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   63919793 s          0 s    9868068 s  2988359284 s         89 s
#2  3501 MHz  247928276 s          0 s   10865152 s  2804311202 s         36 s
#3  3501 MHz   54851560 s          0 s    6382650 s  3006109607 s         47 s
#4  3501 MHz   50423955 s          0 s    6331031 s  3010871229 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-rc1.0
Commit 6bdb395 (2017-05-07 00:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8260.734375 MB free)
Uptime: 3.0688869e7 sec
Load Avg:  1.01513671875  1.7294921875  2.27490234375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   64005873 s          0 s    9877076 s  2988419722 s         89 s
#2  3501 MHz  248030559 s          0 s   10873538 s  2804356206 s         36 s
#3  3501 MHz   54936219 s          0 s    6391183 s  3006171919 s         47 s
#4  3501 MHz   50519759 s          0 s    6339505 s  3010922569 s         17 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
