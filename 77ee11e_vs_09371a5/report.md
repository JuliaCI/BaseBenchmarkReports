# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@77ee11ee7325a6ce3c8fb380fe91f8f4f44292a0](https://github.com/JuliaLang/julia/commit/77ee11ee7325a6ce3c8fb380fe91f8f4f44292a0) vs [JuliaLang/julia@09371a5c904348b4f7883dac8e3e034818678e87](https://github.com/JuliaLang/julia/commit/09371a5c904348b4f7883dac8e3e034818678e87)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22974#issuecomment-319099908)

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
| `["array","bool","bitarray_true_fill!"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd",500)]` | 1.47 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("catnd_setind",500)]` | 1.77 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",500)]` | 2.05 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",500)]` | 1.90 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat",500)]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",500)]` | 1.77 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat",500)]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",500)]` | 1.71 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("append!",2048)]` | 1.07 (15%)  | 0.53 (1%) :white_check_mark: |
| `["array","growth",("append!",256)]` | 0.93 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("append!",8)]` | 1.03 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("prerend!",2048)]` | 1.64 (15%) :x: | 0.57 (1%) :white_check_mark: |
| `["array","growth",("prerend!",256)]` | 1.01 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("prerend!",8)]` | 1.03 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","growth",("push_multiple!",2048)]` | 1.16 (15%) :x: | 0.67 (1%) :white_check_mark: |
| `["array","growth",("push_multiple!",256)]` | 0.97 (15%)  | 0.53 (1%) :white_check_mark: |
| `["array","growth",("push_multiple!",8)]` | 1.10 (15%)  | 0.50 (1%) :white_check_mark: |
| `["array","index",("sumcolon","100000:-1:1")]` | 1.62 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","100000:-1:1")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 1.05 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 1.09 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 1.03 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 1.07 (15%)  | 1.32 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 1.00 (15%)  | 1.32 (1%) :x: |
| `["broadcast","sparse",((10000000,),1)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 1.82 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 0.99 (15%)  | 1.02 (1%) :x: |
| `["io","read","readstring"]` | 1.00 (15%)  | 1.01 (1%) :x: |
| `["io","serialization",("deserialize","Matrix{Float64}")]` | 2.02 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Bidiagonal","Vector",1024)]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.57 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Diagonal",1024)]` | 1.82 (45%) :x: | 1.00 (1%)  |
| `["misc","julia",("macroexpand","evalpoly")]` | 0.95 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",1024)]` | 1.05 (15%)  | 1.04 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.00 (15%)  | 1.07 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 0.98 (15%)  | 1.01 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 0.97 (15%)  | 1.05 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 0.99 (15%)  | 1.06 (1%) :x: |
| `["problem","imdb","centrality"]` | 0.90 (15%)  | 1.03 (1%) :x: |
| `["problem","stockcorr","stockcorr"]` | 0.54 (15%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 0.98 (25%)  | 1.01 (1%) :x: |
| `["scalar","predicate",("isequal","BigInt")]` | 2.32 (40%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.00 (25%)  | 0.83 (1%) :white_check_mark: |
| `["simd",("local_arrays","Int64",4095)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(600,600))]` | 1.31 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","OneTo",1000)]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",1000)]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","row","OneTo",10)]` | 1.57 (30%) :x: | 1.56 (1%) :x: |
| `["sparse","index",("spmat","row","OneTo",100)]` | 1.48 (30%) :x: | 1.29 (1%) :x: |
| `["sparse","index",("spmat","row","OneTo",1000)]` | 1.04 (30%)  | 0.68 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",10)]` | 1.54 (30%) :x: | 1.56 (1%) :x: |
| `["sparse","index",("spmat","row","array",100)]` | 1.49 (30%) :x: | 0.96 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.05 (30%)  | 0.68 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 1.38 (30%) :x: | 1.38 (1%) :x: |
| `["sparse","index",("spmat","row","logical",100)]` | 1.19 (30%)  | 1.19 (1%) :x: |
| `["sparse","index",("spmat","row","range",10)]` | 1.58 (30%) :x: | 1.56 (1%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.33 (30%) :x: | 1.29 (1%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.02 (30%)  | 0.68 (1%) :white_check_mark: |

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
Julia Version 0.7.0-DEV.1172
Commit 77ee11e (2017-07-31 15:19 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77088863 s          0 s   11942760 s  3619464452 s        126 s
       #2  3501 MHz  301594262 s          0 s   12831353 s  3395565264 s         42 s
       #3  3501 MHz   65100749 s          0 s    7505612 s  3642397709 s         61 s
       #4  3501 MHz   60524233 s          0 s    7437888 s  3647387548 s         21 s
       
  Memory: 31.383651733398438 GB (4734.609375 MB free)
  Uptime: 3.7166344e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1169
Commit 09371a5 (2017-07-31 13:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77167370 s          0 s   11952414 s  3620053999 s        127 s
       #2  3501 MHz  302211728 s          0 s   12842326 s  3395616408 s         42 s
       #3  3501 MHz   65197772 s          0 s    7512899 s  3642972954 s         61 s
       #4  3501 MHz   60605353 s          0 s    7445092 s  3647979026 s         21 s
       
  Memory: 31.383651733398438 GB (4538.29296875 MB free)
  Uptime: 3.7173147e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
