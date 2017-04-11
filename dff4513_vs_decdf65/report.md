# Benchmark Report

## Job Properties

*Commit(s):* [TotalVerb/julia@dff45133bc437e421f5bbe166c75b2918b18af12](https://github.com/TotalVerb/julia/commit/dff45133bc437e421f5bbe166c75b2918b18af12) vs [JuliaLang/julia@decdf651c3ed4e3925d32b9cd6e469c1a405141c](https://github.com/JuliaLang/julia/commit/decdf651c3ed4e3925d32b9cd6e469c1a405141c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21328#issuecomment-293329531)

*Tag Predicate:* `"broadcast" || "nullable"`

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
- `["broadcast","fusion"]`
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.104
Commit dff4513 (2017-04-11 14:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2541.32421875 MB free)
Uptime: 2.757793e7 sec
Load Avg:  1.0029296875  1.40869140625  1.72802734375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53522353 s          0 s   10444487 s  2685812490 s         74 s
#2  3501 MHz  213448594 s          0 s    6423328 s  2536314611 s         11 s
#3  3501 MHz   47497932 s          0 s    5686734 s  2703288443 s         57 s
#4  3501 MHz   44912112 s          0 s    5822340 s  2705745094 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.100
Commit decdf65 (2017-04-11 14:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2512.9921875 MB free)
Uptime: 2.7579622e7 sec
Load Avg:  0.92333984375  1.46484375  2.00732421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   53616980 s          0 s   10452682 s  2685878178 s         74 s
#2  3501 MHz  213558550 s          0 s    6431514 s  2536365196 s         11 s
#3  3501 MHz   47581495 s          0 s    5694930 s  2703365297 s         57 s
#4  3501 MHz   44992040 s          0 s    5830674 s  2705825512 s         11 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
