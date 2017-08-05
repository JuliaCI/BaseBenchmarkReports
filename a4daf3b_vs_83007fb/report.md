# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@a4daf3b21f1a98dd208f50bc1b785d4d92f24d3b](https://github.com/pkofod/julia/commit/a4daf3b21f1a98dd208f50bc1b785d4d92f24d3b) vs [JuliaLang/julia@83007fb8c4c748fb23d38759daafd77fa1d56c2b](https://github.com/JuliaLang/julia/commit/83007fb8c4c748fb23d38759daafd77fa1d56c2b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23088#issuecomment-320467940)

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
| `["array","cat",("hcat",500)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 103.97 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 103.85 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 96.82 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 103.79 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= |x| < 0.975","positive argument","Float32")]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= |x| < 0.975","positive argument","Float64")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= |x| < 1.0","negative argument","Float64")]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= |x| < 1.0","positive argument","Float64")]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","negative argument","Float32")]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","negative argument","Float64")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float32")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("one","positive argument","Float64")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","negative argument","Float32")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","positive argument","Float32")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("small","positive argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float32")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("zero","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","negative argument","Float32")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","negative argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","positive argument","Float32")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("|x| < 0.5","positive argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (hard) abs(x) < 2π/4","negative argument","Float64","sin_kernel")]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(16,16))]` | 1.17 (15%) :x: | 1.00 (1%)  |

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
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
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
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
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
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1251
Commit a4daf3b (2017-08-05 19:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78050895 s          0 s   12066755 s  3663276543 s        131 s
       #2  3501 MHz  306856578 s          0 s   13052002 s  3434967228 s         46 s
       #3  3501 MHz   66166063 s          0 s    7603181 s  3686207020 s         62 s
       #4  3501 MHz   61521086 s          0 s    7533584 s  3691272517 s         21 s
       
  Memory: 31.383651733398438 GB (5937.46484375 MB free)
  Uptime: 3.7616228e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1248
Commit 83007fb (2017-08-05 18:12 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   78145706 s          0 s   12076012 s  3663784995 s        131 s
       #2  3501 MHz  307410962 s          0 s   13062977 s  3435016213 s         46 s
       #3  3501 MHz   66247294 s          0 s    7610405 s  3686732704 s         62 s
       #4  3501 MHz   61600013 s          0 s    7541058 s  3691800398 s         21 s
       
  Memory: 31.383651733398438 GB (5351.44921875 MB free)
  Uptime: 3.7622377e7 sec
  Load Avg:  1.02783203125  1.02490234375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
