# Benchmark Report

## Job Properties

*Commit(s):* [wsshin/julia@8cf53f288b4f88726f01d01a647a287b99c1de42](https://github.com/wsshin/julia/commit/8cf53f288b4f88726f01d01a647a287b99c1de42) vs [JuliaLang/julia@dc6c583ccf46fbe0e982bce90b7fd72f5f71b728](https://github.com/JuliaLang/julia/commit/dc6c583ccf46fbe0e982bce90b7fd72f5f71b728)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21446#issuecomment-296338928)

*Tag Predicate:* `"broadcast" || "tuple"`

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
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 0.23 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 0.21 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",5)]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.20 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.249
Commit 8cf53f2 (2017-04-22 00:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2817.1875 MB free)
Uptime: 2.8473198e7 sec
Load Avg:  1.00732421875  1.61669921875  1.81494140625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   56216280 s          0 s   10889325 s  2771927521 s         77 s
#2  3501 MHz  228901458 s          0 s    6742264 s  2610015670 s         11 s
#3  3501 MHz   50289263 s          0 s    5984811 s  2789679878 s         59 s
#4  3501 MHz   47585488 s          0 s    6126245 s  2792248028 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.244
Commit dc6c583 (2017-04-22 00:08 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2795.49609375 MB free)
Uptime: 2.8474772e7 sec
Load Avg:  0.99169921875  1.5625  2.103515625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   56299381 s          0 s   10898077 s  2771992447 s         77 s
#2  3501 MHz  229002698 s          0 s    6750848 s  2610062651 s         11 s
#3  3501 MHz   50370836 s          0 s    5993048 s  2789746799 s         59 s
#4  3501 MHz   47680576 s          0 s    6134396 s  2792301772 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
