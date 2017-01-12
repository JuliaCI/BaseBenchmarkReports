# Benchmark Report

## Job Properties

*Commit(s):* [ararslan/julia@459bc3a62c227c795747b217a870280ac4827e0b](https://github.com/ararslan/julia/commit/459bc3a62c227c795747b217a870280ac4827e0b) vs [JuliaLang/julia@7b7b4e1d24aa449bf33af93e684ca8924b66a010](https://github.com/JuliaLang/julia/commit/7b7b4e1d24aa449bf33af93e684ca8924b66a010)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19989#issuecomment-272170135)

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
| `["array","cat",("catnd_setind",5)]` | 1000.28 (15%) :x: | 12.30 (1%) :x: |
| `["array","cat",("catnd_setind",500)]` | 9.68 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("hcat_setind",5)]` | 60545.96 (15%) :x: | 182.23 (1%) :x: |
| `["array","cat",("hcat_setind",500)]` | 16.65 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("hvcat_setind",5)]` | 50720.80 (15%) :x: | 162.10 (1%) :x: |
| `["array","cat",("hvcat_setind",500)]` | 15.11 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("vcat_setind",5)]` | 59262.74 (15%) :x: | 182.23 (1%) :x: |
| `["array","cat",("vcat_setind",500)]` | 15.69 (15%) :x: | 1.02 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["shootout","fannkuch"]` | 81.75 (15%) :x: | 501.71 (1%) :x: |
| `["shootout","fasta"]` | 1849.15 (15%) :x: | 24.66 (1%) :x: |
| `["shootout","k_nucleotide"]` | 1.71 (15%) :x: | 1.04 (1%) :x: |

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
