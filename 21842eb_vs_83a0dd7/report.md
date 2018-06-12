# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@21842eb9542ed530c6dcbeec8e6ed189830bba63](https://github.com/JuliaLang/julia/commit/21842eb9542ed530c6dcbeec8e6ed189830bba63) vs [JuliaLang/julia@83a0dd79cd39ff2f62c6f353f6daa7110a73d2c4](https://github.com/JuliaLang/julia/commit/83a0dd79cd39ff2f62c6f353f6daa7110a73d2c4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27499#issuecomment-396413224)

*Tag Predicate:* `"string"`

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

- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["problem", "spellcheck"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha.84
Commit 21842eb (2018-06-11 22:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   26868065 s        276 s    2905600 s  627465155 s          6 s
       #2  3501 MHz  107946776 s          0 s    1525956 s  549503027 s          3 s
       #3  3501 MHz   14101227 s       2373 s    1223248 s  643326746 s          8 s
       #4  3501 MHz   13270606 s          0 s    1457533 s  644081217 s          5 s
       
  Memory: 31.383651733398438 GB (3026.4765625 MB free)
  Uptime: 6.593252e6 sec
  Load Avg:  0.9228515625  0.998046875  1.0849609375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.79
Commit 83a0dd7 (2018-06-11 21:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   27011801 s        276 s    2915149 s  627732699 s          6 s
       #2  3501 MHz  108276452 s          0 s    1534984 s  549586421 s          3 s
       #3  3501 MHz   14219478 s       2373 s    1232568 s  643620984 s          8 s
       #4  3501 MHz   13381390 s          0 s    1466533 s  644383364 s          5 s
       
  Memory: 31.383651733398438 GB (2971.85546875 MB free)
  Uptime: 6.597477e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.111328125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
