# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@26eb512367936550a0fd1c6414f09215845f6eb1](https://github.com/JuliaLang/julia/commit/26eb512367936550a0fd1c6414f09215845f6eb1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/26eb512367936550a0fd1c6414f09215845f6eb1#commitcomment-25524191)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-11-10

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

| ID | time | GC time | memory | allocations |
|----|------|---------|--------|-------------|
| `["array", "bool", "bitarray_bool_load!"]` | 2.449 ms (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "bitarray_true_fill!"]` | 3.081 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "bitarray_true_load!"]` | 1.543 ms (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "boolarray_bool_load!"]` | 922.062 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "boolarray_true_fill!"]` | 33.249 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "boolarray_true_load!"]` | 514.302 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "cat", "(\"catnd\", 5)"]` | 17.934 μs (15%) | 0.000 ns | 19.11 KiB (1%) | 106 |
| `["array", "cat", "(\"catnd\", 500)"]` | 2.308 ms (15%) | 0.000 ns | 11.46 MiB (1%) | 116 |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 9.080 μs (15%) | 0.000 ns | 15.59 KiB (1%) | 23 |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 1.493 ms (15%) | 0.000 ns | 11.46 MiB (1%) | 26 |
| `["array", "cat", "(\"hcat\", 5)"]` | 279.000 ns (15%) | 0.000 ns | 944 bytes (1%) | 2 |
| `["array", "cat", "(\"hcat\", 500)"]` | 626.900 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 3 |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 178.000 ns (15%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 779.593 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "cat", "(\"hvcat\", 5)"]` | 179.000 ns (15%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"hvcat\", 500)"]` | 866.800 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 162.000 ns (15%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 863.620 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "cat", "(\"vcat\", 5)"]` | 1.251 μs (15%) | 0.000 ns | 944 bytes (1%) | 2 |
| `["array", "cat", "(\"vcat\", 500)"]` | 878.866 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 4 |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 178.000 ns (15%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 841.394 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 21.483 ms (15%) | 8.103 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 37.009 ms (15%) | 8.124 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 21.042 ms (15%) | 8.112 ms | 76.29 MiB (1%) | 3 |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 37.301 ms (15%) | 8.108 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"comprehension_indexing\", \"Array{Float64,1}\")"]` | 70.778 ms (30%) | 8.103 ms | 76.29 MiB (1%) | 4 |
| `["array", "comprehension", "(\"comprehension_indexing\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 116.509 ms (30%) | 8.115 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 73.329 ms (15%) | 8.100 ms | 76.29 MiB (1%) | 3 |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 93.185 ms (15%) | 8.102 ms | 76.29 MiB (1%) | 2 |
| `["array", "convert", "(\"Complex{Float64}\", \"Int\")"]` | 6.692 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "convert", "(\"Float64\", \"Int\")"]` | 5.161 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 19.640 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "convert", "(\"Int\", \"Float64\")"]` | 15.422 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "growth", "(\"append!\", 2048)"]` | 2.571 μs (15%) | 0.000 ns | 32.06 KiB (1%) | 1 |
| `["array", "growth", "(\"append!\", 256)"]` | 344.000 ns (15%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["array", "growth", "(\"append!\", 8)"]` | 42.000 ns (15%) | 0.000 ns | 144 bytes (1%) | 1 |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 2.270 μs (15%) | 0.000 ns | 64.06 KiB (1%) | 1 |
| `["array", "growth", "(\"prerend!\", 256)"]` | 338.000 ns (15%) | 0.000 ns | 8.06 KiB (1%) | 1 |
| `["array", "growth", "(\"prerend!\", 8)"]` | 55.000 ns (15%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["array", "growth", "(\"push_multiple!\", 2048)"]` | 10.916 μs (15%) | 0.000 ns | 32.06 KiB (1%) | 1 |
| `["array", "growth", "(\"push_multiple!\", 256)"]` | 1.505 μs (15%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 72.000 ns (15%) | 0.000 ns | 144 bytes (1%) | 1 |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 4.920 μs (15%) | 0.000 ns | 38.95 KiB (1%) | 8 |
| `["array", "growth", "(\"push_single!\", 256)"]` | 3.847 μs (15%) | 0.000 ns | 10.95 KiB (1%) | 8 |
| `["array", "growth", "(\"push_single!\", 8)"]` | 3.467 μs (15%) | 0.000 ns | 7.03 KiB (1%) | 8 |
| `["array", "index", "(\"mapr_access\", \"Array{Float32,2}\")"]` | 10.909 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"Array{Int32,2}\")"]` | 10.181 ms (50%) | 0.000 ns | 7.71 MiB (1%) | 503500 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 87.688 ms (50%) | 12.161 ms | 26.86 MiB (1%) | 1257000 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 88.201 ms (50%) | 12.120 ms | 26.82 MiB (1%) | 1255000 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 10.112 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 10.173 ms (50%) | 0.000 ns | 7.71 MiB (1%) | 503500 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 10.192 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 10.695 ms (50%) | 0.000 ns | 7.71 MiB (1%) | 503500 |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 70.919 ms (50%) | 0.000 ns | 19.18 MiB (1%) | 754000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 85.420 ms (50%) | 12.190 ms | 26.86 MiB (1%) | 1257000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 10.096 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 90.440 ms (50%) | 12.166 ms | 26.86 MiB (1%) | 1257000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 8.435 μs (50%) | 0.000 ns | 3.00 KiB (1%) | 136 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.363 μs (50%) | 0.000 ns | 1008 bytes (1%) | 51 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.848 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 12.713 ms (50%) | 0.000 ns | 7.71 MiB (1%) | 503491 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 86.646 ms (50%) | 12.102 ms | 26.82 MiB (1%) | 1255000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 10.533 ms (50%) | 0.000 ns | 7.71 MiB (1%) | 503500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 90.977 ms (50%) | 12.134 ms | 26.82 MiB (1%) | 1255000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 8.326 μs (50%) | 0.000 ns | 2.75 KiB (1%) | 120 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 2.251 μs (50%) | 0.000 ns | 816 bytes (1%) | 39 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 11.042 ms (50%) | 0.000 ns | 7.71 MiB (1%) | 503500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 12.046 ms (50%) | 0.000 ns | 7.68 MiB (1%) | 501495 |
| `["array", "index", "(\"sum\", \"3darray\")"]` | 148.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 1.399 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.008 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"1.0:1.0:100000.0\")"]` | 269.462 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"100000:-1:1\")"]` | 51.304 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"1:100000\")"]` | 102.576 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"Array{Float32,2}\")"]` | 265.326 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"Array{Float64,3}\")"]` | 1.856 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"Array{Int32,2}\")"]` | 290.443 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 265.353 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 290.476 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 265.400 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 290.495 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 265.305 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 290.536 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BitArray{2}\")"]` | 769.355 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 290.417 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 300.284 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 293.984 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.450 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.764 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 265.429 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 297.769 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.422 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 302.278 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 361.363 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 336.893 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.616 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.012 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 290.385 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 323.466 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.018 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"1.0:1.0:100000.0\")"]` | 270.468 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"100000:-1:1\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"1:100000\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float32,2}\")"]` | 23.154 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float64,3}\")"]` | 1.044 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Int32,2}\")"]` | 20.690 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 23.188 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 20.725 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 23.359 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 20.943 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 23.345 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 20.922 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BitArray{2}\")"]` | 826.383 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 23.437 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 32.786 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.380 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.560 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.422 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 23.748 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 191.645 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 788.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 20.970 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 21.202 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 111.789 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.165 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.510 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 21.281 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 111.843 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon\", \"1.0:0.00010001000100010001:2.0\")"]` | 24.973 μs (50%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"1.0:1.0:100000.0\")"]` | 247.704 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"100000:-1:1\")"]` | 65.102 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"1:100000\")"]` | 54.730 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"Array{Float32,2}\")"]` | 195.875 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"Array{Int32,2}\")"]` | 195.702 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 195.955 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 194.856 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 200.294 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 199.588 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 194.965 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 195.580 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BitArray{2}\")"]` | 31.159 μs (50%) | 0.000 ns | 85.94 KiB (1%) | 1000 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 235.498 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 196.578 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 331.027 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 16.046 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 22.731 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 195.667 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 262.275 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 234.630 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 195.904 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 330.628 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 15.596 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 22.585 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 195.772 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 264.568 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumcolon_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 23.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"1.0:1.0:100000.0\")"]` | 23.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"100000:-1:1\")"]` | 57.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"1:100000\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"Array{Float32,2}\")"]` | 3.084 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"Array{Int32,2}\")"]` | 3.046 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 3.111 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 3.057 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 3.102 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 3.132 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 3.084 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 3.072 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BitArray{2}\")"]` | 3.582 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.129 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.044 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 4.002 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.195 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.706 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.140 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.862 μs (50%) | 0.000 ns | 31.19 KiB (1%) | 499 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.119 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.038 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.963 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.233 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 5.924 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.084 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.842 μs (50%) | 0.000 ns | 31.19 KiB (1%) | 499 |
| `["array", "index", "(\"sumeach\", \"1.0:0.00010001000100010001:2.0\")"]` | 26.854 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"1.0:1.0:100000.0\")"]` | 269.295 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"100000:-1:1\")"]` | 24.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"1:100000\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"Array{Float32,2}\")"]` | 192.335 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"Array{Float64,3}\")"]` | 1.032 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"Array{Int32,2}\")"]` | 20.000 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.337 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 20.034 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 265.261 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 290.506 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 265.286 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 290.545 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BitArray{2}\")"]` | 512.901 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.344 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 300.260 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.345 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.552 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.019 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 265.435 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 286.581 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.375 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 20.031 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 320.010 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 95.390 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 102.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.004 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 290.492 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 323.536 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.044 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"1.0:1.0:100000.0\")"]` | 269.455 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"100000:-1:1\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"1:100000\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"Array{Float32,2}\")"]` | 8.316 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumeach_view\", \"Array{Float64,3}\")"]` | 42.724 μs (50%) | 0.000 ns | 103.98 KiB (1%) | 2662 |
| `["array", "index", "(\"sumeach_view\", \"Array{Int32,2}\")"]` | 8.242 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.339 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 104.406 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 23.349 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 20.974 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 23.376 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 20.915 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 21.350 ms (50%) | 11.999 ms | 26.70 MiB (1%) | 500000 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.481 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 32.777 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 203.083 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.408 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.378 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 23.837 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 191.626 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 788.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 149.951 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 21.263 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 206.597 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.338 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.484 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 21.306 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 112.301 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.014 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"1.0:1.0:100000.0\")"]` | 270.205 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"100000:-1:1\")"]` | 38.493 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"1:100000\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"Array{Float32,2}\")"]` | 192.335 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"Array{Float64,3}\")"]` | 1.032 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"Array{Int32,2}\")"]` | 20.014 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.343 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 101.719 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 293.519 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 321.941 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 293.473 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 322.054 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BitArray{2}\")"]` | 513.011 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 226.784 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 483.608 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 262.195 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.732 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 10.988 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 516.015 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 592.519 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.672 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 217.011 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 485.936 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 268.957 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.748 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 11.052 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 475.982 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 580.037 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"1.0:0.00010001000100010001:2.0\")"]` | 28.216 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"1.0:1.0:100000.0\")"]` | 275.571 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"100000:-1:1\")"]` | 85.500 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"1:100000\")"]` | 85.491 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Float32,2}\")"]` | 192.334 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Float64,3}\")"]` | 1.031 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Int32,2}\")"]` | 19.982 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.343 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 101.639 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.054 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.940 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.054 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.940 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BitArray{2}\")"]` | 769.366 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 226.881 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.149 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 262.384 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.733 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 23.833 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.064 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.131 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 16.579 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 220.259 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.153 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 269.154 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.748 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 24.097 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.065 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.134 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"1.0:0.00010001000100010001:2.0\")"]` | 26.854 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"1.0:1.0:100000.0\")"]` | 269.281 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"100000:-1:1\")"]` | 24.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"1:100000\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"Array{Float32,2}\")"]` | 192.334 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"Array{Float64,3}\")"]` | 1.032 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"Array{Int32,2}\")"]` | 20.013 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.344 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 20.005 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 1.875 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 1.867 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 1.875 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 1.867 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BitArray{2}\")"]` | 512.883 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.342 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.993 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.345 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.559 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 21.521 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.873 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.877 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 16.674 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 20.034 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.001 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 95.786 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 103.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 21.803 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.999 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.057 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.010 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"1.0:1.0:100000.0\")"]` | 269.449 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"100000:-1:1\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"1:100000\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"Array{Float32,2}\")"]` | 8.479 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumlinear_view\", \"Array{Float64,3}\")"]` | 43.427 μs (50%) | 0.000 ns | 103.98 KiB (1%) | 2662 |
| `["array", "index", "(\"sumlinear_view\", \"Array{Int32,2}\")"]` | 8.419 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.340 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 104.403 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 12.957 ms (50%) | 0.000 ns | 11.44 MiB (1%) | 250000 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 13.048 ms (50%) | 0.000 ns | 11.44 MiB (1%) | 250000 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 12.985 ms (50%) | 0.000 ns | 11.44 MiB (1%) | 250000 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 13.053 ms (50%) | 0.000 ns | 11.44 MiB (1%) | 250000 |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 21.031 ms (50%) | 11.951 ms | 26.70 MiB (1%) | 500000 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.746 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 13.319 ms (50%) | 0.000 ns | 11.44 MiB (1%) | 250000 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 203.397 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.410 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 64.161 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 11.043 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 10.044 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 91.339 μs (50%) | 0.000 ns | 78.13 KiB (1%) | 1000 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 149.667 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 13.350 ms (50%) | 0.000 ns | 11.44 MiB (1%) | 250000 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 206.615 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.335 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 63.094 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 11.041 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 10.008 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlogical\", \"1.0:0.00010001000100010001:2.0\")"]` | 13.519 μs (50%) | 0.000 ns | 21.09 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"1.0:1.0:100000.0\")"]` | 132.291 μs (50%) | 0.000 ns | 207.89 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"100000:-1:1\")"]` | 112.814 μs (50%) | 0.000 ns | 207.86 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"1:100000\")"]` | 93.725 μs (50%) | 0.000 ns | 207.86 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 206.763 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 207.458 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 226.385 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 227.280 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 210.597 μs (50%) | 0.000 ns | 328.30 KiB (1%) | 1502 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 221.337 μs (50%) | 0.000 ns | 328.30 KiB (1%) | 1502 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 208.765 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 209.160 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 268.719 μs (50%) | 0.000 ns | 78.30 KiB (1%) | 1502 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 284.022 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 270.999 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 266.181 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 20.545 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 25.285 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 215.513 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 293.602 μs (50%) | 0.000 ns | 319.84 KiB (1%) | 1000 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 287.238 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 272.778 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 276.003 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 20.378 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 24.991 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 216.359 μs (50%) | 0.000 ns | 320.48 KiB (1%) | 1002 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 294.303 μs (50%) | 0.000 ns | 319.84 KiB (1%) | 1000 |
| `["array", "index", "(\"sumlogical_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 10.273 μs (50%) | 0.000 ns | 21.17 KiB (1%) | 8 |
| `["array", "index", "(\"sumlogical_view\", \"1.0:1.0:100000.0\")"]` | 100.600 μs (50%) | 0.000 ns | 207.97 KiB (1%) | 8 |
| `["array", "index", "(\"sumlogical_view\", \"100000:-1:1\")"]` | 100.605 μs (50%) | 0.000 ns | 207.95 KiB (1%) | 8 |
| `["array", "index", "(\"sumlogical_view\", \"1:100000\")"]` | 100.557 μs (50%) | 0.000 ns | 207.94 KiB (1%) | 8 |
| `["array", "index", "(\"sumlogical_view\", \"Array{Float32,2}\")"]` | 218.806 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"Array{Int32,2}\")"]` | 217.903 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 219.598 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 219.160 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 220.628 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 218.659 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 217.804 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 219.112 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"BitArray{2}\")"]` | 223.171 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 222.325 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 200.495 μs (50%) | 0.000 ns | 601.73 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 222.096 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 25.545 μs (50%) | 0.000 ns | 109.50 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 28.737 μs (50%) | 0.000 ns | 109.50 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 219.441 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 223.213 μs (50%) | 0.000 ns | 592.73 KiB (1%) | 2497 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 219.833 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 199.706 μs (50%) | 0.000 ns | 601.73 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 223.052 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 25.325 μs (50%) | 0.000 ns | 109.50 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 28.588 μs (50%) | 0.000 ns | 109.50 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 219.692 μs (50%) | 0.000 ns | 593.92 KiB (1%) | 2502 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 221.649 μs (50%) | 0.000 ns | 592.73 KiB (1%) | 2497 |
| `["array", "index", "(\"sumrange\", \"1.0:0.00010001000100010001:2.0\")"]` | 25.015 μs (50%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"1.0:1.0:100000.0\")"]` | 247.948 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"100000:-1:1\")"]` | 61.557 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"1:100000\")"]` | 62.852 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"Array{Float32,2}\")"]` | 196.579 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"Array{Int32,2}\")"]` | 195.478 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 196.817 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 196.321 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 199.870 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 199.803 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 197.122 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 196.166 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BitArray{2}\")"]` | 30.789 μs (50%) | 0.000 ns | 85.94 KiB (1%) | 1000 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 234.875 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 197.518 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 332.851 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 16.204 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 22.803 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 197.197 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 264.162 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 235.050 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 196.513 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 330.943 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 15.864 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 22.474 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 195.889 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 264.087 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumrange_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 23.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"1.0:1.0:100000.0\")"]` | 23.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"100000:-1:1\")"]` | 57.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"1:100000\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"Array{Float32,2}\")"]` | 3.872 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"Array{Int32,2}\")"]` | 3.870 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 3.849 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 3.866 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 3.822 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 3.843 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 3.853 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 3.865 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 3.965 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.863 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.013 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.991 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.913 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.938 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.899 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.918 μs (50%) | 0.000 ns | 31.19 KiB (1%) | 499 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.854 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 3.996 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.942 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.881 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.181 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.836 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.914 μs (50%) | 0.000 ns | 31.19 KiB (1%) | 499 |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 150.000 ns (50%) | 0.000 ns | 320 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 150.000 ns (50%) | 0.000 ns | 320 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 166.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 141.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector\", \"Array{Float32,2}\")"]` | 23.462 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"Array{Int32,2}\")"]` | 22.863 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 23.519 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 22.885 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 25.954 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 25.462 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 23.458 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 22.900 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BitArray{2}\")"]` | 26.793 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 23.759 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 23.510 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 30.514 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 19.462 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 31.728 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 23.445 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 30.620 μs (50%) | 0.000 ns | 54.70 KiB (1%) | 500 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 23.173 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 23.226 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 29.741 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 18.904 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 31.580 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 22.957 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 30.172 μs (50%) | 0.000 ns | 54.70 KiB (1%) | 500 |
| `["array", "index", "(\"sumvector_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 124.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"1.0:1.0:100000.0\")"]` | 123.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"100000:-1:1\")"]` | 160.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"1:100000\")"]` | 110.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"Array{Float32,2}\")"]` | 10.038 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"Array{Int32,2}\")"]` | 9.665 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 9.653 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 7.370 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 10.799 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 6.557 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 8.558 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 9.897 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 6.226 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 9.411 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 33.074 μs (50%) | 0.000 ns | 117.31 KiB (1%) | 2001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 11.157 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 5.315 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 8.587 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.776 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.906 μs (50%) | 0.000 ns | 39.11 KiB (1%) | 999 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 6.041 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 33.225 μs (50%) | 0.000 ns | 117.31 KiB (1%) | 2001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 6.706 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 5.293 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 8.393 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.793 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 11.647 μs (50%) | 0.000 ns | 39.11 KiB (1%) | 999 |
| `["array", "index", "2d"]` | 58.843 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "3d"]` | 84.151 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "4d"]` | 99.785 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "5d"]` | 152.109 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "6d"]` | 179.375 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "7d"]` | 4.562 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "ind2sub"]` | 1.539 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "sub2ind"]` | 268.757 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norm1\", \"Float64\")"]` | 148.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norm1\", \"Int64\")"]` | 804.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Float64\")"]` | 1.471 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Int64\")"]` | 808.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Float64\")"]` | 781.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 95.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Float64\")"]` | 780.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 97.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"maxabs\", \"Float64\")"]` | 1.676 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"maxabs\", \"Int64\")"]` | 787.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"mean\", \"Float64\")"]` | 114.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"mean\", \"Int64\")"]` | 97.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"norm\", \"Float64\")"]` | 286.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"norm\", \"Int64\")"]` | 1.570 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 109.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 92.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 145.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs2\", \"Int64\")"]` | 292.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 113.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 171.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"var\", \"Float64\")"]` | 294.000 ns (15%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["array", "reductions", "(\"var\", \"Int64\")"]` | 977.000 ns (15%) | 0.000 ns | 176 bytes (1%) | 4 |
| `["array", "reverse", "rev_load_fast!"]` | 876.736 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reverse", "rev_load_slow!"]` | 2.152 ms (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reverse", "rev_loadmul_fast!"]` | 3.097 ms (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reverse", "rev_loadmul_slow!"]` | 3.354 ms (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 833.000 ns (15%) | 0.000 ns | 352 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 830.000 ns (15%) | 0.000 ns | 352 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 838.000 ns (15%) | 0.000 ns | 352 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 834.000 ns (15%) | 0.000 ns | 352 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 817.000 ns (15%) | 0.000 ns | 352 bytes (1%) | 8 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.701 ms (15%) | 0.000 ns | 5.81 MiB (1%) | 1311 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 3.650 s (15%) | 1.980 s | 5.03 GiB (1%) | 17815 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 51.223 ms (15%) | 27.432 ms | 83.54 MiB (1%) | 3411 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 443.769 ms (15%) | 255.340 ms | 651.51 MiB (1%) | 6911 |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.396 ms (15%) | 0.000 ns | 2.80 MiB (1%) | 1156 |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 2.298 s (15%) | 982.716 ms | 2.50 GiB (1%) | 15860 |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 28.446 ms (15%) | 9.149 ms | 41.10 MiB (1%) | 2956 |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 277.883 ms (15%) | 127.819 ms | 323.00 MiB (1%) | 5956 |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 377.074 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 993.361 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 991.407 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 667.819 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.065 ms (15%) | 0.000 ns | 128 bytes (1%) | 4 |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 1.059 ms (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 994.481 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(10, \"tup_tup\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(3, \"tup_tup\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 19.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 19.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 5.443 μs (15%) | 0.000 ns | 23.92 KiB (1%) | 4 |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 10.252 μs (15%) | 0.000 ns | 39.55 KiB (1%) | 4 |
| `["broadcast", "sparse", "((10000000,), 1)"]` | 36.426 μs (15%) | 0.000 ns | 156.69 KiB (1%) | 5 |
| `["broadcast", "sparse", "((10000000,), 2)"]` | 30.394 μs (15%) | 0.000 ns | 313.19 KiB (1%) | 5 |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 50.000 ns (15%) | 0.000 ns | 160 bytes (1%) | 1 |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 44.000 ns (15%) | 0.000 ns | 112 bytes (1%) | 1 |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 46.000 ns (15%) | 0.000 ns | 128 bytes (1%) | 1 |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "day"]` | 13.516 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "hour"]` | 4.126 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "millisecond"]` | 2.069 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "minute"]` | 4.123 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "month"]` | 10.704 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "second"]` | 4.126 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "year"]` | 9.668 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 14.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Hour\")"]` | 14.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Millisecond\")"]` | 14.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Minute\")"]` | 14.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Month\")"]` | 71.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "arithmetic", "(\"DateTime\", \"Second\")"]` | 14.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Year\")"]` | 61.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 14.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 54.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "arithmetic", "(\"Date\", \"Year\")"]` | 47.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "construction", "Date"]` | 12.877 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "construction", "DateTime"]` | 15.104 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "conversion", "Date -> DateTime"]` | 1.296 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "conversion", "DateTime -> Date"]` | 2.066 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 27.053 μs (15%) | 0.000 ns | 7.69 KiB (1%) | 177 |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 84.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 266.000 ns (15%) | 0.000 ns | 224 bytes (1%) | 7 |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 390.000 ns (15%) | 0.000 ns | 480 bytes (1%) | 12 |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 266.000 ns (15%) | 0.000 ns | 224 bytes (1%) | 7 |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 18.555 μs (15%) | 0.000 ns | 3.78 KiB (1%) | 87 |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 62.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "parse", "Date"]` | 42.389 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "parse", "DateTime"]` | 54.363 ns (15%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["dates", "query", "(\"dayofweek\", \"DateTime\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofweek\", \"Date\")"]` | 17.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofweekofmonth\", \"Date\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofyear\", \"DateTime\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofyear\", \"Date\")"]` | 31.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"daysofweekinmonth\", \"DateTime\")"]` | 42.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"daysofweekinmonth\", \"Date\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofmonth\", \"DateTime\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofmonth\", \"Date\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofweek\", \"DateTime\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofweek\", \"Date\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"isleapyear\", \"DateTime\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"isleapyear\", \"Date\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofmonth\", \"DateTime\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofmonth\", \"Date\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofweek\", \"DateTime\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofweek\", \"Date\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "string", "Date"]` | 223.236 ns (15%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["dates", "string", "DateTime"]` | 543.732 ns (15%) | 0.000 ns | 1.02 KiB (1%) | 19 |
| `["io", "read", "read"]` | 7.705 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["io", "read", "readstring"]` | 30.144 ns (15%) | 0.000 ns | 96 bytes (1%) | 2 |
| `["io", "serialization", "(\"deserialize\", \"Matrix{Float64}\")"]` | 652.891 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 25 |
| `["io", "serialization", "(\"deserialize\", \"Vector{String}\")"]` | 117.560 μs (15%) | 0.000 ns | 122.34 KiB (1%) | 2995 |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 3.974 ms (15%) | 0.000 ns | 7.63 MiB (1%) | 12 |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 56.067 μs (15%) | 0.000 ns | 71.64 KiB (1%) | 22 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 58.053 ms (45%) | 8.910 ms | 24.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 917.029 μs (45%) | 0.000 ns | 1.50 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Vector\", 1024)"]` | 1.041 ms (45%) | 0.000 ns | 8.01 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Vector\", 256)"]` | 54.713 μs (45%) | 0.000 ns | 514.20 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 1024)"]` | 764.000 ns (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 296.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 1024)"]` | 842.000 ns (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 280.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 28.826 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 673.193 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"Vector\", 1024)"]` | 123.766 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"Vector\", 256)"]` | 9.227 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Matrix\", 1024)"]` | 47.664 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Matrix\", 256)"]` | 828.067 μs (45%) | 0.000 ns | 512.08 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Vector\", 1024)"]` | 225.597 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Vector\", 256)"]` | 11.846 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 58.330 ms (45%) | 8.889 ms | 24.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 915.473 μs (45%) | 0.000 ns | 1.50 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"Vector\", 1024)"]` | 1.344 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"Vector\", 256)"]` | 484.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 57.967 ms (45%) | 8.630 ms | 24.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 916.811 μs (45%) | 0.000 ns | 1.50 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 1024)"]` | 3.828 μs (45%) | 0.000 ns | 32.50 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 256)"]` | 1.704 μs (45%) | 0.000 ns | 8.50 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 28.878 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 674.514 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"Vector\", 1024)"]` | 124.738 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"Vector\", 256)"]` | 8.863 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.665 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 728.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 804.000 ns (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 283.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.131 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 49.196 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 1024)"]` | 1.141 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 256)"]` | 47.820 μs (45%) | 0.000 ns | 512.08 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.774 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 723.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 2.779 μs (45%) | 0.000 ns | 24.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.237 μs (45%) | 0.000 ns | 6.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.138 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 49.282 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 771.000 ns (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 303.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.651 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 697.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 773.000 ns (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 285.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.162 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 48.540 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 1024)"]` | 1.141 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 256)"]` | 50.467 μs (45%) | 0.000 ns | 512.08 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.772 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 698.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 2.661 μs (45%) | 0.000 ns | 24.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.228 μs (45%) | 0.000 ns | 6.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.164 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 49.168 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 743.000 ns (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 288.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 1024)"]` | 2.065 μs (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 644.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"/\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 32.835 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"/\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 906.951 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 1024)"]` | 105.880 ms (45%) | 8.262 ms | 40.01 MiB (1%) | 12 |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 256)"]` | 2.522 ms (45%) | 0.000 ns | 2.50 MiB (1%) | 12 |
| `["linalg", "arithmetic", "(\"/\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 27.766 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"/\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 650.972 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"A_mul_B!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 1024)"]` | 851.308 ms (45%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["linalg", "arithmetic", "(\"A_mul_B!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 256)"]` | 12.142 ms (45%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Bidiagonal\", \"Vector\", 1024)"]` | 8.476 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Bidiagonal\", \"Vector\", 256)"]` | 2.257 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 1024)"]` | 2.093 μs (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 663.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 1024)"]` | 2.099 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 677.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 1024)"]` | 635.753 μs (45%) | 0.000 ns | 600.97 KiB (1%) | 73 |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 256)"]` | 150.879 μs (45%) | 0.000 ns | 150.17 KiB (1%) | 73 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 31.879 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 836.377 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"Vector\", 1024)"]` | 561.554 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"Vector\", 256)"]` | 32.629 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Matrix\", 1024)"]` | 87.060 ms (45%) | 0.000 ns | 16.01 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Matrix\", 256)"]` | 2.246 ms (45%) | 0.000 ns | 1.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Vector\", 1024)"]` | 24.784 ms (45%) | 0.000 ns | 8.02 MiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Vector\", 256)"]` | 678.299 μs (45%) | 0.000 ns | 516.36 KiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"SymTridiagonal\", \"Vector\", 1024)"]` | 17.050 μs (45%) | 0.000 ns | 24.42 KiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"SymTridiagonal\", \"Vector\", 256)"]` | 4.783 μs (45%) | 0.000 ns | 6.42 KiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Tridiagonal\", \"Vector\", 1024)"]` | 26.136 μs (45%) | 0.000 ns | 48.88 KiB (1%) | 9 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Tridiagonal\", \"Vector\", 256)"]` | 7.592 μs (45%) | 0.000 ns | 12.88 KiB (1%) | 9 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 32.068 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 844.387 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"Vector\", 1024)"]` | 537.519 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"Vector\", 256)"]` | 31.754 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 1024)"]` | 1.079 μs (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 256)"]` | 282.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 1024)"]` | 1.061 μs (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 256)"]` | 282.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 1024)"]` | 403.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 256)"]` | 124.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 1024)"]` | 416.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 256)"]` | 136.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"exp\", \"Hermitian\", 1024)"]` | 990.906 ms (45%) | 27.697 ms | 80.82 MiB (1%) | 23 |
| `["linalg", "arithmetic", "(\"exp\", \"Hermitian\", 256)"]` | 20.965 ms (45%) | 0.000 ns | 5.21 MiB (1%) | 23 |
| `["linalg", "arithmetic", "(\"log\", \"Hermitian\", 1024)"]` | 975.115 ms (45%) | 18.528 ms | 80.85 MiB (1%) | 23 |
| `["linalg", "arithmetic", "(\"log\", \"Hermitian\", 256)"]` | 20.977 ms (45%) | 0.000 ns | 5.21 MiB (1%) | 23 |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 243.283 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 256)"]` | 3.724 ms (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"Hermitian\", 1024)"]` | 977.173 ms (45%) | 18.611 ms | 80.85 MiB (1%) | 23 |
| `["linalg", "arithmetic", "(\"sqrt\", \"Hermitian\", 256)"]` | 20.969 ms (45%) | 0.000 ns | 5.21 MiB (1%) | 23 |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.085 s (45%) | 0.000 ns | 16.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 256)"]` | 8.997 ms (45%) | 0.000 ns | 1.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 244.244 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 256)"]` | 3.843 ms (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "blas", "asum"]` | 132.872 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "axpy!"]` | 202.279 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "blascopy!"]` | 137.397 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "dot"]` | 98.195 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "dotc"]` | 235.187 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "dotu"]` | 234.509 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gbmv!"]` | 177.819 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gbmv"]` | 180.115 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "gemm!"]` | 47.448 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gemm"]` | 47.759 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "gemv!"]` | 226.584 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gemv"]` | 214.751 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "ger!"]` | 681.936 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "her!"]` | 1.928 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "herk!"]` | 113.572 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "herk"]` | 112.860 ms (40%) | 0.000 ns | 16.00 MiB (1%) | 2 |
| `["linalg", "blas", "nrm2"]` | 270.153 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "sbmv!"]` | 189.748 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "sbmv"]` | 193.264 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "scal!"]` | 209.880 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "scal"]` | 984.200 ns (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "symm!"]` | 47.520 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "symm"]` | 48.003 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "symv!"]` | 111.804 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "symv"]` | 112.075 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "syr!"]` | 508.968 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "syrk!"]` | 28.661 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "syrk"]` | 28.687 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "trmm!"]` | 28.035 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trmm"]` | 29.044 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "trmv!"]` | 112.244 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trmv"]` | 109.483 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "trsm!"]` | 31.150 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trsm"]` | 32.197 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "trsv!"]` | 112.866 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trsv"]` | 110.886 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "factorization", "(\"chol\", \"Matrix\", 1024)"]` | 15.978 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 5 |
| `["linalg", "factorization", "(\"chol\", \"Matrix\", 256)"]` | 449.102 μs (45%) | 0.000 ns | 512.16 KiB (1%) | 5 |
| `["linalg", "factorization", "(\"cholfact\", \"Matrix\", 1024)"]` | 15.981 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 6 |
| `["linalg", "factorization", "(\"cholfact\", \"Matrix\", 256)"]` | 448.945 μs (45%) | 0.000 ns | 512.19 KiB (1%) | 6 |
| `["linalg", "factorization", "(\"eig\", \"Bidiagonal\", 1024)"]` | 5.302 ms (45%) | 0.000 ns | 8.01 MiB (1%) | 61 |
| `["linalg", "factorization", "(\"eig\", \"Bidiagonal\", 256)"]` | 340.579 μs (45%) | 0.000 ns | 516.20 KiB (1%) | 59 |
| `["linalg", "factorization", "(\"eig\", \"Diagonal\", 1024)"]` | 711.356 μs (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "factorization", "(\"eig\", \"Diagonal\", 256)"]` | 38.455 μs (45%) | 0.000 ns | 512.11 KiB (1%) | 3 |
| `["linalg", "factorization", "(\"eig\", \"LowerTriangular\", 1024)"]` | 77.884 ms (45%) | 9.076 ms | 32.03 MiB (1%) | 17 |
| `["linalg", "factorization", "(\"eig\", \"LowerTriangular\", 256)"]` | 2.264 ms (45%) | 0.000 ns | 2.01 MiB (1%) | 16 |
| `["linalg", "factorization", "(\"eig\", \"Matrix\", 1024)"]` | 1.380 s (45%) | 9.132 ms | 33.07 MiB (1%) | 56 |
| `["linalg", "factorization", "(\"eig\", \"Matrix\", 256)"]` | 51.153 ms (45%) | 0.000 ns | 2.27 MiB (1%) | 50 |
| `["linalg", "factorization", "(\"eig\", \"SymTridiagonal\", 1024)"]` | 107.230 ms (45%) | 0.000 ns | 8.27 MiB (1%) | 38 |
| `["linalg", "factorization", "(\"eig\", \"SymTridiagonal\", 256)"]` | 5.629 ms (45%) | 0.000 ns | 581.88 KiB (1%) | 33 |
| `["linalg", "factorization", "(\"eig\", \"UpperTriangular\", 1024)"]` | 69.098 ms (45%) | 9.091 ms | 24.03 MiB (1%) | 15 |
| `["linalg", "factorization", "(\"eig\", \"UpperTriangular\", 256)"]` | 1.923 ms (45%) | 0.000 ns | 1.51 MiB (1%) | 14 |
| `["linalg", "factorization", "(\"eigfact\", \"Bidiagonal\", 1024)"]` | 5.299 ms (45%) | 0.000 ns | 8.01 MiB (1%) | 61 |
| `["linalg", "factorization", "(\"eigfact\", \"Bidiagonal\", 256)"]` | 340.484 μs (45%) | 0.000 ns | 516.20 KiB (1%) | 59 |
| `["linalg", "factorization", "(\"eigfact\", \"Diagonal\", 1024)"]` | 712.210 μs (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "factorization", "(\"eigfact\", \"Diagonal\", 256)"]` | 42.971 μs (45%) | 0.000 ns | 512.11 KiB (1%) | 3 |
| `["linalg", "factorization", "(\"eigfact\", \"LowerTriangular\", 1024)"]` | 77.614 ms (45%) | 9.088 ms | 32.03 MiB (1%) | 16 |
| `["linalg", "factorization", "(\"eigfact\", \"LowerTriangular\", 256)"]` | 2.264 ms (45%) | 0.000 ns | 2.01 MiB (1%) | 15 |
| `["linalg", "factorization", "(\"eigfact\", \"Matrix\", 1024)"]` | 1.376 s (45%) | 8.997 ms | 33.07 MiB (1%) | 50 |
| `["linalg", "factorization", "(\"eigfact\", \"Matrix\", 256)"]` | 51.197 ms (45%) | 0.000 ns | 2.27 MiB (1%) | 44 |
| `["linalg", "factorization", "(\"eigfact\", \"SymTridiagonal\", 1024)"]` | 107.219 ms (45%) | 0.000 ns | 8.27 MiB (1%) | 37 |
| `["linalg", "factorization", "(\"eigfact\", \"SymTridiagonal\", 256)"]` | 5.633 ms (45%) | 0.000 ns | 581.84 KiB (1%) | 32 |
| `["linalg", "factorization", "(\"eigfact\", \"UpperTriangular\", 1024)"]` | 68.941 ms (45%) | 9.078 ms | 24.03 MiB (1%) | 14 |
| `["linalg", "factorization", "(\"eigfact\", \"UpperTriangular\", 256)"]` | 1.927 ms (45%) | 0.000 ns | 1.51 MiB (1%) | 13 |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 1024)"]` | 36.633 ms (45%) | 9.056 ms | 24.02 MiB (1%) | 10 |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 256)"]` | 810.674 μs (45%) | 0.000 ns | 1.50 MiB (1%) | 10 |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 1024)"]` | 17.144 ms (45%) | 9.156 ms | 24.34 MiB (1%) | 2063 |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 256)"]` | 445.686 μs (45%) | 0.000 ns | 1.58 MiB (1%) | 527 |
| `["linalg", "factorization", "(\"lufact\", \"Matrix\", 1024)"]` | 24.421 ms (45%) | 0.000 ns | 8.01 MiB (1%) | 4 |
| `["linalg", "factorization", "(\"lufact\", \"Matrix\", 256)"]` | 660.092 μs (45%) | 0.000 ns | 514.23 KiB (1%) | 4 |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 1024)"]` | 13.059 μs (45%) | 0.000 ns | 40.75 KiB (1%) | 8 |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 256)"]` | 4.101 μs (45%) | 0.000 ns | 10.75 KiB (1%) | 8 |
| `["linalg", "factorization", "(\"qr\", \"Matrix\", 1024)"]` | 166.502 ms (45%) | 9.338 ms | 32.56 MiB (1%) | 19 |
| `["linalg", "factorization", "(\"qr\", \"Matrix\", 256)"]` | 3.861 ms (45%) | 0.000 ns | 2.14 MiB (1%) | 19 |
| `["linalg", "factorization", "(\"qrfact\", \"Matrix\", 1024)"]` | 63.844 ms (45%) | 0.000 ns | 8.56 MiB (1%) | 8 |
| `["linalg", "factorization", "(\"qrfact\", \"Matrix\", 256)"]` | 1.886 ms (45%) | 0.000 ns | 656.30 KiB (1%) | 8 |
| `["linalg", "factorization", "(\"schur\", \"Matrix\", 1024)"]` | 1.254 s (45%) | 0.000 ns | 16.30 MiB (1%) | 13 |
| `["linalg", "factorization", "(\"schur\", \"Matrix\", 256)"]` | 47.838 ms (45%) | 0.000 ns | 1.08 MiB (1%) | 13 |
| `["linalg", "factorization", "(\"schurfact\", \"Matrix\", 1024)"]` | 1.257 s (45%) | 0.000 ns | 16.30 MiB (1%) | 12 |
| `["linalg", "factorization", "(\"schurfact\", \"Matrix\", 256)"]` | 47.875 ms (45%) | 0.000 ns | 1.08 MiB (1%) | 12 |
| `["linalg", "factorization", "(\"svd\", \"Bidiagonal\", 1024)"]` | 66.656 ms (45%) | 8.082 ms | 48.11 MiB (1%) | 24 |
| `["linalg", "factorization", "(\"svd\", \"Bidiagonal\", 256)"]` | 5.484 ms (45%) | 0.000 ns | 3.03 MiB (1%) | 23 |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 10.409 ms (45%) | 0.000 ns | 858.95 KiB (1%) | 14370 |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 718.333 μs (45%) | 0.000 ns | 208.45 KiB (1%) | 3614 |
| `["linalg", "factorization", "(\"svd\", \"LowerTriangular\", 1024)"]` | 578.124 ms (45%) | 18.336 ms | 64.13 MiB (1%) | 24 |
| `["linalg", "factorization", "(\"svd\", \"LowerTriangular\", 256)"]` | 16.741 ms (45%) | 0.000 ns | 4.03 MiB (1%) | 23 |
| `["linalg", "factorization", "(\"svd\", \"Matrix\", 1024)"]` | 600.673 ms (45%) | 18.048 ms | 56.13 MiB (1%) | 22 |
| `["linalg", "factorization", "(\"svd\", \"Matrix\", 256)"]` | 17.667 ms (45%) | 0.000 ns | 3.53 MiB (1%) | 21 |
| `["linalg", "factorization", "(\"svd\", \"UpperTriangular\", 1024)"]` | 581.461 ms (45%) | 18.314 ms | 64.13 MiB (1%) | 24 |
| `["linalg", "factorization", "(\"svd\", \"UpperTriangular\", 256)"]` | 16.899 ms (45%) | 0.000 ns | 4.03 MiB (1%) | 23 |
| `["linalg", "factorization", "(\"svdfact\", \"Bidiagonal\", 1024)"]` | 61.446 ms (45%) | 8.997 ms | 40.11 MiB (1%) | 18 |
| `["linalg", "factorization", "(\"svdfact\", \"Bidiagonal\", 256)"]` | 5.383 ms (45%) | 0.000 ns | 2.53 MiB (1%) | 17 |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 1024)"]` | 10.437 ms (45%) | 0.000 ns | 883.63 KiB (1%) | 14379 |
| `["linalg", "factorization", "(\"svdfact\", \"Diagonal\", 256)"]` | 719.173 μs (45%) | 0.000 ns | 215.13 KiB (1%) | 3623 |
| `["linalg", "factorization", "(\"svdfact\", \"LowerTriangular\", 1024)"]` | 579.245 ms (45%) | 18.241 ms | 56.13 MiB (1%) | 18 |
| `["linalg", "factorization", "(\"svdfact\", \"LowerTriangular\", 256)"]` | 16.666 ms (45%) | 0.000 ns | 3.53 MiB (1%) | 17 |
| `["linalg", "factorization", "(\"svdfact\", \"Matrix\", 1024)"]` | 592.663 ms (45%) | 18.098 ms | 48.13 MiB (1%) | 16 |
| `["linalg", "factorization", "(\"svdfact\", \"Matrix\", 256)"]` | 17.542 ms (45%) | 0.000 ns | 3.03 MiB (1%) | 15 |
| `["linalg", "factorization", "(\"svdfact\", \"UpperTriangular\", 1024)"]` | 581.482 ms (45%) | 18.174 ms | 56.13 MiB (1%) | 18 |
| `["linalg", "factorization", "(\"svdfact\", \"UpperTriangular\", 256)"]` | 16.772 ms (45%) | 0.000 ns | 3.53 MiB (1%) | 17 |
| `["micro", "fib"]` | 29.339 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["micro", "mandel"]` | 110.407 μs (15%) | 0.000 ns | 4.44 KiB (1%) | 1 |
| `["micro", "parseint"]` | 114.373 μs (15%) | 0.000 ns | 93.75 KiB (1%) | 2000 |
| `["micro", "pisum"]` | 17.941 ms (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["micro", "quicksort"]` | 264.231 μs (15%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["micro", "randmatmul"]` | 54.495 ms (15%) | 8.938 ms | 22.89 MiB (1%) | 6 |
| `["micro", "randmatstat"]` | 8.038 ms (15%) | 0.000 ns | 15.14 MiB (1%) | 13029 |
| `["misc", "afoldl", "Complex{Float64}"]` | 668.172 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "afoldl", "Float64"]` | 334.676 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "afoldl", "Int"]` | 306.996 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "julia", "(\"macroexpand\", \"evalpoly\")"]` | 108.300 μs (15%) | 0.000 ns | 14.20 KiB (1%) | 145 |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 1.505 ms (15%) | 0.000 ns | 30.58 KiB (1%) | 381 |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 310.624 μs (15%) | 0.000 ns | 17.64 KiB (1%) | 210 |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 2.414 ms (15%) | 0.000 ns | 43.73 KiB (1%) | 579 |
| `["misc", "parse", "DateTime"]` | 10.950 μs (15%) | 0.000 ns | 6.25 KiB (1%) | 200 |
| `["misc", "parse", "Float64"]` | 36.180 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "parse", "Int"]` | 32.474 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "repeat", "(200, 1, 24)"]` | 10.512 μs (15%) | 0.000 ns | 39.63 KiB (1%) | 60 |
| `["misc", "repeat", "(200, 24, 1)"]` | 16.400 μs (15%) | 0.000 ns | 50.50 KiB (1%) | 410 |
| `["misc", "splatting", "(3, 3, 3)"]` | 25.148 μs (15%) | 0.000 ns | 6.25 KiB (1%) | 300 |
| `["nullable", "basic", "(\"get1\", \"Nullable{BigFloat}(1.0)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get1\", \"Nullable{BigInt}(1)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get1\", \"Nullable{Bool}(true)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get1\", \"Nullable{Float32}(1.0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get1\", \"Nullable{Float64}(1.0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get1\", \"Nullable{Int64}(1)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get1\", \"Nullable{Int8}(1)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{BigFloat}()\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{BigFloat}(1.0)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{BigInt}()\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{BigInt}(1)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Bool}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Bool}(true)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Float32}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Float32}(1.0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Float64}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Float64}(1.0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Int64}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Int64}(1)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Int8}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"get2\", \"Nullable{Int8}(1)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigFloat}()\", \"Nullable{BigFloat}()\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigFloat}()\", \"Nullable{BigFloat}(0.0)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigFloat}()\", \"Nullable{BigFloat}(1.0)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigFloat}(1.0)\", \"Nullable{BigFloat}()\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigFloat}(1.0)\", \"Nullable{BigFloat}(0.0)\")"]` | 23.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigFloat}(1.0)\", \"Nullable{BigFloat}(1.0)\")"]` | 28.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigInt}()\", \"Nullable{BigInt}()\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigInt}()\", \"Nullable{BigInt}(0)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigInt}()\", \"Nullable{BigInt}(1)\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigInt}(1)\", \"Nullable{BigInt}()\")"]` | 15.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigInt}(1)\", \"Nullable{BigInt}(0)\")"]` | 16.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{BigInt}(1)\", \"Nullable{BigInt}(1)\")"]` | 18.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Bool}()\", \"Nullable{Bool}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Bool}()\", \"Nullable{Bool}(false)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Bool}()\", \"Nullable{Bool}(true)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Bool}(true)\", \"Nullable{Bool}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Bool}(true)\", \"Nullable{Bool}(false)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Bool}(true)\", \"Nullable{Bool}(true)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float32}()\", \"Nullable{Float32}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float32}()\", \"Nullable{Float32}(0.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float32}()\", \"Nullable{Float32}(1.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float32}(1.0)\", \"Nullable{Float32}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float32}(1.0)\", \"Nullable{Float32}(0.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float32}(1.0)\", \"Nullable{Float32}(1.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float64}()\", \"Nullable{Float64}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float64}()\", \"Nullable{Float64}(0.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float64}()\", \"Nullable{Float64}(1.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float64}(1.0)\", \"Nullable{Float64}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float64}(1.0)\", \"Nullable{Float64}(0.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Float64}(1.0)\", \"Nullable{Float64}(1.0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int64}()\", \"Nullable{Int64}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int64}()\", \"Nullable{Int64}(0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int64}()\", \"Nullable{Int64}(1)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int64}(1)\", \"Nullable{Int64}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int64}(1)\", \"Nullable{Int64}(0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int64}(1)\", \"Nullable{Int64}(1)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int8}()\", \"Nullable{Int8}()\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int8}()\", \"Nullable{Int8}(0)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int8}()\", \"Nullable{Int8}(1)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int8}(1)\", \"Nullable{Int8}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int8}(1)\", \"Nullable{Int8}(0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isequal\", \"Nullable{Int8}(1)\", \"Nullable{Int8}(1)\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{BigFloat}()\")"]` | 14.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{BigFloat}(1.0)\")"]` | 14.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{BigInt}()\")"]` | 14.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{BigInt}(1)\")"]` | 14.000 ns (60%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Bool}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Bool}(true)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Float32}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Float32}(1.0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Float64}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Float64}(1.0)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Int64}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Int64}(1)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Int8}()\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "basic", "(\"isnull\", \"Nullable{Int8}(1)\")"]` | 14.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_all\", \"Array\")"]` | 534.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_all\", \"NullableArray\")"]` | 1.050 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_any\", \"Array\")"]` | 885.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_any\", \"NullableArray\")"]` | 1.348 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"BigFloat\")"]` | 3.900 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"BigInt\")"]` | 2.502 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"Bool\")"]` | 1.052 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"Complex{Float64}\")"]` | 3.322 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"Float32\")"]` | 1.805 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"Float64\")"]` | 2.172 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"Int64\")"]` | 1.362 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"Array\", \"Int8\")"]` | 1.310 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"BigFloat\")"]` | 12.072 μs (50%) | 0.000 ns | 62.50 KiB (1%) | 2000 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"BigInt\")"]` | 10.966 μs (50%) | 0.000 ns | 62.50 KiB (1%) | 2000 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"Bool\")"]` | 2.297 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"Complex{Float64}\")"]` | 4.128 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"Float32\")"]` | 3.006 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"Float64\")"]` | 2.798 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"Int64\")"]` | 2.416 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countequals\", \"NullableArray\", \"Int8\")"]` | 2.333 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"BigFloat\")"]` | 900.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"BigInt\")"]` | 896.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"Bool\")"]` | 449.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"Complex{Float64}\")"]` | 604.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"Float32\")"]` | 454.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"Float64\")"]` | 547.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"Int64\")"]` | 542.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"Array\", \"Int8\")"]` | 450.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"BigFloat\")"]` | 5.229 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 1000 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"BigInt\")"]` | 5.155 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 1000 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"Bool\")"]` | 788.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"Complex{Float64}\")"]` | 787.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"Float32\")"]` | 787.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"Float64\")"]` | 791.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"Int64\")"]` | 788.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_countnulls\", \"NullableArray\", \"Int8\")"]` | 787.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"BigFloat\")"]` | 94.587 μs (50%) | 0.000 ns | 172.13 KiB (1%) | 4006 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"BigInt\")"]` | 121.378 μs (50%) | 0.000 ns | 98.95 KiB (1%) | 5000 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"Bool\")"]` | 538.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"Complex{Float64}\")"]` | 1.254 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"Float32\")"]` | 1.235 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"Float64\")"]` | 1.135 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"Int64\")"]` | 630.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"Array\", \"Int8\")"]` | 1.241 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"BigFloat\")"]` | 102.275 μs (50%) | 0.000 ns | 203.38 KiB (1%) | 5006 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"BigInt\")"]` | 126.086 μs (50%) | 0.000 ns | 130.20 KiB (1%) | 6000 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"Bool\")"]` | 1.191 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"Complex{Float64}\")"]` | 1.450 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"Float32\")"]` | 1.377 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"Float64\")"]` | 1.373 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"Int64\")"]` | 1.065 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["nullable", "nullablearray", "(\"perf_sum\", \"NullableArray\", \"Int8\")"]` | 1.260 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 64.751 μs (15%) | 0.000 ns | 4.44 KiB (1%) | 66 |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 63.041 μs (15%) | 0.000 ns | 2.28 KiB (1%) | 62 |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 70.506 μs (15%) | 0.000 ns | 10.53 KiB (1%) | 66 |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 64.224 μs (15%) | 0.000 ns | 3.38 KiB (1%) | 66 |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 63.589 μs (15%) | 0.000 ns | 2.44 KiB (1%) | 64 |
| `["problem", "chaosgame", "chaosgame"]` | 95.614 ms (15%) | 0.000 ns | 512.19 KiB (1%) | 4 |
| `["problem", "fem", "sparse_fem"]` | 238.754 ms (15%) | 27.434 ms | 119.05 MiB (1%) | 415 |
| `["problem", "go", "go_game"]` | 665.700 ms (15%) | 187.024 ms | 386.84 MiB (1%) | 2932663 |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.645 s (15%) | 913.135 ms | 2.02 GiB (1%) | 1701249 |
| `["problem", "imdb", "centrality"]` | 732.099 ms (15%) | 75.842 ms | 120.04 MiB (1%) | 3730060 |
| `["problem", "json", "parse_json"]` | 1.808 ms (15%) | 0.000 ns | 479.48 KiB (1%) | 12196 |
| `["problem", "laplacian", "laplace_iter_devec"]` | 8.499 ms (15%) | 0.000 ns | 64.16 KiB (1%) | 4 |
| `["problem", "laplacian", "laplace_iter_sub"]` | 20.754 ms (15%) | 0.000 ns | 32.27 KiB (1%) | 5 |
| `["problem", "laplacian", "laplace_iter_vec"]` | 65.730 ms (15%) | 46.034 ms | 120.59 MiB (1%) | 8194 |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 28.511 ms (15%) | 9.540 ms | 24.89 MiB (1%) | 100300 |
| `["problem", "monte carlo", "euro_option_devec"]` | 27.544 ms (15%) | 0.000 ns | 156.41 KiB (1%) | 4 |
| `["problem", "monte carlo", "euro_option_vec"]` | 29.391 ms (15%) | 0.000 ns | 234.61 KiB (1%) | 6 |
| `["problem", "raytrace", "raytrace"]` | 1.253 s (15%) | 101.928 ms | 198.96 MiB (1%) | 3842142 |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 590.240 μs (15%) | 0.000 ns | 938.13 KiB (1%) | 14 |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.083 ms (15%) | 0.000 ns | 1.83 MiB (1%) | 12 |
| `["problem", "simplex", "simplex"]` | 22.958 ms (15%) | 0.000 ns | 251.02 KiB (1%) | 11 |
| `["problem", "spellcheck", "spellcheck"]` | 5.956 s (15%) | 1.352 s | 2.50 GiB (1%) | 54475519 |
| `["problem", "stockcorr", "stockcorr"]` | 513.128 ms (15%) | 336.135 ms | 231.32 MiB (1%) | 20013 |
| `["problem", "ziggurat", "ziggurat"]` | 7.105 s (15%) | 3.066 s | 6.62 GiB (1%) | 10000002 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"'a':'z'\")"]` | 13.519 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 73.871 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large IntSet\")"]` | 26.221 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 74.044 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large String\")"]` | 14.170 μs (25%) | 0.000 ns | 3.73 KiB (1%) | 3 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Vector\")"]` | 12.140 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 83.288 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small IntSet\")"]` | 263.069 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 84.416 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small String\")"]` | 12.479 μs (25%) | 0.000 ns | 144 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Vector\")"]` | 12.372 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"'a':'z'\")"]` | 13.105 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 74.462 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large IntSet\")"]` | 26.007 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 73.931 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large String\")"]` | 14.164 μs (25%) | 0.000 ns | 3.73 KiB (1%) | 3 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Vector\")"]` | 12.145 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 83.190 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small IntSet\")"]` | 261.046 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 83.965 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small String\")"]` | 12.469 μs (25%) | 0.000 ns | 144 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Vector\")"]` | 12.372 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"'a':'z'\")"]` | 17.823 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Dict\")"]` | 94.323 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large IntSet\")"]` | 31.149 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 94.710 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large String\")"]` | 19.476 μs (25%) | 0.000 ns | 3.73 KiB (1%) | 3 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Vector\")"]` | 17.085 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Dict\")"]` | 105.640 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small IntSet\")"]` | 360.796 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 104.733 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small String\")"]` | 17.100 μs (25%) | 0.000 ns | 144 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Vector\")"]` | 16.983 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"'a':'z'\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 52.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large IntSet\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 42.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large String\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Vector\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 48.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small IntSet\")"]` | 42.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 50.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small String\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Vector\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 47.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large IntSet\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 45.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Vector\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 46.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small IntSet\")"]` | 42.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 43.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small String\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Vector\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"'a':'z'\")"]` | 53.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 55.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large IntSet\")"]` | 47.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 48.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large String\")"]` | 47.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Vector\")"]` | 46.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 59.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small IntSet\")"]` | 57.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 48.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small String\")"]` | 48.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Vector\")"]` | 46.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\")"]` | 148.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 2 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", 100)"]` | 1.211 μs (25%) | 0.000 ns | 320 bytes (1%) | 2 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 382.000 ns (25%) | 0.000 ns | 432 bytes (1%) | 7 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 2.444 μs (25%) | 0.000 ns | 1.16 KiB (1%) | 8 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\")"]` | 150.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 2 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\", 100)"]` | 1.219 μs (25%) | 0.000 ns | 320 bytes (1%) | 2 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 104.000 ns (25%) | 0.000 ns | 104 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 103.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 101.000 ns (25%) | 0.000 ns | 104 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 96.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:2^10000\")"]` | 282.000 ns (25%) | 0.000 ns | 1.31 KiB (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 104.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 104.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551615\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551616\")"]` | 53.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 42.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 43.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int16\", \"1:1\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int32\", \"1:1\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:1\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967295\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967297\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int8\", \"1:1\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:170141183460469231731687303715884105728\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551615\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551616\")"]` | 47.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt16\", \"1:1\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt32\", \"1:1\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt32\", \"1:4294967295\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:18446744073709551615\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:1\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967295\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967297\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt8\", \"1:1\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 2.751 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 2.760 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand!\", \"RandomDevice\", \"Int\", \"1:1000\")"]` | 4.176 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 176.000 ns (25%) | 0.000 ns | 288 bytes (1%) | 7 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 185.000 ns (25%) | 0.000 ns | 296 bytes (1%) | 7 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 178.000 ns (25%) | 0.000 ns | 288 bytes (1%) | 7 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 158.000 ns (25%) | 0.000 ns | 288 bytes (1%) | 6 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 433.000 ns (25%) | 0.000 ns | 1.50 KiB (1%) | 7 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 177.000 ns (25%) | 0.000 ns | 288 bytes (1%) | 7 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967297)\")"]` | 178.000 ns (25%) | 0.000 ns | 288 bytes (1%) | 7 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Bool\", \"RangeGenerator(true:true)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:1)\")"]` | 31.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 48.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 52.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967295)\")"]` | 53.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967297)\")"]` | 52.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int16\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int32\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:1)\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:4294967295)\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:4294967297)\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int8\", \"RangeGenerator(1:1)\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:1)\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 48.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 52.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967295)\")"]` | 53.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967297)\")"]` | 52.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt16\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt32\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt32\", \"RangeGenerator(1:4294967295)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:1)\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:18446744073709551615)\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967295)\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967297)\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt8\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"RandomDevice\", \"Int\", \"1:1000\")"]` | 43.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "sequences", "(\"randcycle\", \"MersenneTwister\", \"1000\")"]` | 6.058 μs (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["random", "sequences", "(\"randcycle\", \"MersenneTwister\", \"5\")"]` | 56.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 1 |
| `["random", "sequences", "(\"randperm\", \"MersenneTwister\", \"1000\")"]` | 6.110 μs (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["random", "sequences", "(\"randperm\", \"MersenneTwister\", \"5\")"]` | 53.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 1 |
| `["random", "sequences", "(\"randsubseq!\", \"MersenneTwister\", \"0.2\")"]` | 4.394 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "sequences", "(\"randsubseq!\", \"MersenneTwister\", \"0.8\")"]` | 7.431 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "sequences", "(\"shuffle!\", \"MersenneTwister\")"]` | 6.094 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"ImplicitRNG\", \"Float64\")"]` | 760.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"ImplicitRNG\", \"Int64\")"]` | 1.094 μs (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Bool\")"]` | 1.705 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 16.230 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 5.692 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 6.095 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 17.811 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int16}\")"]` | 5.295 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int32}\")"]` | 5.326 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int64}\")"]` | 8.318 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int8}\")"]` | 5.321 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 17.841 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 5.296 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 5.333 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt64}\")"]` | 8.305 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt8}\")"]` | 5.321 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float16\")"]` | 7.691 μs (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 838.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float64\")"]` | 761.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int128\")"]` | 2.335 μs (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int16\")"]` | 221.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int32\")"]` | 664.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int64\")"]` | 1.085 μs (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int8\")"]` | 184.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt128\")"]` | 2.309 μs (25%) | 0.000 ns | 80 bytes (1%) | 1 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt16\")"]` | 222.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt32\")"]` | 664.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt64\")"]` | 1.089 μs (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt8\")"]` | 189.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["random", "types", "(\"rand!\", \"RandomDevice\", \"Float64\")"]` | 8.394 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"RandomDevice\", \"Int64\")"]` | 217.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Float64\")"]` | 66.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Int64\")"]` | 70.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Bool\")"]` | 79.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 97.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 84.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 80.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 88.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int16}\")"]` | 84.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int32}\")"]` | 88.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int64}\")"]` | 82.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int8}\")"]` | 83.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 90.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 81.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 82.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt64}\")"]` | 90.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt8}\")"]` | 88.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float16\")"]` | 89.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float32\")"]` | 80.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float64\")"]` | 82.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int128\")"]` | 84.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int16\")"]` | 81.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int32\")"]` | 84.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int64\")"]` | 83.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int8\")"]` | 84.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt128\")"]` | 86.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt16\")"]` | 84.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt32\")"]` | 79.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt64\")"]` | 80.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt8\")"]` | 80.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Float64\")"]` | 110.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Int64\")"]` | 103.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randexp!\", \"ImplicitRNG\", \"Float64\")"]` | 5.022 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float16\")"]` | 17.101 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float32\")"]` | 4.986 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float64\")"]` | 4.740 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"RandomDevice\", \"Float64\")"]` | 10.924 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"Float64\")"]` | 79.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float16\")"]` | 70.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float32\")"]` | 95.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float64\")"]` | 86.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"Float64\")"]` | 84.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"ImplicitRNG\", \"Float64\")"]` | 5.325 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 73.967 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 10.866 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 10.181 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float16\")"]` | 17.030 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float32\")"]` | 5.309 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float64\")"]` | 5.014 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"RandomDevice\", \"Float64\")"]` | 11.398 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"Float64\")"]` | 85.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 202.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 90.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 129.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float16\")"]` | 118.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float32\")"]` | 72.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float64\")"]` | 60.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"RandomDevice\", \"Float64\")"]` | 96.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["random", "types", "(\"randn\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 105.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 202.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 26.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 39.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"zero\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigFloat\")"]` | 71.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 164.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 82.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 209.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 218.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 219.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 144.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 143.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 171.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 172.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Int64\")"]` | 99.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"UInt64\")"]` | 97.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 164.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigInt\")"]` | 80.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 168.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 84.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 254.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 254.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Int64}\")"]` | 110.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{UInt64}\")"]` | 108.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float32\")"]` | 210.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float64\")"]` | 210.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Int64\")"]` | 69.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"UInt64\")"]` | 70.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 81.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 168.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 122.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 210.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 281.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 282.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 146.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 144.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 177.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 175.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 104.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 103.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 210.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigInt\")"]` | 94.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 210.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 121.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 339.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 339.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 113.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 110.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 252.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 251.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 80.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 80.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 219.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 254.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 282.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 340.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 218.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 254.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 282.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 338.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Int64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 145.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 109.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 146.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 110.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 151.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 110.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 144.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 111.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Float64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 171.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigInt\")"]` | 209.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 175.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 252.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Float32\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 171.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigInt\")"]` | 211.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 175.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 253.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Float64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigFloat\")"]` | 99.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigInt\")"]` | 70.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 104.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigInt}\")"]` | 78.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 98.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 69.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 103.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 80.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigFloat\")"]` | 179.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 201.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 586.000 ns (50%) | 0.000 ns | 800 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 680.000 ns (50%) | 0.000 ns | 976 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 706.000 ns (50%) | 0.000 ns | 976 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 705.000 ns (50%) | 0.000 ns | 976 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 677.000 ns (50%) | 0.000 ns | 976 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 683.000 ns (50%) | 0.000 ns | 976 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 209.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 206.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Int64\")"]` | 59.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"UInt64\")"]` | 58.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigFloat\")"]` | 240.000 ns (50%) | 0.000 ns | 176 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigInt\")"]` | 294.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 719.000 ns (50%) | 0.000 ns | 832 bytes (1%) | 21 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 818.000 ns (50%) | 0.000 ns | 1008 bytes (1%) | 25 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 843.000 ns (50%) | 0.000 ns | 1008 bytes (1%) | 25 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 838.000 ns (50%) | 0.000 ns | 1008 bytes (1%) | 25 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 919.000 ns (50%) | 0.000 ns | 1.06 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 907.000 ns (50%) | 0.000 ns | 1.06 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float32\")"]` | 321.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float64\")"]` | 320.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 120.000 ns (50%) | 0.000 ns | 176 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"UInt64\")"]` | 120.000 ns (50%) | 0.000 ns | 176 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 229.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 323.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 668.000 ns (50%) | 0.000 ns | 1000 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 746.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 764.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 760.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 732.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 743.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 344.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 343.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 107.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 105.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 328.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 438.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 751.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 1.033 μs (50%) | 0.000 ns | 1.05 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 854.000 ns (50%) | 0.000 ns | 1.38 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 856.000 ns (50%) | 0.000 ns | 1.38 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 1.121 μs (50%) | 0.000 ns | 1.20 KiB (1%) | 34 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 1.108 μs (50%) | 0.000 ns | 1.20 KiB (1%) | 34 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 479.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 477.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 206.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 205.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 373.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 473.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 761.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 884.000 ns (50%) | 0.000 ns | 1.38 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 31.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 28.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 28.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Float32\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Float64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Int64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 374.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 459.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 761.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 879.000 ns (50%) | 0.000 ns | 1.38 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 31.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 32.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 40.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Float32\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Float64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Int64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"UInt64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 240.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 375.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 732.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 1.110 μs (50%) | 0.000 ns | 1.20 KiB (1%) | 34 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 27.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 32.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 30.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Float32\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Float64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Int64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"UInt64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 239.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 344.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 729.000 ns (50%) | 0.000 ns | 1.21 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 1.120 μs (50%) | 0.000 ns | 1.20 KiB (1%) | 34 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 28.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 32.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 30.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Float32\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Float64\")"]` | 22.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Int64\")"]` | 19.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"UInt64\")"]` | 20.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 260.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigInt\")"]` | 321.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 738.000 ns (50%) | 0.000 ns | 832 bytes (1%) | 21 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 848.000 ns (50%) | 0.000 ns | 1008 bytes (1%) | 25 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{Float32}\")"]` | 21.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{Float64}\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{Int64}\")"]` | 22.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{UInt64}\")"]` | 22.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Float32\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 259.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigInt\")"]` | 319.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 742.000 ns (50%) | 0.000 ns | 832 bytes (1%) | 21 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 849.000 ns (50%) | 0.000 ns | 1008 bytes (1%) | 25 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{Float32}\")"]` | 27.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{Float64}\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{Int64}\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{UInt64}\")"]` | 28.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Float64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"UInt64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigFloat\")"]` | 187.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigInt\")"]` | 248.000 ns (50%) | 0.000 ns | 176 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 543.000 ns (50%) | 0.000 ns | 800 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 659.000 ns (50%) | 0.000 ns | 976 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Float32}\")"]` | 20.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Float64}\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Int64}\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{UInt64}\")"]` | 28.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"UInt64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigFloat\")"]` | 186.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigInt\")"]` | 248.000 ns (50%) | 0.000 ns | 176 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 540.000 ns (50%) | 0.000 ns | 800 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 639.000 ns (50%) | 0.000 ns | 976 bytes (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Float32}\")"]` | 20.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Float64}\")"]` | 26.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Int64}\")"]` | 29.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{UInt64}\")"]` | 28.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Float64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Int64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"UInt64\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigFloat\")"]` | 103.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 162.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 151.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 265.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 281.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 282.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 106.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 105.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 171.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 171.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Int64\")"]` | 59.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"UInt64\")"]` | 58.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 164.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigInt\")"]` | 80.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 284.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 124.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 382.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 382.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 119.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 112.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float32\")"]` | 242.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float64\")"]` | 241.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Int64\")"]` | 72.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"UInt64\")"]` | 71.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 152.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 285.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 331.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 571.000 ns (50%) | 0.000 ns | 624 bytes (1%) | 17 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 597.000 ns (50%) | 0.000 ns | 624 bytes (1%) | 17 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 598.000 ns (50%) | 0.000 ns | 624 bytes (1%) | 17 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 285.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 280.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 303.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 303.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 107.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 106.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 266.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 124.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 572.000 ns (50%) | 0.000 ns | 624 bytes (1%) | 17 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 302.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 762.000 ns (50%) | 0.000 ns | 1.23 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 760.000 ns (50%) | 0.000 ns | 1.23 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 293.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 327.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 404.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 402.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Int64\")"]` | 113.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"UInt64\")"]` | 135.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 283.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 382.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 600.000 ns (50%) | 0.000 ns | 624 bytes (1%) | 17 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 761.000 ns (50%) | 0.000 ns | 1.23 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Float64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 282.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 383.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 591.000 ns (50%) | 0.000 ns | 624 bytes (1%) | 17 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 748.000 ns (50%) | 0.000 ns | 1.23 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Int64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"UInt64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 107.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigInt\")"]` | 115.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 284.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 293.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Int64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 105.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigInt\")"]` | 106.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 282.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 293.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Float64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Int64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 171.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 241.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 304.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 402.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Float32\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 170.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigInt\")"]` | 242.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 305.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 407.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{Float32}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{UInt64}\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Float64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"UInt64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigFloat\")"]` | 59.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 79.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 107.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 119.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigFloat\")"]` | 58.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 71.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 105.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigInt}\")"]` | 119.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{Float64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"BigInt\")"]` | 71.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"Bool\")"]` | 127.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"Int64\")"]` | 68.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"UInt64\")"]` | 110.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 122.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Bool\")"]` | 90.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Int64\")"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"UInt64\")"]` | 70.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"BigInt\")"]` | 140.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"Bool\")"]` | 86.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"Int64\")"]` | 79.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"UInt64\")"]` | 98.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"BigInt\")"]` | 190.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Bool\")"]` | 169.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Int64\")"]` | 134.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"UInt64\")"]` | 121.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"BigInt\")"]` | 160.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Bool\")"]` | 132.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Int64\")"]` | 71.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"UInt64\")"]` | 119.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigFloat\")"]` | 60.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 139.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 108.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 226.000 ns (50%) | 0.000 ns | 312 bytes (1%) | 8 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 238.000 ns (50%) | 0.000 ns | 312 bytes (1%) | 8 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 240.000 ns (50%) | 0.000 ns | 312 bytes (1%) | 8 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 167.000 ns (50%) | 0.000 ns | 296 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 165.000 ns (50%) | 0.000 ns | 296 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 146.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 147.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Int64\")"]` | 80.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"UInt64\")"]` | 80.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 140.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigInt\")"]` | 81.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 186.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigInt}\")"]` | 123.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 285.000 ns (50%) | 0.000 ns | 472 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 285.000 ns (50%) | 0.000 ns | 472 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Int64}\")"]` | 147.000 ns (50%) | 0.000 ns | 160 bytes (1%) | 8 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{UInt64}\")"]` | 146.000 ns (50%) | 0.000 ns | 160 bytes (1%) | 8 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float32\")"]` | 202.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float64\")"]` | 201.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Int64\")"]` | 67.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"UInt64\")"]` | 70.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 65.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 144.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 107.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 186.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 257.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 258.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 128.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 127.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 158.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 152.000 ns (50%) | 0.000 ns | 136 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 86.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 91.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 184.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigInt\")"]` | 86.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 187.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 125.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 330.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 329.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 110.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 110.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 242.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 242.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 80.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 78.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 200.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 246.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 256.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 329.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 198.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 255.000 ns (50%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 256.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 338.000 ns (50%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Int64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"UInt64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 126.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 90.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 131.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 92.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 126.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 88.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 130.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 91.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Float64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 146.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigInt\")"]` | 200.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 192.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 286.000 ns (50%) | 0.000 ns | 472 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Float32\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 146.000 ns (50%) | 0.000 ns | 104 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigInt\")"]` | 200.000 ns (50%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 199.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 285.000 ns (50%) | 0.000 ns | 472 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Float64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigFloat\")"]` | 82.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 51.000 ns (50%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 127.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigInt}\")"]` | 90.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigFloat\")"]` | 80.000 ns (50%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 51.000 ns (50%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 126.000 ns (50%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 92.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Float64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 105.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float64\")"]` | 217.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float32\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"zero\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float32\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 26.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 21.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 27.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 42.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 42.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float32\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float32\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 43.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float32\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float64\")"]` | 42.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float32\")"]` | 28.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float64\")"]` | 41.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float32\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 43.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float32\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 43.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"zero\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float64\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float64\")"]` | 47.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 47.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float64\")"]` | 48.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 33.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float64\")"]` | 47.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float64\")"]` | 47.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float64\")"]` | 46.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float64\")"]` | 47.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float64\")"]` | 46.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 26.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 56.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 58.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 57.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 59.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 56.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 58.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 56.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 59.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 19.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"BigFloat\")"]` | 70.000 ns (40%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 80.000 ns (40%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 124.000 ns (40%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 120.000 ns (40%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "fastmath", "(\"add\", \"Complex{Float32}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Complex{Float64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Complex{Int64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Complex{UInt64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Float32\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Float64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"UInt64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"BigFloat\")"]` | 177.000 ns (40%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"div\", \"BigInt\")"]` | 294.000 ns (40%) | 0.000 ns | 264 bytes (1%) | 6 |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 631.000 ns (40%) | 0.000 ns | 1000 bytes (1%) | 23 |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 1.046 μs (40%) | 0.000 ns | 1.05 KiB (1%) | 28 |
| `["scalar", "fastmath", "(\"div\", \"Complex{Float32}\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Complex{Float64}\")"]` | 19.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Complex{Int64}\")"]` | 26.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Complex{UInt64}\")"]` | 28.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Float32\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Float64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"UInt64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"BigFloat\")"]` | 98.000 ns (40%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 81.000 ns (40%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 326.000 ns (40%) | 0.000 ns | 560 bytes (1%) | 13 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 301.000 ns (40%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{Float32}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{Float64}\")"]` | 17.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{Int64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{UInt64}\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Float32\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Float64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"UInt64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"BigFloat\")"]` | 61.000 ns (40%) | 0.000 ns | 88 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 72.000 ns (40%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 106.000 ns (40%) | 0.000 ns | 208 bytes (1%) | 5 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigInt}\")"]` | 125.000 ns (40%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{Float32}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{Float64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{Int64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{UInt64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Float32\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Float64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"UInt64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float32\")"]` | 25.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float64\")"]` | 40.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float32\")"]` | 24.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float64\")"]` | 40.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float32\")"]` | 19.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float64\")"]` | 29.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float32\")"]` | 22.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float64\")"]` | 30.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"normal path -> small, k = -1075\", \"Float64\")"]` | 80.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"normal path -> small, k = -150\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"overflow\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"overflow\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"taylor expansion\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"underflow\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"underflow\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"fast path, k = 1\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"fast path, k = 1\", \"Float64\")"]` | 29.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"no agument reduction, k = 9\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"no agument reduction, k = 9\", \"Float64\")"]` | 25.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path -> small, k = -1045\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path -> small, k = -1045\", \"Float64\")"]` | 79.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path, k = 2\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path, k = 2\", \"Float64\")"]` | 40.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"overflow\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"overflow\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"small argument path\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"small argument path\", \"Float64\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"underflow\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"underflow\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"norm\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"norm\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"subnorm\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"subnorm\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"inf\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"inf\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"norm\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"norm\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"subnorm\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"subnorm\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"inf -> inf\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"inf -> inf\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> inf\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> inf\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> norm\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> norm\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> subnorm\", \"Float32\")"]` | 52.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> subnorm\", \"Float64\")"]` | 53.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> norm\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> norm\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> subnorm\", \"Float32\")"]` | 53.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> subnorm\", \"Float64\")"]` | 54.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"norm\", \"Float32\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"norm\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"subnorm\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"subnorm\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"+\")"]` | 738.000 ns (40%) | 0.000 ns | 656 bytes (1%) | 18 |
| `["scalar", "intfuncs", "(\"nextpow2\", \"BigInt\", \"-\")"]` | 738.000 ns (40%) | 0.000 ns | 656 bytes (1%) | 18 |
| `["scalar", "intfuncs", "(\"nextpow2\", \"Int64\", \"+\")"]` | 67.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"nextpow2\", \"Int64\", \"-\")"]` | 68.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"nextpow2\", \"UInt64\", \"+\")"]` | 60.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"nextpow2\", \"UInt64\", \"-\")"]` | 61.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"+\")"]` | 972.000 ns (40%) | 0.000 ns | 1.19 KiB (1%) | 30 |
| `["scalar", "intfuncs", "(\"prevpow2\", \"BigInt\", \"-\")"]` | 975.000 ns (40%) | 0.000 ns | 1.19 KiB (1%) | 30 |
| `["scalar", "intfuncs", "(\"prevpow2\", \"Int64\", \"+\")"]` | 53.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"prevpow2\", \"Int64\", \"-\")"]` | 54.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"prevpow2\", \"UInt64\", \"+\")"]` | 51.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"prevpow2\", \"UInt64\", \"-\")"]` | 47.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "iteration", "in"]` | 4.895 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "iteration", "indexed"]` | 4.374 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 21.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 54.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 53.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 23.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"no reduction\", \"zero\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"BigFloat\")"]` | 26.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"BigInt\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{BigFloat}\")"]` | 42.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{BigInt}\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{Float32}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{Float64}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Float32\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Float64\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 103.000 ns (40%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "predicate", "(\"iseven\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"iseven\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"BigFloat\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"BigInt\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{BigFloat}\")"]` | 20.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{BigInt}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{Float32}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{Float64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Float32\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Float64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"BigFloat\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"BigInt\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{BigFloat}\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{BigInt}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{Float32}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{Float64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Float32\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Float64\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"BigFloat\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"BigInt\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 24.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigInt}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{Float32}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{Float64}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Float32\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Float64\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"BigFloat\")"]` | 25.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"BigInt\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"Float32\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"Float64\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"BigFloat\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"BigInt\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{BigFloat}\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{BigInt}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{Float64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Float32\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Float64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 104.000 ns (40%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "predicate", "(\"isodd\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isodd\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 19.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 52.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 52.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 27.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 27.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 21.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 21.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 29.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 59.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 55.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 58.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 58.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 58.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 56.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 58.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 58.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 19.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 19.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\")"]` | 25.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\")"]` | 26.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 30.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 32.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 21.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 44.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\")"]` | 65.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 65.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\")"]` | 64.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 65.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 27.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 26.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 26.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 26.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 20.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float32\")"]` | 101.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float64\")"]` | 210.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float32\")"]` | 100.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float64\")"]` | 200.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 100.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float64\")"]` | 205.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float32\")"]` | 99.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float64\")"]` | 208.000 ns (15%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"zero\", \"Float32\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"zero\", \"Float64\")"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["shootout", "binary_trees"]` | 16.556 ms (15%) | 0.000 ns | 11.92 MiB (1%) | 515432 |
| `["shootout", "fannkuch"]` | 117.770 μs (15%) | 0.000 ns | 336 bytes (1%) | 3 |
| `["shootout", "fasta"]` | 11.376 μs (15%) | 0.000 ns | 14.11 KiB (1%) | 806 |
| `["shootout", "k_nucleotide"]` | 28.107 ms (15%) | 0.000 ns | 9.07 MiB (1%) | 254319 |
| `["shootout", "mandelbrot"]` | 3.242 ms (15%) | 0.000 ns | 8.30 KiB (1%) | 41 |
| `["shootout", "meteor_contest"]` | 2.229 s (15%) | 588.311 ms | 1.01 GiB (1%) | 51140675 |
| `["shootout", "nbody"]` | 106.729 μs (15%) | 0.000 ns | 448 bytes (1%) | 6 |
| `["shootout", "nbody_vec"]` | 256.712 μs (15%) | 0.000 ns | 110.86 KiB (1%) | 1017 |
| `["shootout", "pidigits"]` | 32.819 ms (15%) | 20.879 ms | 62.89 MiB (1%) | 98965 |
| `["shootout", "regex_dna"]` | 3.365 ms (15%) | 0.000 ns | 1.70 MiB (1%) | 355 |
| `["shootout", "revcomp"]` | 1.382 ms (25%) | 0.000 ns | 96.13 KiB (1%) | 1233 |
| `["shootout", "spectralnorm"]` | 1.436 ms (15%) | 0.000 ns | 2.63 KiB (1%) | 3 |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 257.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 244.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Float64\", 4095)"]` | 709.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Float64\", 4096)"]` | 692.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int32\", 4095)"]` | 305.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 297.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int64\", 4095)"]` | 1.743 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int64\", 4096)"]` | 1.744 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4095)"]` | 1.805 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4096)"]` | 1.787 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4095)"]` | 3.560 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4096)"]` | 3.548 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 363.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 367.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 698.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 704.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float32\", 4095)"]` | 252.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float32\", 4096)"]` | 210.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float64\", 4095)"]` | 621.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float64\", 4096)"]` | 609.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int32\", 4095)"]` | 298.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int32\", 4096)"]` | 286.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int64\", 4095)"]` | 1.993 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int64\", 4096)"]` | 1.991 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 22.881 μs (20%) | 0.000 ns | 69.52 KiB (1%) | 30 |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 22.847 μs (20%) | 0.000 ns | 69.52 KiB (1%) | 30 |
| `["simd", "(\"local_arrays\", \"Float64\", 4095)"]` | 28.648 μs (20%) | 0.000 ns | 116.91 KiB (1%) | 27 |
| `["simd", "(\"local_arrays\", \"Float64\", 4096)"]` | 28.986 μs (20%) | 0.000 ns | 116.91 KiB (1%) | 27 |
| `["simd", "(\"local_arrays\", \"Int32\", 4095)"]` | 20.389 μs (20%) | 0.000 ns | 69.52 KiB (1%) | 30 |
| `["simd", "(\"local_arrays\", \"Int32\", 4096)"]` | 20.614 μs (20%) | 0.000 ns | 69.52 KiB (1%) | 30 |
| `["simd", "(\"local_arrays\", \"Int64\", 4095)"]` | 29.959 μs (20%) | 0.000 ns | 117.38 KiB (1%) | 33 |
| `["simd", "(\"local_arrays\", \"Int64\", 4096)"]` | 30.074 μs (20%) | 0.000 ns | 117.38 KiB (1%) | 33 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 358.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 342.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 351.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 336.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 876.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 867.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 851.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 848.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 414.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 404.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 428.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 420.000 ns (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.215 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.216 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.201 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.190 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"manual_example!\", \"Float32\", 4095)"]` | 414.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Float32\", 4096)"]` | 395.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Float64\", 4095)"]` | 718.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Float64\", 4096)"]` | 716.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int32\", 4095)"]` | 365.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int32\", 4096)"]` | 359.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int64\", 4095)"]` | 1.278 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int64\", 4096)"]` | 1.272 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float32\", 4095)"]` | 92.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float32\", 4096)"]` | 92.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float64\", 4095)"]` | 112.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float64\", 4096)"]` | 104.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 54.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 54.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int64\", 4095)"]` | 89.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int64\", 4096)"]` | 93.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float32\", 4095)"]` | 490.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float32\", 4096)"]` | 467.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float64\", 4095)"]` | 859.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float64\", 4096)"]` | 838.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int32\", 4095)"]` | 9.529 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int32\", 4096)"]` | 9.533 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int64\", 4095)"]` | 761.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int64\", 4096)"]` | 750.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort forwards\", \"ascending\")"]` | 119.338 μs (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "insertionsort", "(\"sort forwards\", \"descending\")"]` | 580.000 ms (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "insertionsort", "(\"sort forwards\", \"ones\")"]` | 132.752 μs (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "insertionsort", "(\"sort forwards\", \"random\")"]` | 288.734 ms (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "insertionsort", "(\"sort reverse\", \"ascending\")"]` | 579.951 ms (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "insertionsort", "(\"sort reverse\", \"descending\")"]` | 75.516 μs (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "insertionsort", "(\"sort reverse\", \"ones\")"]` | 156.442 μs (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "insertionsort", "(\"sort reverse\", \"random\")"]` | 286.126 ms (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 78.349 μs (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"descending\")"]` | 579.907 ms (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ones\")"]` | 94.214 μs (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"random\")"]` | 288.614 ms (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 579.918 ms (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 33.881 μs (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 114.897 μs (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 286.010 ms (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ascending\")"]` | 171.883 μs (30%) | 0.000 ns | 390.84 KiB (1%) | 6 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"descending\")"]` | 1.762 s (30%) | 0.000 ns | 390.84 KiB (1%) | 6 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ones\")"]` | 214.238 μs (30%) | 0.000 ns | 390.88 KiB (1%) | 8 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"random\")"]` | 1.251 s (30%) | 0.000 ns | 390.88 KiB (1%) | 8 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ascending\")"]` | 1.762 s (30%) | 0.000 ns | 390.95 KiB (1%) | 8 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"descending\")"]` | 125.757 μs (30%) | 0.000 ns | 390.95 KiB (1%) | 8 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ones\")"]` | 236.691 μs (30%) | 0.000 ns | 390.98 KiB (1%) | 10 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"random\")"]` | 1.234 s (30%) | 0.000 ns | 390.98 KiB (1%) | 10 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 99.852 μs (30%) | 0.000 ns | 144 bytes (1%) | 4 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 1.764 s (30%) | 0.000 ns | 144 bytes (1%) | 4 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 187.870 μs (30%) | 0.000 ns | 176 bytes (1%) | 6 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 1.251 s (30%) | 0.000 ns | 176 bytes (1%) | 6 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.763 s (30%) | 0.000 ns | 256 bytes (1%) | 6 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 100.113 μs (30%) | 0.000 ns | 256 bytes (1%) | 6 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 210.479 μs (30%) | 0.000 ns | 288 bytes (1%) | 8 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 1.238 s (30%) | 0.000 ns | 288 bytes (1%) | 8 |
| `["sort", "issorted", "(\"forwards\", \"ascending\")"]` | 21.239 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"forwards\", \"descending\")"]` | 15.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"forwards\", \"ones\")"]` | 106.256 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"forwards\", \"random\")"]` | 18.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 643.000 ns (30%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 22.735 μs (30%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["sort", "issorted", "(\"reverse\", \"ones\")"]` | 107.308 μs (30%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 653.000 ns (30%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["sort", "mergesort", "(\"sort forwards\", \"ascending\")"]` | 492.797 μs (30%) | 0.000 ns | 586.56 KiB (1%) | 13 |
| `["sort", "mergesort", "(\"sort forwards\", \"descending\")"]` | 676.191 μs (30%) | 0.000 ns | 586.56 KiB (1%) | 13 |
| `["sort", "mergesort", "(\"sort forwards\", \"ones\")"]` | 504.550 μs (30%) | 0.000 ns | 586.64 KiB (1%) | 14 |
| `["sort", "mergesort", "(\"sort forwards\", \"random\")"]` | 2.853 ms (30%) | 0.000 ns | 586.64 KiB (1%) | 14 |
| `["sort", "mergesort", "(\"sort reverse\", \"ascending\")"]` | 632.490 μs (30%) | 0.000 ns | 586.78 KiB (1%) | 18 |
| `["sort", "mergesort", "(\"sort reverse\", \"descending\")"]` | 448.735 μs (30%) | 0.000 ns | 586.78 KiB (1%) | 18 |
| `["sort", "mergesort", "(\"sort reverse\", \"ones\")"]` | 540.450 μs (30%) | 0.000 ns | 586.86 KiB (1%) | 19 |
| `["sort", "mergesort", "(\"sort reverse\", \"random\")"]` | 2.907 ms (30%) | 0.000 ns | 586.86 KiB (1%) | 19 |
| `["sort", "mergesort", "(\"sort! forwards\", \"ascending\")"]` | 455.676 μs (30%) | 0.000 ns | 195.58 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sort! forwards\", \"descending\")"]` | 639.898 μs (30%) | 0.000 ns | 195.58 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sort! forwards\", \"ones\")"]` | 464.863 μs (30%) | 0.000 ns | 195.66 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sort! forwards\", \"random\")"]` | 2.806 ms (30%) | 0.000 ns | 195.66 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sort! reverse\", \"ascending\")"]` | 593.372 μs (30%) | 0.000 ns | 195.69 KiB (1%) | 7 |
| `["sort", "mergesort", "(\"sort! reverse\", \"descending\")"]` | 409.212 μs (30%) | 0.000 ns | 195.69 KiB (1%) | 7 |
| `["sort", "mergesort", "(\"sort! reverse\", \"ones\")"]` | 501.219 μs (30%) | 0.000 ns | 195.77 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sort! reverse\", \"random\")"]` | 2.868 ms (30%) | 0.000 ns | 195.77 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ascending\")"]` | 777.305 μs (30%) | 0.000 ns | 586.30 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"descending\")"]` | 1.141 ms (30%) | 0.000 ns | 586.30 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ones\")"]` | 816.492 μs (30%) | 0.000 ns | 586.41 KiB (1%) | 11 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"random\")"]` | 4.124 ms (30%) | 0.000 ns | 586.41 KiB (1%) | 11 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ascending\")"]` | 1.093 ms (30%) | 0.000 ns | 586.41 KiB (1%) | 10 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"descending\")"]` | 725.929 μs (30%) | 0.000 ns | 586.41 KiB (1%) | 10 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ones\")"]` | 860.433 μs (30%) | 0.000 ns | 586.52 KiB (1%) | 13 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"random\")"]` | 4.211 ms (30%) | 0.000 ns | 586.52 KiB (1%) | 13 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ascending\")"]` | 707.364 μs (30%) | 0.000 ns | 195.59 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"descending\")"]` | 1.072 ms (30%) | 0.000 ns | 195.59 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ones\")"]` | 785.998 μs (30%) | 0.000 ns | 195.70 KiB (1%) | 9 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"random\")"]` | 4.097 ms (30%) | 0.000 ns | 195.70 KiB (1%) | 9 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.067 ms (30%) | 0.000 ns | 195.70 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"descending\")"]` | 703.030 μs (30%) | 0.000 ns | 195.70 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ones\")"]` | 834.497 μs (30%) | 0.000 ns | 195.81 KiB (1%) | 11 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"random\")"]` | 4.177 ms (30%) | 0.000 ns | 195.81 KiB (1%) | 11 |
| `["sort", "quicksort", "(\"sort forwards\", \"ascending\")"]` | 346.573 μs (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "quicksort", "(\"sort forwards\", \"descending\")"]` | 359.667 μs (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "quicksort", "(\"sort forwards\", \"ones\")"]` | 477.929 μs (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "quicksort", "(\"sort forwards\", \"random\")"]` | 2.237 ms (30%) | 0.000 ns | 391.11 KiB (1%) | 11 |
| `["sort", "quicksort", "(\"sort reverse\", \"ascending\")"]` | 331.319 μs (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "quicksort", "(\"sort reverse\", \"descending\")"]` | 315.415 μs (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "quicksort", "(\"sort reverse\", \"ones\")"]` | 508.778 μs (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "quicksort", "(\"sort reverse\", \"random\")"]` | 2.264 ms (30%) | 0.000 ns | 391.33 KiB (1%) | 16 |
| `["sort", "quicksort", "(\"sort! forwards\", \"ascending\")"]` | 304.151 μs (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "quicksort", "(\"sort! forwards\", \"descending\")"]` | 316.839 μs (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "quicksort", "(\"sort! forwards\", \"ones\")"]` | 435.976 μs (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "quicksort", "(\"sort! forwards\", \"random\")"]` | 2.197 ms (30%) | 0.000 ns | 128 bytes (1%) | 3 |
| `["sort", "quicksort", "(\"sort! reverse\", \"ascending\")"]` | 286.539 μs (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "quicksort", "(\"sort! reverse\", \"descending\")"]` | 276.014 μs (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "quicksort", "(\"sort! reverse\", \"ones\")"]` | 467.149 μs (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "quicksort", "(\"sort! reverse\", \"random\")"]` | 2.219 ms (30%) | 0.000 ns | 240 bytes (1%) | 5 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"ascending\")"]` | 883.121 μs (30%) | 0.000 ns | 390.84 KiB (1%) | 6 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"descending\")"]` | 882.806 μs (30%) | 0.000 ns | 390.84 KiB (1%) | 6 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"ones\")"]` | 932.124 μs (30%) | 0.000 ns | 390.88 KiB (1%) | 8 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"random\")"]` | 3.607 ms (30%) | 0.000 ns | 390.88 KiB (1%) | 8 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"ascending\")"]` | 835.484 μs (30%) | 0.000 ns | 390.95 KiB (1%) | 8 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"descending\")"]` | 837.279 μs (30%) | 0.000 ns | 390.95 KiB (1%) | 8 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"ones\")"]` | 945.694 μs (30%) | 0.000 ns | 390.98 KiB (1%) | 10 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"random\")"]` | 3.595 ms (30%) | 0.000 ns | 390.98 KiB (1%) | 10 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ascending\")"]` | 810.548 μs (30%) | 0.000 ns | 144 bytes (1%) | 4 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"descending\")"]` | 810.037 μs (30%) | 0.000 ns | 144 bytes (1%) | 4 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 903.939 μs (30%) | 0.000 ns | 176 bytes (1%) | 6 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 3.577 ms (30%) | 0.000 ns | 176 bytes (1%) | 6 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ascending\")"]` | 809.023 μs (30%) | 0.000 ns | 256 bytes (1%) | 6 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"descending\")"]` | 809.458 μs (30%) | 0.000 ns | 256 bytes (1%) | 6 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 919.339 μs (30%) | 0.000 ns | 288 bytes (1%) | 8 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 3.565 ms (30%) | 0.000 ns | 288 bytes (1%) | 8 |
| `["sparse", "arithmetic", "(\"unary minus\", (20000, 20000))"]` | 26.913 ms (30%) | 17.063 ms | 61.18 MiB (1%) | 8 |
| `["sparse", "arithmetic", "(\"unary minus\", (600, 600))"]` | 5.579 μs (30%) | 0.000 ns | 60.59 KiB (1%) | 7 |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 515.000 ns (15%) | 0.000 ns | 2.19 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 2.438 μs (15%) | 0.000 ns | 14.84 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"Bidiagonal\", 1000)"]` | 25.492 μs (15%) | 0.000 ns | 134.30 KiB (1%) | 15 |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 104.000 ns (15%) | 0.000 ns | 544 bytes (1%) | 4 |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 159.000 ns (15%) | 0.000 ns | 2.67 KiB (1%) | 4 |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 2.180 μs (15%) | 0.000 ns | 23.92 KiB (1%) | 4 |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 86.000 ns (15%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 695.000 ns (15%) | 0.000 ns | 3.11 KiB (1%) | 10 |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 7.159 μs (15%) | 0.000 ns | 27.55 KiB (1%) | 12 |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 84.000 ns (15%) | 0.000 ns | 192 bytes (1%) | 3 |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 493.000 ns (15%) | 0.000 ns | 528 bytes (1%) | 7 |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 2.299 μs (15%) | 0.000 ns | 4.44 KiB (1%) | 8 |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 641.000 ns (15%) | 0.000 ns | 3.00 KiB (1%) | 19 |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 4.437 μs (15%) | 0.000 ns | 20.39 KiB (1%) | 19 |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 35.377 μs (15%) | 0.000 ns | 188.97 KiB (1%) | 28 |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 626.000 ns (15%) | 0.000 ns | 3.00 KiB (1%) | 19 |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 4.669 μs (15%) | 0.000 ns | 20.39 KiB (1%) | 19 |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 36.155 μs (15%) | 0.000 ns | 188.94 KiB (1%) | 26 |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 10)"]` | 147.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 100)"]` | 2.169 μs (30%) | 0.000 ns | 16.67 KiB (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 1000)"]` | 53.076 μs (30%) | 0.000 ns | 501.95 KiB (1%) | 6 |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 3.121 μs (30%) | 0.000 ns | 2.86 KiB (1%) | 29 |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 68.700 μs (30%) | 0.000 ns | 37.63 KiB (1%) | 311 |
| `["sparse", "index", "(\"spmat\", \"array\", 1000)"]` | 1.434 ms (30%) | 0.000 ns | 721.34 KiB (1%) | 3013 |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 10)"]` | 92.000 ns (30%) | 0.000 ns | 352 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 100)"]` | 96.000 ns (30%) | 0.000 ns | 416 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 1000)"]` | 131.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 1.092 μs (30%) | 0.000 ns | 1.47 KiB (1%) | 16 |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 2.445 μs (30%) | 0.000 ns | 3.86 KiB (1%) | 16 |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 1000)"]` | 30.721 μs (30%) | 0.000 ns | 25.91 KiB (1%) | 16 |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 232.000 ns (30%) | 0.000 ns | 784 bytes (1%) | 8 |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 540.000 ns (30%) | 0.000 ns | 1.95 KiB (1%) | 8 |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 3.892 μs (30%) | 0.000 ns | 12.67 KiB (1%) | 8 |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 93.000 ns (30%) | 0.000 ns | 352 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 100)"]` | 97.000 ns (30%) | 0.000 ns | 416 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 1000)"]` | 136.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"integer\", 10)"]` | 18.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spmat\", \"integer\", 100)"]` | 19.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spmat\", \"integer\", 1000)"]` | 18.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 279.000 ns (30%) | 0.000 ns | 816 bytes (1%) | 7 |
| `["sparse", "index", "(\"spmat\", \"logical\", 100)"]` | 5.305 μs (30%) | 0.000 ns | 7.02 KiB (1%) | 7 |
| `["sparse", "index", "(\"spmat\", \"logical\", 1000)"]` | 134.159 μs (30%) | 0.000 ns | 142.45 KiB (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"range\", 10)"]` | 152.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"range\", 100)"]` | 2.179 μs (30%) | 0.000 ns | 16.67 KiB (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"range\", 1000)"]` | 55.540 μs (30%) | 0.000 ns | 501.95 KiB (1%) | 6 |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 10)"]` | 136.000 ns (30%) | 0.000 ns | 288 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 100)"]` | 682.000 ns (30%) | 0.000 ns | 736 bytes (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 9.957 μs (30%) | 0.000 ns | 2.44 KiB (1%) | 13 |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 168.000 ns (30%) | 0.000 ns | 288 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 837.000 ns (30%) | 0.000 ns | 736 bytes (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 11.815 μs (30%) | 0.000 ns | 2.44 KiB (1%) | 13 |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 170.000 ns (30%) | 0.000 ns | 416 bytes (1%) | 6 |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 681.000 ns (30%) | 0.000 ns | 992 bytes (1%) | 8 |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 6.232 μs (30%) | 0.000 ns | 5.44 KiB (1%) | 12 |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 10)"]` | 136.000 ns (30%) | 0.000 ns | 288 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 100)"]` | 669.000 ns (30%) | 0.000 ns | 736 bytes (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 9.983 μs (30%) | 0.000 ns | 2.44 KiB (1%) | 13 |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 120.000 ns (30%) | 0.000 ns | 192 bytes (1%) | 3 |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 447.000 ns (30%) | 0.000 ns | 192 bytes (1%) | 3 |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 3.333 ms (30%) | 0.000 ns | 352 bytes (1%) | 3 |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 32.071 μs (30%) | 0.000 ns | 27.06 KiB (1%) | 18 |
| `["sparse", "index", "(\"spvec\", \"array\", 10000)"]` | 626.376 μs (30%) | 0.000 ns | 239.19 KiB (1%) | 21 |
| `["sparse", "index", "(\"spvec\", \"array\", 100000)"]` | 7.996 ms (30%) | 0.000 ns | 2.30 MiB (1%) | 21 |
| `["sparse", "index", "(\"spvec\", \"integer\", 1000)"]` | 21.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spvec\", \"integer\", 10000)"]` | 24.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spvec\", \"integer\", 100000)"]` | 22.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 3.334 μs (30%) | 0.000 ns | 4.94 KiB (1%) | 9 |
| `["sparse", "index", "(\"spvec\", \"logical\", 10000)"]` | 57.975 μs (30%) | 0.000 ns | 39.98 KiB (1%) | 10 |
| `["sparse", "index", "(\"spvec\", \"logical\", 100000)"]` | 598.930 μs (30%) | 0.000 ns | 394.77 KiB (1%) | 10 |
| `["sparse", "index", "(\"spvec\", \"range\", 1000)"]` | 159.000 ns (30%) | 0.000 ns | 832 bytes (1%) | 3 |
| `["sparse", "index", "(\"spvec\", \"range\", 10000)"]` | 297.000 ns (30%) | 0.000 ns | 2.00 KiB (1%) | 3 |
| `["sparse", "index", "(\"spvec\", \"range\", 100000)"]` | 972.000 ns (30%) | 0.000 ns | 5.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 5.433 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 5.513 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 5.257 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 51.091 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 7.052 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 59.823 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 58.154 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 580.091 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 143.629 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x400, dense 400x40 -> dense 4000x40\")"]` | 641.945 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 5.431 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x40, dense 40x400 -> dense 400x400\")"]` | 516.307 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 5.230 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x4000, dense 4000x40 -> dense 400x40\")"]` | 5.174 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 4.615 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 5.116 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 17.845 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 15.031 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.689 μs (30%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 14.882 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 15.803 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 16.350 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x50 -> dense 5x50\")"]` | 1.828 μs (30%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 15.977 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 3.515 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 500x50, dense 50x5 -> dense 500x5\")"]` | 5.859 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 36.990 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x5, dense 5x50 -> dense 50x50\")"]` | 6.331 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 31.353 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x500, dense 500x5 -> dense 50x5\")"]` | 36.973 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 27.827 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 26.761 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 1.204 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 1.392 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 11.343 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.062 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.976 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x200, sparse 2000x200 -> dense 20x2000\")"]` | 13.323 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 117.236 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 200x2000 -> dense 20x200\")"]` | 10.898 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x20, dense 20x20 -> dense 2000x20\")"]` | 1.225 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x200, dense 20x200 -> dense 2000x20\")"]` | 11.708 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 116.873 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x20, dense 200x20 -> dense 200x200\")"]` | 1.191 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 11.358 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x2000, dense 20x2000 -> dense 200x20\")"]` | 11.814 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.191 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x200, dense 200x200 -> dense 20x200\")"]` | 1.239 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 460.997 μs (30%) | 0.000 ns | 181.34 KiB (1%) | 26 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 448.544 μs (30%) | 0.000 ns | 147.92 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 567.847 μs (30%) | 0.000 ns | 143.55 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 34.795 μs (30%) | 0.000 ns | 27.75 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 2.011 ms (30%) | 0.000 ns | 240.06 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 2.272 ms (30%) | 0.000 ns | 232.56 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 4.709 ms (30%) | 0.000 ns | 229.16 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 262.918 μs (30%) | 0.000 ns | 33.61 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 44.796 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 297.830 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.884 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 25.341 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 174.284 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 305.136 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 37.240 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 21.931 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 5.433 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x40, sparse 400x40 -> dense 400x400\")"]` | 6.282 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 50.670 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 4.726 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 10.229 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 70.332 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 577.821 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 49.950 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 9.613 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x400, dense 40x400 -> dense 4000x40\")"]` | 93.563 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 933.747 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x40, dense 400x40 -> dense 400x400\")"]` | 9.283 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 90.697 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x4000, dense 40x4000 -> dense 400x40\")"]` | 94.497 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 9.512 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 10.006 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 334.394 μs (30%) | 0.000 ns | 93.19 KiB (1%) | 24 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 318.166 μs (30%) | 0.000 ns | 196.94 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 395.757 μs (30%) | 0.000 ns | 192.72 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 23.354 μs (30%) | 0.000 ns | 10.25 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.127 ms (30%) | 0.000 ns | 222.31 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 1.346 ms (30%) | 0.000 ns | 225.06 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 2.996 ms (30%) | 0.000 ns | 222.31 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 174.767 μs (30%) | 0.000 ns | 26.50 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 38.678 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 280.579 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.770 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 24.908 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 173.449 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 295.857 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 31.330 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 20.883 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 39.213 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 390.957 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 43.101 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 4.513 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 43.150 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 8.081 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 7.516 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 4.523 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 573.451 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x2000, dense 2000x20 -> dense 2000x20\")"]` | 857.123 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 504.116 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 719.398 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 226.403 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 650.898 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x200, dense 20x200 -> dense 200x200\")"]` | 217.604 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 139.344 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 542.506 μs (30%) | 0.000 ns | 33.28 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 6.262 ms (30%) | 0.000 ns | 228.83 KiB (1%) | 9 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.773 ms (30%) | 0.000 ns | 232.23 KiB (1%) | 9 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 75.183 μs (30%) | 0.000 ns | 27.42 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.143 ms (30%) | 0.000 ns | 143.22 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.257 ms (30%) | 0.000 ns | 239.73 KiB (1%) | 9 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 649.944 μs (30%) | 0.000 ns | 147.59 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 549.360 μs (30%) | 0.000 ns | 181.02 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 16.715 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 30.440 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 15.380 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 29.123 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 12.859 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 30.948 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 11.530 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 10.192 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 119.145 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 11.777 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 13.524 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 11.477 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 1.147 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 2.000 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 1.408 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 1.220 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x200, dense 20x2000 -> dense 200x20\")"]` | 13.431 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 118.098 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.540 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 11.478 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x2000, dense 20x200 -> dense 2000x20\")"]` | 11.174 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 1.219 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x200, dense 200x20 -> dense 200x200\")"]` | 1.123 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 1.119 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 4.816 ms (30%) | 0.000 ns | 229.16 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 272.641 μs (30%) | 0.000 ns | 33.61 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 2.282 ms (30%) | 0.000 ns | 232.56 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 569.969 μs (30%) | 0.000 ns | 143.55 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 35.732 μs (30%) | 0.000 ns | 27.75 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 2.026 ms (30%) | 0.000 ns | 240.06 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 449.754 μs (30%) | 0.000 ns | 147.92 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 467.943 μs (30%) | 0.000 ns | 181.34 KiB (1%) | 26 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 410.014 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.970 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 24.315 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 177.486 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 251.046 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 44.089 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 25.969 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 43.266 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 270.250 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 2.704 s (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 288.491 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 28.856 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 287.896 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 48.662 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 48.429 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 34.164 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 3.527 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 4.759 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 2.940 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 4.054 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 1.197 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 3.555 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 984.538 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 604.099 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 450.572 μs (30%) | 0.000 ns | 26.17 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 4.760 ms (30%) | 0.000 ns | 221.98 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.272 ms (30%) | 0.000 ns | 224.73 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 60.141 μs (30%) | 0.000 ns | 9.92 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 929.800 μs (30%) | 0.000 ns | 95.27 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 810.380 μs (30%) | 0.000 ns | 221.98 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 500.250 μs (30%) | 0.000 ns | 97.48 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 406.684 μs (30%) | 0.000 ns | 92.86 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 17.721 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 31.567 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 15.239 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 30.182 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 12.468 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 28.111 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 13.166 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 10.235 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 581.046 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 50.245 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 70.432 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 50.445 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 4.685 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 10.218 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 6.274 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 5.394 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x400, dense 40x4000 -> dense 400x40\")"]` | 105.852 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 931.598 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 11.996 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 90.595 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x4000, dense 40x400 -> dense 4000x40\")"]` | 89.325 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 9.438 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x400, dense 400x40 -> dense 400x400\")"]` | 8.618 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 8.651 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 2.984 ms (30%) | 0.000 ns | 222.31 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 172.965 μs (30%) | 0.000 ns | 26.50 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.344 ms (30%) | 0.000 ns | 225.06 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 395.918 μs (30%) | 0.000 ns | 192.72 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 23.086 μs (30%) | 0.000 ns | 10.25 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.126 ms (30%) | 0.000 ns | 222.31 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 318.207 μs (30%) | 0.000 ns | 196.94 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 334.802 μs (30%) | 0.000 ns | 93.19 KiB (1%) | 24 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 393.633 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.772 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 22.092 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 172.221 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 225.403 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 31.571 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 23.951 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 31.378 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 32.350 ms (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 64.880 ms (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 11.907 μs (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 18.582 μs (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"adjoint\", (20000, 10000))"]` | 41.642 ms (30%) | 9.046 ms | 45.91 MiB (1%) | 9 |
| `["sparse", "transpose", "(\"adjoint\", (20000, 20000))"]` | 85.202 ms (30%) | 15.632 ms | 91.69 MiB (1%) | 9 |
| `["sparse", "transpose", "(\"adjoint\", (600, 400))"]` | 15.930 μs (30%) | 0.000 ns | 60.58 KiB (1%) | 8 |
| `["sparse", "transpose", "(\"adjoint\", (600, 600))"]` | 24.420 μs (30%) | 0.000 ns | 88.33 KiB (1%) | 8 |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 29.772 ms (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 59.868 ms (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 9.458 μs (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 16.167 μs (30%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["sparse", "transpose", "(\"transpose\", (20000, 10000))"]` | 38.972 ms (30%) | 9.034 ms | 30.66 MiB (1%) | 9 |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 77.783 ms (30%) | 17.740 ms | 61.18 MiB (1%) | 9 |
| `["sparse", "transpose", "(\"transpose\", (600, 400))"]` | 12.303 μs (30%) | 0.000 ns | 42.14 KiB (1%) | 8 |
| `["sparse", "transpose", "(\"transpose\", (600, 600))"]` | 20.239 μs (30%) | 0.000 ns | 60.64 KiB (1%) | 8 |
| `["string", "join"]` | 96.356 ms (40%) | 18.965 ms | 156.27 MiB (1%) | 21 |
| `["string", "readuntil", "backtracking"]` | 435.085 μs (15%) | 0.000 ns | 105.83 KiB (1%) | 20 |
| `["string", "readuntil", "barbarian backtrack"]` | 447.094 μs (15%) | 0.000 ns | 73.81 KiB (1%) | 19 |
| `["string", "readuntil", "no backtracking"]` | 320.855 μs (15%) | 0.000 ns | 66.63 KiB (1%) | 18 |
| `["string", "readuntil", "target length 1"]` | 46.680 ns (15%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["string", "readuntil", "target length 1000"]` | 7.344 μs (15%) | 0.000 ns | 2.50 KiB (1%) | 12 |
| `["string", "readuntil", "target length 2"]` | 80.334 ns (15%) | 0.000 ns | 192 bytes (1%) | 4 |
| `["string", "readuntil", "target length 50000"]` | 353.129 μs (15%) | 0.000 ns | 66.63 KiB (1%) | 18 |
| `["string", "replace"]` | 112.360 μs (15%) | 0.000 ns | 12.06 KiB (1%) | 6 |
| `["string", "search", "Char"]` | 10.060 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string", "search", "String"]` | 21.846 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string", "searchindex", "Char"]` | 10.058 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string", "searchindex", "String"]` | 14.694 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 3, Float32)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 3, Float64)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 30, Float32)"]` | 31.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 30, Float64)"]` | 31.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 60, Float32)"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 60, Float64)"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 8, Float32)"]` | 17.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 8, Float64)"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 3, Float32)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 3, Float64)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 30, Float32)"]` | 31.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 30, Float64)"]` | 32.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 60, Float32)"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 60, Float64)"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 8, Float32)"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 8, Float64)"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (16, 16), (16, 16))"]` | 1.459 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (2, 2), (2, 2))"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (4, 4), (4, 4))"]` | 43.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (8, 8), (8, 8))"]` | 200.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (16, 16), (16,))"]` | 98.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (2, 2), (2,))"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (4, 4), (4,))"]` | 19.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (8, 8), (8,))"]` | 43.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (16, 16))"]` | 370.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 31.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (2, 2))"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (2,))"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 40.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (4,))"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (8, 8))"]` | 97.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (8,))"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 51.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (2, 2))"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (2,))"]` | 14.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 22.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (4,))"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 35.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 17.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (16, 16))"]` | 212.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 15.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 24.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 16.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (8, 8))"]` | 61.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 18.000 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "growth"]`
- `["array", "index"]`
- `["array", "reductions"]`
- `["array", "reverse"]`
- `["array", "setindex!"]`
- `["array", "subarray"]`
- `["broadcast", "dotop"]`
- `["broadcast", "fusion"]`
- `["broadcast", "mix_scalar_tuple"]`
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["micro"]`
- `["misc", "afoldl"]`
- `["misc", "bitshift"]`
- `["misc", "julia"]`
- `["misc", "parse"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
- `["nullable", "basic"]`
- `["nullable", "nullablearray"]`
- `["parallel", "remotecall"]`
- `["problem", "chaosgame"]`
- `["problem", "fem"]`
- `["problem", "go"]`
- `["problem", "grigoriadis khachiyan"]`
- `["problem", "imdb"]`
- `["problem", "json"]`
- `["problem", "laplacian"]`
- `["problem", "monte carlo"]`
- `["problem", "raytrace"]`
- `["problem", "seismic"]`
- `["problem", "simplex"]`
- `["problem", "spellcheck"]`
- `["problem", "stockcorr"]`
- `["problem", "ziggurat"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["scalar", "acos"]`
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "cos"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "transpose"]`
- `["string"]`
- `["string", "readuntil"]`
- `["string", "search"]`
- `["string", "searchindex"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2484
Commit 26eb512 (2017-11-09 21:25 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  100286424 s          0 s   17916485 s  4462618287 s         96 s
       #2  3501 MHz  437280059 s          0 s   11596932 s  4142649609 s         21 s
       #3  3501 MHz   86591022 s          0 s    9926798 s  4495454890 s         80 s
       #4  3501 MHz   82782771 s          0 s   10090338 s  4499109424 s         20 s
       
  Memory: 31.383651733398438 GB (14064.953125 MB free)
  Uptime: 4.594194e7 sec
  Load Avg:  0.88671875  0.9814453125  1.03466796875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
