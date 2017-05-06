# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@87448f2f882e1dd91e141d6657a21b7c5b0bedde](https://github.com/JuliaLang/julia/commit/87448f2f882e1dd91e141d6657a21b7c5b0bedde) vs [JuliaLang/julia@f797f92465e59893ae8f51ac1a6dd30605b26cf2](https://github.com/JuliaLang/julia/commit/f797f92465e59893ae8f51ac1a6dd30605b26cf2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/87448f2f882e1dd91e141d6657a21b7c5b0bedde#commitcomment-22042356)

*Tag Predicate:* `ALL`

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("prerend!",2048)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",2048)]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",256)]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("push_multiple!",8)]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","2d"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("mean","Float64")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("sum","Float64")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","reductions",("sumabs2","Float64")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.59 (40%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","sparse"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.2-pre+65
Commit 87448f2 (2017-05-04 21:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9449.8515625 MB free)
Uptime: 2.9725221e7 sec
Load Avg:  1.01513671875  1.021484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   62226220 s          0 s    9574516 s  2894351749 s         87 s
#2  3501 MHz  240024821 s          0 s   10570870 s  2716423382 s         35 s
#3  3501 MHz   53100141 s          0 s    6171197 s  2911911496 s         45 s
#4  3501 MHz   48637346 s          0 s    6111323 s  2916715337 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.2-pre+49
Commit f797f92 (2017-05-03 06:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9250.484375 MB free)
Uptime: 2.9731242e7 sec
Load Avg:  1.0234375  1.0390625  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   62301838 s          0 s    9584942 s  2894865479 s         87 s
#2  3501 MHz  240585222 s          0 s   10579761 s  2716455584 s         35 s
#3  3501 MHz   53176022 s          0 s    6179690 s  2912428516 s         45 s
#4  3501 MHz   48718547 s          0 s    6119504 s  2917227562 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
