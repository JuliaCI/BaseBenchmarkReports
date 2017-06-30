# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fe71996f645c4c6566ced227ad6400d6057e22d4](https://github.com/JuliaLang/julia/commit/fe71996f645c4c6566ced227ad6400d6057e22d4) vs [JuliaLang/julia@c5093215fea47b93a2209502438d547f0e92573f](https://github.com/JuliaLang/julia/commit/c5093215fea47b93a2209502438d547f0e92573f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22635#issuecomment-312358576)

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
| `["array","cat",("catnd",5)]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","Date"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.77 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.98 (15%)  | 0.98 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.97 (15%)  | 0.91 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.93 (15%)  | 0.82 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.94 (15%)  | 0.96 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.96 (15%)  | 0.88 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.93 (15%)  | 0.84 (1%) :white_check_mark: |
| `["simd",("sum_reduce","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 0.65 (30%) :white_check_mark: | 1.00 (1%)  |

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
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
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
Julia Version 0.7.0-DEV.809
Commit fe71996 (2017-06-30 19:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71323515 s          0 s   10973576 s  3360656666 s         99 s
       #2  3501 MHz  281312278 s          0 s   12103828 s  3150654675 s         39 s
       #3  3501 MHz   61244850 s          0 s    7125036 s  3380414734 s         53 s
       #4  3501 MHz   56649534 s          0 s    7037550 s  3385432730 s         18 s
       
  Memory: 31.383651733398438 GB (4025.4453125 MB free)
  Uptime: 3.4503437e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.807
Commit c509321 (2017-06-30 19:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71401749 s          0 s   10982327 s  3361088353 s         99 s
       #2  3501 MHz  281776850 s          0 s   12111835 s  3150702057 s         39 s
       #3  3501 MHz   61325940 s          0 s    7132526 s  3380846152 s         53 s
       #4  3501 MHz   56741650 s          0 s    7044863 s  3385853497 s         18 s
       
  Memory: 31.383651733398438 GB (3608.375 MB free)
  Uptime: 3.4508644e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
