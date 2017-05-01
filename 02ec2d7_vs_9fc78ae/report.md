# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@02ec2d7e46bdfd28f015e5738744e477564e7ca5](https://github.com/JuliaLang/julia/commit/02ec2d7e46bdfd28f015e5738744e477564e7ca5) vs [JuliaLang/julia@9fc78aeb763156c9041dc141054d57d9f2ae79aa](https://github.com/JuliaLang/julia/commit/9fc78aeb763156c9041dc141054d57d9f2ae79aa)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21654#issuecomment-298375974)

*Tag Predicate:* `"BigInt" || "Complex"`

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

- `["nullable","nullablearray"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","intfuncs"]`
- `["scalar","predicate"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.456
Commit 02ec2d7 (2017-05-01 17:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7156.59375 MB free)
Uptime: 2.9306158e7 sec
Load Avg:  1.0029296875  1.43603515625  1.72216796875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   58421353 s          0 s   11250086 s  2852422050 s         77 s
#2  3501 MHz  237883432 s          0 s    7014016 s  2684001708 s         11 s
#3  3501 MHz   52556872 s          0 s    6231794 s  2870419289 s         60 s
#4  3501 MHz   49759527 s          0 s    6386119 s  2873060606 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.454
Commit 9fc78ae (2017-05-01 17:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7105.734375 MB free)
Uptime: 2.930782e7 sec
Load Avg:  1.0029296875  1.42236328125  1.9794921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   58503645 s          0 s   11258640 s  2852496700 s         77 s
#2  3501 MHz  237995157 s          0 s    7022389 s  2684047291 s         11 s
#3  3501 MHz   52651670 s          0 s    6239750 s  2870482019 s         60 s
#4  3501 MHz   49838989 s          0 s    6394426 s  2873138464 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
