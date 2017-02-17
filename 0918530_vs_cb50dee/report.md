# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0918530782cb26109e57246a04b5be0ff525b7b9](https://github.com/JuliaLang/julia/commit/0918530782cb26109e57246a04b5be0ff525b7b9) vs [JuliaLang/julia@cb50dee5edec12bf214c29299df008f09a2e043c](https://github.com/JuliaLang/julia/commit/cb50dee5edec12bf214c29299df008f09a2e043c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20626#issuecomment-280631316)

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
| `["array","bool","bitarray_true_fill!"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.45 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem","json","parse_json"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","range",100)]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.44 (30%) :x: | 1.00 (1%)  |

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

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.2843
Commit 0918530 (2017-02-17 08:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2860.5546875 MB free)
Uptime: 2.2984809e7 sec
Load Avg:  0.94140625  1.0068359375  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   38663742 s          0 s    8177744 s  2244986432 s         66 s
#2  3501 MHz  134402466 s          0 s    4842622 s  2157909170 s          8 s
#3  3501 MHz   34450429 s          0 s    4243380 s  2258719734 s         48 s
#4  3501 MHz   32132986 s          0 s    4379288 s  2260894686 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2840
Commit cb50dee (2017-02-17 08:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2839.59765625 MB free)
Uptime: 2.2991075e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   38747400 s          0 s    8187408 s  2245517214 s         66 s
#2  3501 MHz  134974759 s          0 s    4851394 s  2157954077 s          8 s
#3  3501 MHz   34547330 s          0 s    4251597 s  2259240431 s         49 s
#4  3501 MHz   32211568 s          0 s    4387499 s  2261433804 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
