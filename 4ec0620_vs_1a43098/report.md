# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4ec06208e7bcaea675531a0250ff5853f72dbaac](https://github.com/JuliaLang/julia/commit/4ec06208e7bcaea675531a0250ff5853f72dbaac) vs [JuliaLang/julia@1a43098cf7868045e64f051146484dbb2d132633](https://github.com/JuliaLang/julia/commit/1a43098cf7868045e64f051146484dbb2d132633)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22974#issuecomment-318962667)

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
| `["array","cat",("catnd",500)]` | 1.45 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",500)]` | 1.68 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",500)]` | 1.98 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",500)]` | 1.74 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",500)]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",500)]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat",500)]` | 1.64 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",500)]` | 1.67 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",2048)]` | 1.05 (15%)  | 0.53 (1%) :white_check_mark: |
| `["array","growth",("append!",256)]` | 0.93 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("append!",8)]` | 0.98 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("prerend!",2048)]` | 1.43 (15%) :x: | 0.57 (1%) :white_check_mark: |
| `["array","growth",("prerend!",256)]` | 1.06 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("prerend!",8)]` | 0.97 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("push_multiple!",2048)]` | 1.03 (15%)  | 0.67 (1%) :white_check_mark: |
| `["array","growth",("push_multiple!",256)]` | 0.93 (15%)  | 0.53 (1%) :white_check_mark: |
| `["array","growth",("push_multiple!",8)]` | 1.00 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumcolon","100000:-1:1")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000:-1:1")]` | 1.59 (50%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 1.08 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 1.06 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 1.10 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 1.08 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 1.08 (15%)  | 1.32 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.42 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),1)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 1.80 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.02 (15%)  | 1.02 (1%) :x: |
| `["dates","string","Date"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["io","read","readstring"]` | 1.08 (15%)  | 1.01 (1%) :x: |
| `["io","serialization",("deserialize","Matrix{Float64}")]` | 2.00 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 1.66 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 1.71 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 1.54 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 1.51 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["misc","julia",("macroexpand","evalpoly")]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["misc","repeat",(200,1,24)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["misc","repeat",(200,24,1)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.00 (15%)  | 1.04 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 0.99 (15%)  | 1.07 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 0.99 (15%)  | 1.05 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 0.99 (15%)  | 1.06 (1%) :x: |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 0.99 (15%)  | 1.03 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.35 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","ziggurat","ziggurat"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Int32")]` | 0.79 (25%)  | 0.94 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 0.97 (25%)  | 0.83 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int64",4096)]` | 1.25 (20%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(600,600))]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","OneTo",100)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","OneTo",1000)]` | 1.53 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 1.52 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","OneTo",10)]` | 1.39 (30%) :x: | 1.56 (1%) :x: |
| `["sparse","index",("spmat","row","OneTo",100)]` | 1.47 (30%) :x: | 1.29 (1%) :x: |
| `["sparse","index",("spmat","row","OneTo",1000)]` | 1.03 (30%)  | 0.68 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",10)]` | 1.29 (30%)  | 1.56 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.43 (30%) :x: | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.07 (30%)  | 0.68 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.27 (30%)  | 1.38 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.18 (30%)  | 1.19 (1%) :x: |
| `["sparse","index",("spmat","row","range",10)]` | 1.29 (30%)  | 1.56 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.38 (30%) :x: | 1.29 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.11 (30%)  | 0.68 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",10000)]` | 1.42 (30%) :x: | 1.00 (1%)  |

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
- `["scalar","arithmetic"]`
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
Julia Version 0.7.0-DEV.1167
Commit 4ec0620 (2017-07-31 04:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   76927292 s          0 s   11924914 s  3615619613 s        126 s
       #2  3501 MHz  300512207 s          0 s   12799366 s  3392656149 s         42 s
       #3  3501 MHz   64941470 s          0 s    7490520 s  3638541050 s         60 s
       #4  3501 MHz   60353450 s          0 s    7422994 s  3643541714 s         21 s
       
  Memory: 31.383651733398438 GB (4906.79296875 MB free)
  Uptime: 3.7126015e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1165
Commit 1a43098 (2017-07-31 03:33 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77010294 s          0 s   11933466 s  3616119170 s        126 s
       #2  3501 MHz  301059609 s          0 s   12810888 s  3392689905 s         42 s
       #3  3501 MHz   65021864 s          0 s    7498006 s  3639045766 s         60 s
       #4  3501 MHz   60429718 s          0 s    7430353 s  3644050981 s         21 s
       
  Memory: 31.383651733398438 GB (4615.91015625 MB free)
  Uptime: 3.713195e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
