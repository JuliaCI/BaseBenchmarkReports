# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a51c79a37218b05a6250836bdefeaadb16d53f7b](https://github.com/JuliaLang/julia/commit/a51c79a37218b05a6250836bdefeaadb16d53f7b) vs [JuliaLang/julia@29a35637b43855755398062844ae596e6cedfbc0](https://github.com/JuliaLang/julia/commit/29a35637b43855755398062844ae596e6cedfbc0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a51c79a37218b05a6250836bdefeaadb16d53f7b#commitcomment-20445433)

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
| `["array","cat",("catnd",5)]` | 1.21 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","DateTime"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.17 (15%) :x: | 1.01 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","DateFormat")]` | 1.16 (15%) :x: | 1.01 (1%)  |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 0.99 (45%)  | 0.99 (1%) :white_check_mark: |
| `["misc","parse","DateTime"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.23 (15%) :x: | 1.06 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.24 (15%) :x: | 1.09 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.21 (15%) :x: | 1.03 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.23 (15%) :x: | 1.07 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.23 (15%) :x: | 1.09 (1%) :x: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.97 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 0.85 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.98 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 0.84 (50%)  | 0.87 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 0.89 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 0.85 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 0.86 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 0.89 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 0.81 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.96 (50%)  | 0.88 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 1.00 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","predicate",("isfinite","Float32")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float32")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float64")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["shootout","nbody_vec"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","random")]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.48 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 1.46 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.45 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.42 (30%) :x: | 1.00 (1%)  |

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
?
```

#### Comparison Build

```
?
```
