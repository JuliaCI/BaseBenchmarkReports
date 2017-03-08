# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5af4cc063e945c0be138749d644ba81b255644eb](https://github.com/JuliaLang/julia/commit/5af4cc063e945c0be138749d644ba81b255644eb) vs [JuliaLang/julia@78b96d067b038de22489a9337c751416b19c4e2b](https://github.com/JuliaLang/julia/commit/78b96d067b038de22489a9337c751416b19c4e2b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20853#issuecomment-284962317)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.39 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 1.32 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 1.28 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.28 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.30 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.29 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.36 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.31 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.29 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","BitArray{2}")]` | 1.10 (50%)  | 1.63 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.25 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.31 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.36 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.67 (50%) :x: | 1.87 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 2.41 (50%) :x: | 1.87 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.31 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.25 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.25 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.27 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.24 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 2.91 (50%) :x: | 1.87 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 2.47 (50%) :x: | 1.87 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.27 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.23 (50%)  | 1.17 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 1.04 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.04 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.06 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.06 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.06 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 1.06 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.92 (50%) :x: | 1.12 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.04 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 4.09 (50%) :x: | 1.57 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 4.01 (50%) :x: | 1.57 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.04 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.93 (50%) :x: | 1.12 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.03 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 4.30 (50%) :x: | 1.57 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 4.10 (50%) :x: | 1.57 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.05 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.03 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 5.41 (50%) :x: | 1.33 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 17.10 (50%) :x: | 1.80 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 13.30 (50%) :x: | 1.80 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 5.04 (50%) :x: | 1.33 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 16.84 (50%) :x: | 1.80 (1%) :x: |
| `["array","index",("sumvector_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 13.43 (50%) :x: | 1.80 (1%) :x: |
| `["dates","accessor","hour"]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","millisecond"]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 0.39 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Month")]` | 0.71 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Year")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.73 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.98 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.51 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.82 (45%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 0.91 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 0.88 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 0.85 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 0.86 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 0.87 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 0.88 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 0.92 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","UInt64")]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 0.78 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 0.70 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 0.84 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 0.80 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 0.82 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 0.75 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 0.84 (50%)  | 0.92 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 0.77 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 0.81 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 0.77 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 0.80 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 0.90 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 0.84 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 0.90 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 0.87 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 0.82 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 0.89 (50%)  | 0.95 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 0.83 (50%)  | 0.91 (1%) :white_check_mark: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 0.91 (50%)  | 0.95 (1%) :white_check_mark: |
| `["sparse","index",("spmat","logical",100)]` | 1.44 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.alpha.86
Commit 5af4cc0 (2017-03-08 06:51 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8240.13671875 MB free)
Uptime: 2.4607911e7 sec
Load Avg:  0.9228515625  0.998046875  1.0400390625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52061796 s          0 s    8057250 s  2395413502 s         74 s
#2  3501 MHz  187008153 s          0 s    8576691 s  2261219215 s         26 s
#3  3501 MHz   42989547 s          0 s    5036016 s  2411649975 s         39 s
#4  3501 MHz   38799208 s          0 s    4974638 s  2416131743 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.alpha.77
Commit 78b96d0 (2017-03-08 03:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (7797.796875 MB free)
Uptime: 2.4614232e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   52155713 s          0 s    8067720 s  2395938898 s         75 s
#2  3501 MHz  187583108 s          0 s    8585070 s  2261267312 s         26 s
#3  3501 MHz   43073901 s          0 s    5044211 s  2412188804 s         39 s
#4  3501 MHz   38878688 s          0 s    4982802 s  2416675632 s         13 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
