# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@98479af54034aa813f03f24a93b5760d22f48db6](https://github.com/JuliaLang/julia/commit/98479af54034aa813f03f24a93b5760d22f48db6) vs [JuliaLang/julia@87746274eb249a7e81c04437f37e9d9999636f34](https://github.com/JuliaLang/julia/commit/87746274eb249a7e81c04437f37e9d9999636f34)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/98479af54034aa813f03f24a93b5760d22f48db6#commitcomment-22040407)

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
| `["array","cat",("hcat",5)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 0.58 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 2.13 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("mean","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sum","Float64")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("sumabs","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 2.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.88 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 1.67 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.65 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.80 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","go","go_game"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 2.44 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 2.54 (15%) :x: | 1.00 (1%)  |
| `["problem","monte carlo","euro_option_vec"]` | 1.34 (15%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 2.58 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","meteor_contest"]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["shootout","pidigits"]` | 2.03 (15%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.93 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.46 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 2.12 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.5.2-pre+57
Commit 98479af (2017-05-04 15:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9127.10546875 MB free)
Uptime: 2.9680614e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61354935 s          0 s   11598718 s  2886462863 s         78 s
#2  3501 MHz  249465733 s          0 s    7278600 s  2709574383 s         12 s
#3  3501 MHz   54842157 s          0 s    6463794 s  2905322311 s         62 s
#4  3501 MHz   51964616 s          0 s    6617656 s  2908045855 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.2-pre+54
Commit 8774627 (2017-05-04 08:57 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9252.36328125 MB free)
Uptime: 2.9689558e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61440602 s          0 s   11609578 s  2887257460 s         78 s
#2  3501 MHz  250299074 s          0 s    7297603 s  2709615848 s         12 s
#3  3501 MHz   54916264 s          0 s    6472004 s  2906133614 s         62 s
#4  3501 MHz   52042375 s          0 s    6625266 s  2908854331 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
