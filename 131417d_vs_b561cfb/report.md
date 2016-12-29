# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@131417ddfc074270f781912bf5e42e465a002019](https://github.com/JuliaLang/julia/commit/131417ddfc074270f781912bf5e42e465a002019) vs [JuliaLang/julia@b561cfbfbd2b845cb05e8263a86e22dd665fe723](https://github.com/JuliaLang/julia/commit/b561cfbfbd2b845cb05e8263a86e22dd665fe723)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19730#issuecomment-269662049)

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
| `["array","cat",("catnd",5)]` | 1.55 (15%) :x: | 1.28 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 1.18 (15%) :x: | 1.06 (1%) :x: |
| `["array","cat",("vcat",5)]` | 0.99 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 1.10 (15%)  | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 1.05 (50%)  | 1.08 (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 1.01 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000000:-1:1")]` | 0.99 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000000")]` | 1.04 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.10 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.12 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.19 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.18 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.16 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.14 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.18 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.17 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.06 (50%)  | 0.14 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.16 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.17 (50%)  | 0.38 (1%) :white_check_mark: |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 0.79 (50%)  | 0.52 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 3.35 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.23 (15%) :x: | 1.40 (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 1.16 (15%) :x: | 1.22 (1%) :x: |
| `["problem","go","go_game"]` | 1.03 (15%)  | 1.11 (1%) :x: |
| `["scalar","floatexp",("exponent","subnorm","Float64")]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1752
Commit 131417d (2016-12-29 17:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5407.9296875 MB free)
Uptime: 1.8683829e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25754124 s          0 s    6039680 s  1831245855 s         59 s
#2  3501 MHz   81562262 s          0 s    3682642 s  1782023896 s          8 s
#3  3501 MHz   24729680 s          0 s    3183984 s  1839607916 s         39 s
#4  3501 MHz   22286367 s          0 s    3276627 s  1841938192 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1748
Commit b561cfb (2016-12-29 09:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5508.41015625 MB free)
Uptime: 1.8690116e7 sec
Load Avg:  0.9228515625  0.998046875  0.96240234375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25793040 s          0 s    6047008 s  1831826253 s         59 s
#2  3501 MHz   81955854 s          0 s    3690595 s  1782250478 s          8 s
#3  3501 MHz   24826799 s          0 s    3193041 s  1840129687 s         39 s
#4  3501 MHz   22354711 s          0 s    3283912 s  1842490712 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
