# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a57250432abfafcc3b3ffa9df26e79516d1f6160](https://github.com/JuliaLang/julia/commit/a57250432abfafcc3b3ffa9df26e79516d1f6160)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a57250432abfafcc3b3ffa9df26e79516d1f6160#commitcomment-30437511)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-09-08

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
| `["array", "accumulate", "(\"accumulate!\", \"Float64\")"]` | 786.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "accumulate", "(\"accumulate!\", \"Int\")"]` | 380.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "accumulate", "(\"accumulate\", \"Float64\")"]` | 930.000 ns (5%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["array", "accumulate", "(\"accumulate\", \"Int\")"]` | 673.000 ns (5%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\")"]` | 1.041 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim1\")"]` | 1.036 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "accumulate", "(\"cumsum!\", \"Float64\", \"dim2\")"]` | 1.038 ms (5%) | 0.000 ns | 160 bytes (1%) | 5 |
| `["array", "accumulate", "(\"cumsum!\", \"Int\")"]` | 377.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "accumulate", "(\"cumsum\", \"Float64\")"]` | 1.213 μs (5%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim1\")"]` | 1.108 ms (5%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "accumulate", "(\"cumsum\", \"Float64\", \"dim2\")"]` | 1.109 ms (5%) | 0.000 ns | 7.63 MiB (1%) | 7 |
| `["array", "accumulate", "(\"cumsum\", \"Int\")"]` | 685.000 ns (5%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["array", "any/all", "(\"all\", \"Array{Float32,1} generator\")"]` | 3.283 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Array{Float32,1}\")"]` | 3.278 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Array{Float64,1} generator\")"]` | 3.488 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Array{Float64,1}\")"]` | 3.479 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Array{Int16,1} generator\")"]` | 3.622 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Array{Int16,1}\")"]` | 3.627 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Array{Int64,1} generator\")"]` | 4.364 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Array{Int64,1}\")"]` | 4.364 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"BitArray\")"]` | 92.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64} generator\")"]` | 2.589 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"UnitRange{Int64}\")"]` | 2.586 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"all\", \"Vector{Bool}\")"]` | 3.568 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Float32,1} generator\")"]` | 3.264 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 3.259 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 3.414 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Float64,1}\")"]` | 3.403 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Int16,1} generator\")"]` | 3.624 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Int16,1}\")"]` | 3.627 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Int64,1} generator\")"]` | 4.373 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Array{Int64,1}\")"]` | 4.356 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"BitArray\")"]` | 89.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64} generator\")"]` | 2.589 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 2.589 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "any/all", "(\"any\", \"Vector{Bool}\")"]` | 3.573 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "bitarray_bool_load!"]` | 2.217 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "bitarray_true_fill!"]` | 3.113 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "bitarray_true_load!"]` | 1.362 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "boolarray_bool_load!"]` | 686.881 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "boolarray_true_fill!"]` | 33.507 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "bool", "boolarray_true_load!"]` | 284.027 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "cat", "(\"catnd\", 5)"]` | 27.946 μs (5%) | 0.000 ns | 45.30 KiB (1%) | 123 |
| `["array", "cat", "(\"catnd\", 500)"]` | 2.628 ms (5%) | 0.000 ns | 11.49 MiB (1%) | 135 |
| `["array", "cat", "(\"catnd_setind\", 5)"]` | 15.351 μs (5%) | 0.000 ns | 41.56 KiB (1%) | 32 |
| `["array", "cat", "(\"catnd_setind\", 500)"]` | 2.078 ms (5%) | 0.000 ns | 11.48 MiB (1%) | 35 |
| `["array", "cat", "(\"hcat\", 5)"]` | 89.000 ns (5%) | 0.000 ns | 944 bytes (1%) | 2 |
| `["array", "cat", "(\"hcat\", 500)"]` | 632.765 μs (5%) | 0.000 ns | 7.63 MiB (1%) | 3 |
| `["array", "cat", "(\"hcat_setind\", 5)"]` | 171.000 ns (5%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"hcat_setind\", 500)"]` | 914.446 μs (5%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "cat", "(\"hvcat\", 5)"]` | 202.000 ns (5%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"hvcat\", 500)"]` | 987.734 μs (5%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "cat", "(\"hvcat_setind\", 5)"]` | 175.000 ns (5%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"hvcat_setind\", 500)"]` | 981.742 μs (5%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "cat", "(\"vcat\", 5)"]` | 179.000 ns (5%) | 0.000 ns | 944 bytes (1%) | 2 |
| `["array", "cat", "(\"vcat\", 500)"]` | 959.217 μs (5%) | 0.000 ns | 7.63 MiB (1%) | 3 |
| `["array", "cat", "(\"vcat_setind\", 5)"]` | 173.000 ns (5%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["array", "cat", "(\"vcat_setind\", 500)"]` | 957.708 μs (5%) | 0.000 ns | 7.63 MiB (1%) | 2 |
| `["array", "cat", "4467"]` | 1.282 μs (5%) | 0.000 ns | 416 bytes (1%) | 9 |
| `["array", "comprehension", "(\"collect\", \"Array{Float64,1}\")"]` | 44.598 ms (5%) | 19.105 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 55.695 ms (5%) | 17.298 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"comprehension_collect\", \"Array{Float64,1}\")"]` | 38.595 ms (5%) | 17.377 ms | 76.29 MiB (1%) | 3 |
| `["array", "comprehension", "(\"comprehension_collect\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 57.670 ms (5%) | 17.389 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"comprehension_indexing\", \"Array{Float64,1}\")"]` | 103.190 ms (30%) | 17.406 ms | 76.29 MiB (1%) | 4 |
| `["array", "comprehension", "(\"comprehension_indexing\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 134.541 ms (30%) | 19.024 ms | 76.29 MiB (1%) | 2 |
| `["array", "comprehension", "(\"comprehension_iteration\", \"Array{Float64,1}\")"]` | 99.274 ms (5%) | 17.453 ms | 76.29 MiB (1%) | 3 |
| `["array", "comprehension", "(\"comprehension_iteration\", \"StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}\")"]` | 132.340 ms (5%) | 20.974 ms | 76.29 MiB (1%) | 2 |
| `["array", "convert", "(\"Complex{Float64}\", \"Int\")"]` | 7.118 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "convert", "(\"Float64\", \"Int\")"]` | 5.245 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "convert", "(\"Int\", \"Complex{Float64}\")"]` | 51.749 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "convert", "(\"Int\", \"Float64\")"]` | 15.450 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Float32,1}\")"]` | 6.012 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Float64,1}\")"]` | 6.489 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Int16,1}\")"]` | 733.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float32,1}\")"]` | 12.898 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Float64,1}\")"]` | 11.744 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Int16,1}\")"]` | 5.282 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == Array{Int64,1}\")"]` | 2.087 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Int64,1} == UnitRange{Int64}\")"]` | 6.864 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Array{Int64,1}\")"]` | 2.420 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"BitArray\")"]` | 48.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"UnitRange{Int64}\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"==\", \"Vector{Bool}\")"]` | 5.151 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Float32,1}\")"]` | 10.300 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Float64,1}\")"]` | 10.379 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Int16,1}\")"]` | 5.166 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float32,1}\")"]` | 17.885 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Float64,1}\")"]` | 13.747 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int16,1}\")"]` | 5.265 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal Array{Int64,1}\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1} isequal UnitRange{Int64}\")"]` | 6.863 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Array{Int64,1}\")"]` | 5.565 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"BitArray\")"]` | 12.851 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"UnitRange{Int64}\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "equality", "(\"isequal\", \"Vector{Bool}\")"]` | 5.151 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "growth", "(\"append!\", 2048)"]` | 2.546 μs (5%) | 0.000 ns | 32.06 KiB (1%) | 1 |
| `["array", "growth", "(\"append!\", 256)"]` | 455.000 ns (5%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["array", "growth", "(\"append!\", 8)"]` | 44.000 ns (5%) | 0.000 ns | 144 bytes (1%) | 1 |
| `["array", "growth", "(\"prerend!\", 2048)"]` | 2.431 μs (5%) | 0.000 ns | 64.06 KiB (1%) | 1 |
| `["array", "growth", "(\"prerend!\", 256)"]` | 436.000 ns (5%) | 0.000 ns | 8.06 KiB (1%) | 1 |
| `["array", "growth", "(\"prerend!\", 8)"]` | 57.000 ns (5%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["array", "growth", "(\"push_multiple!\", 2048)"]` | 10.162 μs (5%) | 0.000 ns | 32.06 KiB (1%) | 1 |
| `["array", "growth", "(\"push_multiple!\", 256)"]` | 1.404 μs (5%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["array", "growth", "(\"push_multiple!\", 8)"]` | 70.000 ns (5%) | 0.000 ns | 144 bytes (1%) | 1 |
| `["array", "growth", "(\"push_single!\", 2048)"]` | 7.180 μs (5%) | 0.000 ns | 51.86 KiB (1%) | 10 |
| `["array", "growth", "(\"push_single!\", 256)"]` | 5.920 μs (5%) | 0.000 ns | 23.86 KiB (1%) | 10 |
| `["array", "growth", "(\"push_single!\", 8)"]` | 5.600 μs (5%) | 0.000 ns | 19.94 KiB (1%) | 10 |
| `["array", "index", "(\"mapr_access\", \"Array{Float32,2}\")"]` | 6.799 ms (50%) | 0.000 ns | 7.75 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"Array{Int32,2}\")"]` | 6.697 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505000 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 91.499 ms (50%) | 20.522 ms | 26.86 MiB (1%) | 1257000 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 91.438 ms (50%) | 20.105 ms | 26.86 MiB (1%) | 1256500 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 6.453 ms (50%) | 0.000 ns | 7.75 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 6.587 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505000 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 6.757 ms (50%) | 0.000 ns | 7.75 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 6.102 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505000 |
| `["array", "index", "(\"mapr_access\", \"BitArray{2}\")"]` | 67.172 ms (50%) | 0.000 ns | 19.21 MiB (1%) | 755500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 95.285 ms (50%) | 20.659 ms | 26.86 MiB (1%) | 1257000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 6.487 ms (50%) | 0.000 ns | 7.75 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 91.543 ms (50%) | 20.500 ms | 26.86 MiB (1%) | 1257000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 6.744 μs (50%) | 0.000 ns | 3.06 KiB (1%) | 136 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.369 μs (50%) | 0.000 ns | 1.03 KiB (1%) | 51 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 7.116 ms (50%) | 0.000 ns | 7.75 MiB (1%) | 505500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 8.649 ms (50%) | 0.000 ns | 7.72 MiB (1%) | 503491 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 89.812 ms (50%) | 20.079 ms | 26.86 MiB (1%) | 1256500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 7.252 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 95.079 ms (50%) | 20.192 ms | 26.86 MiB (1%) | 1256500 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 6.838 μs (50%) | 0.000 ns | 3.00 KiB (1%) | 132 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.236 μs (50%) | 0.000 ns | 1008 bytes (1%) | 48 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 6.800 ms (50%) | 0.000 ns | 7.74 MiB (1%) | 505000 |
| `["array", "index", "(\"mapr_access\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 8.435 ms (50%) | 0.000 ns | 7.71 MiB (1%) | 502992 |
| `["array", "index", "(\"sum\", \"3darray\")"]` | 146.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sum\", \"3dsubarray\")"]` | 2.133 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.011 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"1.0:1.0:100000.0\")"]` | 270.459 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"100000:-1:1\")"]` | 51.299 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"1:100000\")"]` | 76.935 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"Array{Float32,2}\")"]` | 376.058 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"Array{Float64,3}\")"]` | 1.054 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"Array{Int32,2}\")"]` | 386.668 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 376.062 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 414.345 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 376.082 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 386.682 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 376.048 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 386.683 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"BitArray{2}\")"]` | 546.238 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 399.031 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 350.982 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 337.507 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.794 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.098 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 376.086 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 370.480 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.022 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 407.584 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 364.335 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 375.425 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 2.783 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.357 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 414.373 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 399.815 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 26.963 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"1.0:1.0:100000.0\")"]` | 270.575 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"100000:-1:1\")"]` | 21.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"1:100000\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float32,2}\")"]` | 24.166 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Float64,3}\")"]` | 1.043 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"Array{Int32,2}\")"]` | 21.104 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 24.018 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 21.129 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 24.241 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 21.166 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 24.247 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 21.195 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"BitArray{2}\")"]` | 1.791 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 24.320 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 24.667 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.400 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.564 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 7.927 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 24.850 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 191.653 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 789.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 21.083 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 21.222 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 109.717 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.012 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 8.672 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 21.608 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcartesian_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 110.236 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon\", \"1.0:0.00010001000100010001:2.0\")"]` | 24.954 μs (50%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"1.0:1.0:100000.0\")"]` | 246.896 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"100000:-1:1\")"]` | 61.953 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"1:100000\")"]` | 61.367 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumcolon\", \"Array{Float32,2}\")"]` | 221.757 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"Array{Int32,2}\")"]` | 222.972 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 222.565 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 222.471 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 224.930 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 224.261 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 222.445 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 223.824 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"BitArray{2}\")"]` | 29.279 μs (50%) | 0.000 ns | 85.94 KiB (1%) | 1000 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 217.371 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 220.415 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 284.123 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.917 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 18.162 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 221.425 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 285.283 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 225.636 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 224.024 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 284.237 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 11.833 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 18.420 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 222.519 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumcolon\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 284.183 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumcolon_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 24.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"1.0:1.0:100000.0\")"]` | 24.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"100000:-1:1\")"]` | 44.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"1:100000\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"Array{Float32,2}\")"]` | 409.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"Array{Int32,2}\")"]` | 303.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 2.991 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 2.890 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 2.931 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 3.026 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 2.932 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 2.636 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"BitArray{2}\")"]` | 3.265 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.743 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.139 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 3.006 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.096 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 5.925 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 3.046 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.874 μs (50%) | 0.000 ns | 31.19 KiB (1%) | 499 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.837 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.101 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 2.995 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.011 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 5.881 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.915 μs (50%) | 0.000 ns | 23.44 KiB (1%) | 500 |
| `["array", "index", "(\"sumcolon_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 2.879 μs (50%) | 0.000 ns | 31.19 KiB (1%) | 499 |
| `["array", "index", "(\"sumeach\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.087 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"1.0:1.0:100000.0\")"]` | 268.758 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"100000:-1:1\")"]` | 21.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"1:100000\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"Array{Float32,2}\")"]` | 192.338 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"Array{Float64,3}\")"]` | 1.040 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"Array{Int32,2}\")"]` | 20.002 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.347 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 20.041 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 376.073 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 386.684 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 376.064 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 386.613 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"BitArray{2}\")"]` | 290.809 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.347 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 351.000 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.350 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.564 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.096 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 317.386 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 370.537 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 1.022 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 20.051 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 364.324 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 95.005 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 96.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.362 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 321.179 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 399.792 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 26.967 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"1.0:1.0:100000.0\")"]` | 270.545 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"100000:-1:1\")"]` | 21.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"1:100000\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"Array{Float32,2}\")"]` | 8.274 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumeach_view\", \"Array{Float64,3}\")"]` | 41.805 μs (50%) | 0.000 ns | 103.98 KiB (1%) | 2662 |
| `["array", "index", "(\"sumeach_view\", \"Array{Int32,2}\")"]` | 8.242 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 22.329 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 20.024 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 24.224 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 21.200 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 24.248 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 21.176 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"BitArray{2}\")"]` | 28.936 ms (50%) | 20.312 ms | 26.70 MiB (1%) | 500000 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.364 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 24.701 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.363 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.670 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 8.052 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 24.860 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 191.658 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 789.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 83.250 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 21.234 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 112.071 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.722 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 8.722 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 21.642 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 110.314 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.014 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"1.0:1.0:100000.0\")"]` | 270.480 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"100000:-1:1\")"]` | 25.665 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"1:100000\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"Array{Float32,2}\")"]` | 192.348 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"Array{Float64,3}\")"]` | 1.040 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"Array{Int32,2}\")"]` | 20.518 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.367 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 86.964 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 361.440 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 355.736 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 353.091 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 396.892 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"BitArray{2}\")"]` | 288.801 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.861 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 385.561 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 194.443 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.564 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 8.874 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 382.899 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 395.749 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 2.107 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 158.021 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 396.036 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 164.658 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.244 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 9.235 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 364.276 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 442.574 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.158 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"1.0:1.0:100000.0\")"]` | 271.451 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"100000:-1:1\")"]` | 44.901 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"1:100000\")"]` | 76.942 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Float32,2}\")"]` | 192.351 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Float64,3}\")"]` | 1.040 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"Array{Int32,2}\")"]` | 95.403 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.360 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 102.647 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 897.493 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 961.603 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 961.605 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 897.496 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"BitArray{2}\")"]` | 328.919 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.798 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 961.605 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 194.781 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.566 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 14.020 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 961.915 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.030 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 7.205 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 107.965 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 961.605 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 126.562 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.042 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 14.135 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.026 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumelt_boundscheck\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.030 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"1.0:0.00010001000100010001:2.0\")"]` | 27.088 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"1.0:1.0:100000.0\")"]` | 268.759 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"100000:-1:1\")"]` | 20.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"1:100000\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"Array{Float32,2}\")"]` | 192.338 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"Array{Float64,3}\")"]` | 1.040 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"Array{Int32,2}\")"]` | 20.033 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 192.347 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 20.013 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 833.385 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 833.354 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 833.384 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 833.356 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"BitArray{2}\")"]` | 290.839 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.347 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 897.500 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.350 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.562 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 13.403 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 833.406 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 893.919 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 7.202 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 20.045 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 897.488 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 95.022 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 96.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 13.825 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 833.403 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 893.920 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 26.966 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"1.0:1.0:100000.0\")"]` | 270.524 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"100000:-1:1\")"]` | 22.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"1:100000\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"Array{Float32,2}\")"]` | 8.263 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumlinear_view\", \"Array{Float64,3}\")"]` | 41.870 μs (50%) | 0.000 ns | 103.98 KiB (1%) | 2662 |
| `["array", "index", "(\"sumlinear_view\", \"Array{Int32,2}\")"]` | 8.258 ms (50%) | 0.000 ns | 19.07 MiB (1%) | 500000 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 22.335 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 20.031 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 10.486 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 10.497 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 10.542 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 10.497 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"BitArray{2}\")"]` | 28.464 ms (50%) | 19.874 ms | 26.70 MiB (1%) | 500000 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.364 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 10.565 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 192.364 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.671 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 56.166 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 10.214 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.405 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float64,3,Array{Float64,3},Tuple{UnitRange{Int64},UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 86.250 μs (50%) | 0.000 ns | 78.13 KiB (1%) | 1000 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 83.249 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 10.496 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 112.060 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 1.726 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 55.999 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 10.253 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 9.355 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumlogical\", \"1.0:0.00010001000100010001:2.0\")"]` | 11.703 μs (50%) | 0.000 ns | 21.09 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"1.0:1.0:100000.0\")"]` | 119.979 μs (50%) | 0.000 ns | 207.89 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"100000:-1:1\")"]` | 88.011 μs (50%) | 0.000 ns | 207.89 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"1:100000\")"]` | 87.999 μs (50%) | 0.000 ns | 207.89 KiB (1%) | 6 |
| `["array", "index", "(\"sumlogical\", \"Array{Float32,2}\")"]` | 184.392 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"Array{Int32,2}\")"]` | 184.316 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 184.326 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 184.746 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 185.858 μs (50%) | 0.000 ns | 328.36 KiB (1%) | 1503 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 186.426 μs (50%) | 0.000 ns | 328.36 KiB (1%) | 1503 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 184.274 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 184.828 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"BitArray{2}\")"]` | 264.318 μs (50%) | 0.000 ns | 78.36 KiB (1%) | 1503 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 184.990 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 185.720 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 207.835 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 15.863 μs (50%) | 0.000 ns | 62.69 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 18.881 μs (50%) | 0.000 ns | 62.69 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 184.632 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 208.568 μs (50%) | 0.000 ns | 319.91 KiB (1%) | 1001 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 184.891 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 199.276 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 206.356 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 15.680 μs (50%) | 0.000 ns | 62.69 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 18.548 μs (50%) | 0.000 ns | 62.69 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 184.979 μs (50%) | 0.000 ns | 320.55 KiB (1%) | 1003 |
| `["array", "index", "(\"sumlogical\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 208.658 μs (50%) | 0.000 ns | 319.91 KiB (1%) | 1001 |
| `["array", "index", "(\"sumlogical_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 9.149 μs (50%) | 0.000 ns | 21.23 KiB (1%) | 9 |
| `["array", "index", "(\"sumlogical_view\", \"1.0:1.0:100000.0\")"]` | 88.618 μs (50%) | 0.000 ns | 208.03 KiB (1%) | 9 |
| `["array", "index", "(\"sumlogical_view\", \"100000:-1:1\")"]` | 88.449 μs (50%) | 0.000 ns | 208.02 KiB (1%) | 9 |
| `["array", "index", "(\"sumlogical_view\", \"1:100000\")"]` | 88.725 μs (50%) | 0.000 ns | 208.00 KiB (1%) | 9 |
| `["array", "index", "(\"sumlogical_view\", \"Array{Float32,2}\")"]` | 227.344 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"Array{Int32,2}\")"]` | 228.094 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 252.325 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 251.713 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 251.660 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 253.123 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 250.517 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 251.411 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"BitArray{2}\")"]` | 229.767 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 235.102 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 223.913 μs (50%) | 0.000 ns | 586.17 KiB (1%) | 2003 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 230.503 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 56.962 μs (50%) | 0.000 ns | 109.56 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 82.750 μs (50%) | 0.000 ns | 109.56 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 252.814 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 253.106 μs (50%) | 0.000 ns | 592.80 KiB (1%) | 2498 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 228.182 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 223.825 μs (50%) | 0.000 ns | 586.17 KiB (1%) | 2003 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 229.168 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 56.623 μs (50%) | 0.000 ns | 109.56 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 83.441 μs (50%) | 0.000 ns | 109.56 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 252.695 μs (50%) | 0.000 ns | 593.98 KiB (1%) | 2503 |
| `["array", "index", "(\"sumlogical_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 252.596 μs (50%) | 0.000 ns | 592.80 KiB (1%) | 2498 |
| `["array", "index", "(\"sumrange\", \"1.0:0.00010001000100010001:2.0\")"]` | 25.006 μs (50%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"1.0:1.0:100000.0\")"]` | 250.469 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"100000:-1:1\")"]` | 61.384 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"1:100000\")"]` | 61.638 μs (50%) | 0.000 ns | 781.33 KiB (1%) | 2 |
| `["array", "index", "(\"sumrange\", \"Array{Float32,2}\")"]` | 228.555 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"Array{Int32,2}\")"]` | 230.886 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 231.202 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 228.658 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 230.430 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 234.181 μs (50%) | 0.000 ns | 1.05 MiB (1%) | 1000 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 230.078 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 232.151 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"BitArray{2}\")"]` | 29.583 μs (50%) | 0.000 ns | 85.94 KiB (1%) | 1000 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 231.214 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 227.982 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 290.569 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 12.120 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 18.355 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 231.412 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 288.372 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 227.477 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 228.803 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 288.079 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 12.137 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 18.322 μs (50%) | 0.000 ns | 46.88 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 231.877 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 500 |
| `["array", "index", "(\"sumrange\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 288.236 μs (50%) | 0.000 ns | 1.04 MiB (1%) | 499 |
| `["array", "index", "(\"sumrange_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 21.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"1.0:1.0:100000.0\")"]` | 21.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"100000:-1:1\")"]` | 42.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"1:100000\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"Array{Float32,2}\")"]` | 410.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"Array{Int32,2}\")"]` | 327.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 412.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 329.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 413.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 324.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 412.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 325.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"BitArray{2}\")"]` | 857.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 414.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 3.956 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 413.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 444.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 6.046 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 590.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 727.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 307.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 4.078 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 345.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 442.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 5.777 μs (50%) | 0.000 ns | 31.25 KiB (1%) | 500 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 590.000 ns (50%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["array", "index", "(\"sumrange_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 722.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "(\"sumvector\", \"1.0:0.00010001000100010001:2.0\")"]` | 99.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 2 |
| `["array", "index", "(\"sumvector\", \"1.0:1.0:100000.0\")"]` | 99.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 2 |
| `["array", "index", "(\"sumvector\", \"100000:-1:1\")"]` | 102.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 2 |
| `["array", "index", "(\"sumvector\", \"1:100000\")"]` | 89.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 2 |
| `["array", "index", "(\"sumvector\", \"Array{Float32,2}\")"]` | 17.333 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"Array{Int32,2}\")"]` | 16.958 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 17.265 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 18.569 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 20.268 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 20.403 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 17.339 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 18.167 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"BitArray{2}\")"]` | 23.204 μs (50%) | 0.000 ns | 62.63 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 17.125 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 17.373 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 23.677 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 13.781 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 22.973 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 17.663 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 24.612 μs (50%) | 0.000 ns | 54.70 KiB (1%) | 500 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 17.324 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 17.004 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 23.581 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 13.891 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 23.233 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 18.045 μs (50%) | 0.000 ns | 54.81 KiB (1%) | 501 |
| `["array", "index", "(\"sumvector\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 24.714 μs (50%) | 0.000 ns | 54.70 KiB (1%) | 500 |
| `["array", "index", "(\"sumvector_view\", \"1.0:0.00010001000100010001:2.0\")"]` | 80.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"1.0:1.0:100000.0\")"]` | 80.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"100000:-1:1\")"]` | 103.000 ns (50%) | 0.000 ns | 240 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"1:100000\")"]` | 70.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 3 |
| `["array", "index", "(\"sumvector_view\", \"Array{Float32,2}\")"]` | 8.630 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"Array{Int32,2}\")"]` | 8.154 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 29.860 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 29.757 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}\")"]` | 30.028 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}\")"]` | 29.962 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}\")"]` | 30.069 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}\")"]` | 30.564 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"BitArray{2}\")"]` | 7.326 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.177 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 28.108 μs (50%) | 0.000 ns | 101.69 KiB (1%) | 1501 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 10.886 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 5.778 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 30.688 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 30.282 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 29.667 μs (50%) | 0.000 ns | 39.11 KiB (1%) | 999 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.410 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}\")"]` | 28.197 μs (50%) | 0.000 ns | 101.69 KiB (1%) | 1501 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.379 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 6.018 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 30.821 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 30.671 μs (50%) | 0.000 ns | 39.19 KiB (1%) | 1001 |
| `["array", "index", "(\"sumvector_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 29.061 μs (50%) | 0.000 ns | 39.11 KiB (1%) | 999 |
| `["array", "index", "2d"]` | 66.130 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "3d"]` | 84.597 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "4d"]` | 99.763 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "5d"]` | 193.420 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "6d"]` | 210.815 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "7d"]` | 4.948 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "ind2sub"]` | 666.722 μs (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "index", "sub2ind"]` | 516.270 ms (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norm1\", \"Float64\")"]` | 148.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norm1\", \"Int64\")"]` | 783.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Float64\")"]` | 1.406 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.norminf\", \"Int64\")"]` | 215.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Float64\")"]` | 786.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_mapreduce\", \"Int64\")"]` | 109.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Float64\")"]` | 787.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"BaseBenchmarks.ArrayBenchmarks.perf_reduce\", \"Int64\")"]` | 111.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"LinearAlgebra.norm\", \"Float64\")"]` | 286.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"LinearAlgebra.norm\", \"Int64\")"]` | 983.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"Statistics.mean\", \"Float64\")"]` | 117.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"Statistics.mean\", \"Int64\")"]` | 92.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"maxabs\", \"Float64\")"]` | 2.067 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"maxabs\", \"Int64\")"]` | 798.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sum\", \"Float64\")"]` | 112.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sum\", \"Int64\")"]` | 87.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs2\", \"Float64\")"]` | 144.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs2\", \"Int64\")"]` | 287.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs\", \"Float64\")"]` | 115.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reductions", "(\"sumabs\", \"Int64\")"]` | 159.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reverse", "rev_load_fast!"]` | 763.605 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reverse", "rev_load_slow!"]` | 1.714 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reverse", "rev_loadmul_fast!"]` | 3.133 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "reverse", "rev_loadmul_slow!"]` | 3.134 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["array", "setindex!", "(\"setindex!\", 1)"]` | 1.162 μs (5%) | 0.000 ns | 336 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 2)"]` | 1.126 μs (5%) | 0.000 ns | 336 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 3)"]` | 1.184 μs (5%) | 0.000 ns | 336 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 4)"]` | 1.185 μs (5%) | 0.000 ns | 336 bytes (1%) | 8 |
| `["array", "setindex!", "(\"setindex!\", 5)"]` | 1.169 μs (5%) | 0.000 ns | 336 bytes (1%) | 8 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 100)"]` | 1.882 ms (5%) | 0.000 ns | 5.82 MiB (1%) | 1707 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 1000)"]` | 5.565 s (5%) | 3.749 s | 5.03 GiB (1%) | 21811 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 250)"]` | 78.444 ms (5%) | 52.243 ms | 83.57 MiB (1%) | 4407 |
| `["array", "subarray", "(\"lucompletepivCopy!\", 500)"]` | 696.627 ms (5%) | 487.989 ms | 651.57 MiB (1%) | 8907 |
| `["array", "subarray", "(\"lucompletepivSub!\", 100)"]` | 1.729 ms (5%) | 0.000 ns | 3.20 MiB (1%) | 2443 |
| `["array", "subarray", "(\"lucompletepivSub!\", 1000)"]` | 3.363 s (5%) | 1.870 s | 2.53 GiB (1%) | 28847 |
| `["array", "subarray", "(\"lucompletepivSub!\", 250)"]` | 40.460 ms (5%) | 17.438 ms | 43.21 MiB (1%) | 6193 |
| `["array", "subarray", "(\"lucompletepivSub!\", 500)"]` | 420.110 ms (5%) | 244.313 ms | 331.00 MiB (1%) | 12443 |
| `["broadcast", "dotop", "(\"Float64\", (1000, 1000), 2)"]` | 412.075 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 1)"]` | 1.907 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "dotop", "(\"Float64\", (1000000,), 2)"]` | 1.016 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 2)"]` | 677.076 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "fusion", "(\"Float64\", (1000, 1000), 3)"]` | 1.080 ms (5%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 1)"]` | 1.111 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "fusion", "(\"Float64\", (1000000,), 2)"]` | 1.016 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(10, \"scal_tup_x3\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(10, \"tup_tup\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(3, \"scal_tup_x3\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(3, \"tup_tup\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(5, \"scal_tup_x3\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "mix_scalar_tuple", "(5, \"tup_tup\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "sparse", "((1000, 1000), 1)"]` | 5.277 μs (5%) | 0.000 ns | 24.16 KiB (1%) | 14 |
| `["broadcast", "sparse", "((1000, 1000), 2)"]` | 7.564 μs (5%) | 0.000 ns | 39.55 KiB (1%) | 4 |
| `["broadcast", "sparse", "((10000000,), 1)"]` | 36.531 μs (5%) | 0.000 ns | 156.92 KiB (1%) | 15 |
| `["broadcast", "sparse", "((10000000,), 2)"]` | 31.321 μs (5%) | 0.000 ns | 313.22 KiB (1%) | 6 |
| `["broadcast", "typeargs", "(\"array\", 10)"]` | 51.000 ns (5%) | 0.000 ns | 160 bytes (1%) | 1 |
| `["broadcast", "typeargs", "(\"array\", 3)"]` | 44.000 ns (5%) | 0.000 ns | 112 bytes (1%) | 1 |
| `["broadcast", "typeargs", "(\"array\", 5)"]` | 45.000 ns (5%) | 0.000 ns | 128 bytes (1%) | 1 |
| `["broadcast", "typeargs", "(\"tuple\", 10)"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "typeargs", "(\"tuple\", 3)"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["broadcast", "typeargs", "(\"tuple\", 5)"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"BitSet\", \"Int\", \"pop!\")"]` | 8.753 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter!\")"]` | 36.086 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"filter\")"]` | 44.513 μs (25%) | 0.000 ns | 34.66 KiB (1%) | 695 |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 91.857 μs (25%) | 0.000 ns | 27.97 KiB (1%) | 895 |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"filter!\")"]` | 4.713 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"filter\")"]` | 6.899 μs (25%) | 0.000 ns | 24.00 KiB (1%) | 13 |
| `["collection", "deletion", "(\"Dict\", \"Int\", \"pop!\")"]` | 6.121 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter!\")"]` | 38.523 μs (25%) | 0.000 ns | 31.00 KiB (1%) | 992 |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter\")"]` | 54.285 μs (25%) | 0.000 ns | 55.00 KiB (1%) | 1005 |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 24.288 μs (25%) | 0.000 ns | 31.00 KiB (1%) | 992 |
| `["collection", "deletion", "(\"IdDict\", \"Any\", \"filter!\")"]` | 23.862 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"IdDict\", \"Any\", \"filter\")"]` | 38.442 μs (25%) | 0.000 ns | 24.55 KiB (1%) | 7 |
| `["collection", "deletion", "(\"IdDict\", \"Int\", \"filter!\")"]` | 12.769 μs (25%) | 0.000 ns | 2.34 KiB (1%) | 150 |
| `["collection", "deletion", "(\"IdDict\", \"Int\", \"filter\")"]` | 31.153 μs (25%) | 0.000 ns | 29.08 KiB (1%) | 297 |
| `["collection", "deletion", "(\"IdDict\", \"String\", \"filter!\")"]` | 33.841 μs (25%) | 0.000 ns | 31.00 KiB (1%) | 992 |
| `["collection", "deletion", "(\"IdDict\", \"String\", \"filter\")"]` | 62.641 μs (25%) | 0.000 ns | 55.55 KiB (1%) | 999 |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter!\")"]` | 33.978 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Set\", \"Any\", \"filter\")"]` | 35.133 μs (25%) | 0.000 ns | 21.20 KiB (1%) | 522 |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 86.054 μs (25%) | 0.000 ns | 13.98 KiB (1%) | 895 |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter!\")"]` | 4.718 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Set\", \"Int\", \"filter\")"]` | 6.272 μs (25%) | 0.000 ns | 13.27 KiB (1%) | 14 |
| `["collection", "deletion", "(\"Set\", \"Int\", \"pop!\")"]` | 5.837 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter!\")"]` | 28.051 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 44.240 μs (25%) | 0.000 ns | 13.27 KiB (1%) | 14 |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 21.438 μs (25%) | 0.000 ns | 15.50 KiB (1%) | 992 |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter!\")"]` | 1.399 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"filter\")"]` | 6.334 μs (25%) | 0.000 ns | 8.39 KiB (1%) | 9 |
| `["collection", "deletion", "(\"Vector\", \"Any\", \"pop!\")"]` | 3.103 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter!\")"]` | 746.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"filter\")"]` | 3.604 μs (25%) | 0.000 ns | 8.39 KiB (1%) | 9 |
| `["collection", "deletion", "(\"Vector\", \"Int\", \"pop!\")"]` | 3.110 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 6.794 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter\")"]` | 12.451 μs (25%) | 0.000 ns | 16.45 KiB (1%) | 10 |
| `["collection", "deletion", "(\"Vector\", \"String\", \"pop!\")"]` | 3.101 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"iterator\")"]` | 1.949 μs (25%) | 0.000 ns | 384 bytes (1%) | 5 |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\")"]` | 1.966 μs (25%) | 0.000 ns | 384 bytes (1%) | 5 |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"sorted\", \"loop\", \"sizehint!\")"]` | 1.936 μs (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"iterator\")"]` | 1.696 μs (25%) | 0.000 ns | 496 bytes (1%) | 4 |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\")"]` | 1.692 μs (25%) | 0.000 ns | 496 bytes (1%) | 4 |
| `["collection", "initialization", "(\"BitSet\", \"Int\", \"unsorted\", \"loop\", \"sizehint!\")"]` | 1.717 μs (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"iterator\")"]` | 169.781 μs (25%) | 0.000 ns | 133.67 KiB (1%) | 2595 |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\")"]` | 137.833 μs (25%) | 0.000 ns | 125.73 KiB (1%) | 2155 |
| `["collection", "initialization", "(\"Dict\", \"Any\", \"loop\", \"sizehint!\")"]` | 116.216 μs (25%) | 0.000 ns | 114.80 KiB (1%) | 1847 |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"iterator\")"]` | 16.579 μs (25%) | 0.000 ns | 24.00 KiB (1%) | 13 |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\")"]` | 17.005 μs (25%) | 0.000 ns | 24.00 KiB (1%) | 13 |
| `["collection", "initialization", "(\"Dict\", \"Int\", \"loop\", \"sizehint!\")"]` | 13.971 μs (25%) | 0.000 ns | 17.78 KiB (1%) | 7 |
| `["collection", "initialization", "(\"Dict\", \"String\", \"iterator\")"]` | 76.418 μs (25%) | 0.000 ns | 92.34 KiB (1%) | 18 |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\")"]` | 78.035 μs (25%) | 0.000 ns | 92.34 KiB (1%) | 18 |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\", \"sizehint!\")"]` | 68.385 μs (25%) | 0.000 ns | 86.13 KiB (1%) | 12 |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"iterator\")"]` | 126.375 μs (25%) | 0.000 ns | 96.22 KiB (1%) | 445 |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\")"]` | 123.588 μs (25%) | 0.000 ns | 95.38 KiB (1%) | 441 |
| `["collection", "initialization", "(\"IdDict\", \"Any\", \"loop\", \"sizehint!\")"]` | 106.389 μs (25%) | 0.000 ns | 87.38 KiB (1%) | 437 |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"iterator\")"]` | 62.115 μs (25%) | 0.000 ns | 39.42 KiB (1%) | 959 |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\")"]` | 62.490 μs (25%) | 0.000 ns | 39.42 KiB (1%) | 959 |
| `["collection", "initialization", "(\"IdDict\", \"Int\", \"loop\", \"sizehint!\")"]` | 49.584 μs (25%) | 0.000 ns | 31.42 KiB (1%) | 955 |
| `["collection", "initialization", "(\"IdDict\", \"String\", \"iterator\")"]` | 84.928 μs (25%) | 0.000 ns | 88.63 KiB (1%) | 9 |
| `["collection", "initialization", "(\"IdDict\", \"String\", \"loop\")"]` | 85.493 μs (25%) | 0.000 ns | 88.63 KiB (1%) | 9 |
| `["collection", "initialization", "(\"IdDict\", \"String\", \"loop\", \"sizehint!\")"]` | 66.964 μs (25%) | 0.000 ns | 80.63 KiB (1%) | 5 |
| `["collection", "initialization", "(\"Set\", \"Any\", \"iterator\")"]` | 102.366 μs (25%) | 0.000 ns | 71.26 KiB (1%) | 1631 |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\")"]` | 121.098 μs (25%) | 0.000 ns | 79.63 KiB (1%) | 1939 |
| `["collection", "initialization", "(\"Set\", \"Any\", \"loop\", \"sizehint!\")"]` | 102.801 μs (25%) | 0.000 ns | 71.26 KiB (1%) | 1631 |
| `["collection", "initialization", "(\"Set\", \"Int\", \"iterator\")"]` | 12.781 μs (25%) | 0.000 ns | 9.62 KiB (1%) | 8 |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\")"]` | 15.391 μs (25%) | 0.000 ns | 13.27 KiB (1%) | 14 |
| `["collection", "initialization", "(\"Set\", \"Int\", \"loop\", \"sizehint!\")"]` | 12.888 μs (25%) | 0.000 ns | 9.62 KiB (1%) | 8 |
| `["collection", "initialization", "(\"Set\", \"String\", \"iterator\")"]` | 54.910 μs (25%) | 0.000 ns | 45.96 KiB (1%) | 12 |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\")"]` | 62.301 μs (25%) | 0.000 ns | 49.61 KiB (1%) | 18 |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\", \"sizehint!\")"]` | 54.532 μs (25%) | 0.000 ns | 45.96 KiB (1%) | 12 |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"iterator\")"]` | 1.173 μs (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\")"]` | 7.491 μs (25%) | 0.000 ns | 16.45 KiB (1%) | 10 |
| `["collection", "initialization", "(\"Vector\", \"Any\", \"loop\", \"sizehint!\")"]` | 6.776 μs (25%) | 0.000 ns | 7.95 KiB (1%) | 2 |
| `["collection", "initialization", "(\"Vector\", \"Int\", \"iterator\")"]` | 971.000 ns (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["collection", "initialization", "(\"Vector\", \"Int\", \"loop\")"]` | 6.152 μs (25%) | 0.000 ns | 16.45 KiB (1%) | 10 |
| `["collection", "initialization", "(\"Vector\", \"Int\", \"loop\", \"sizehint!\")"]` | 4.924 μs (25%) | 0.000 ns | 7.95 KiB (1%) | 2 |
| `["collection", "initialization", "(\"Vector\", \"String\", \"iterator\")"]` | 1.054 μs (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\")"]` | 7.355 μs (25%) | 0.000 ns | 16.45 KiB (1%) | 10 |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\", \"sizehint!\")"]` | 6.675 μs (25%) | 0.000 ns | 7.95 KiB (1%) | 2 |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"iterate second\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"BitSet\", \"Int\", \"iterate\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate second\")"]` | 42.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"Dict\", \"Any\", \"iterate\")"]` | 28.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"iterate second\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Dict\", \"Int\", \"iterate\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate second\")"]` | 28.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"Dict\", \"String\", \"iterate\")"]` | 26.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"iterate second\")"]` | 27.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"IdDict\", \"Any\", \"iterate\")"]` | 41.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"IdDict\", \"Int\", \"iterate second\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"IdDict\", \"Int\", \"iterate\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate second\")"]` | 30.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"IdDict\", \"String\", \"iterate\")"]` | 39.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"Set\", \"Any\", \"iterate second\")"]` | 206.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Set\", \"Any\", \"iterate\")"]` | 191.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Set\", \"Int\", \"iterate second\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Set\", \"Int\", \"iterate\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Set\", \"String\", \"iterate second\")"]` | 26.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Set\", \"String\", \"iterate\")"]` | 26.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"iterate second\")"]` | 177.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Vector\", \"Any\", \"iterate\")"]` | 174.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"iterate second\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Vector\", \"Int\", \"iterate\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Vector\", \"String\", \"iterate second\")"]` | 18.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Vector\", \"String\", \"iterate\")"]` | 21.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "optimizations", "(\"BitSet\", \"Int8\")"]` | 158.847 μs (25%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["collection", "optimizations", "(\"BitSet\", \"UInt16\")"]` | 160.675 μs (25%) | 0.000 ns | 23.34 KiB (1%) | 6 |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Bool\")"]` | 723.519 μs (25%) | 0.000 ns | 416 bytes (1%) | 4 |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Int8\")"]` | 1.232 ms (25%) | 0.000 ns | 2.05 KiB (1%) | 10 |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"Nothing\")"]` | 1.667 ms (25%) | 0.000 ns | 352 bytes (1%) | 4 |
| `["collection", "optimizations", "(\"Dict\", \"abstract\", \"UInt16\")"]` | 2.463 ms (25%) | 0.000 ns | 1.67 MiB (1%) | 34 |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Bool\")"]` | 723.975 μs (25%) | 0.000 ns | 416 bytes (1%) | 4 |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Int8\")"]` | 1.227 ms (25%) | 0.000 ns | 2.05 KiB (1%) | 10 |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"Nothing\")"]` | 1.667 ms (25%) | 0.000 ns | 352 bytes (1%) | 4 |
| `["collection", "optimizations", "(\"Dict\", \"concrete\", \"UInt16\")"]` | 2.460 ms (25%) | 0.000 ns | 1.67 MiB (1%) | 34 |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"Bool\")"]` | 2.873 ms (25%) | 0.000 ns | 432 bytes (1%) | 2 |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"Int8\")"]` | 3.419 ms (25%) | 0.000 ns | 8.42 KiB (1%) | 6 |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"Nothing\")"]` | 2.446 ms (25%) | 0.000 ns | 432 bytes (1%) | 2 |
| `["collection", "optimizations", "(\"IdDict\", \"abstract\", \"UInt16\")"]` | 8.795 ms (25%) | 0.000 ns | 4.34 MiB (1%) | 196843 |
| `["collection", "optimizations", "(\"IdDict\", \"concrete\", \"Bool\")"]` | 2.719 ms (25%) | 0.000 ns | 432 bytes (1%) | 2 |
| `["collection", "optimizations", "(\"IdDict\", \"concrete\", \"Int8\")"]` | 3.417 ms (25%) | 0.000 ns | 8.42 KiB (1%) | 6 |
| `["collection", "optimizations", "(\"IdDict\", \"concrete\", \"Nothing\")"]` | 2.335 ms (25%) | 0.000 ns | 432 bytes (1%) | 2 |
| `["collection", "optimizations", "(\"IdDict\", \"concrete\", \"UInt16\")"]` | 8.761 ms (25%) | 0.000 ns | 4.34 MiB (1%) | 196843 |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Bool\")"]` | 723.809 μs (25%) | 0.000 ns | 400 bytes (1%) | 5 |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Int8\")"]` | 1.234 ms (25%) | 0.000 ns | 1.05 KiB (1%) | 8 |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Nothing\")"]` | 122.000 ns (25%) | 0.000 ns | 368 bytes (1%) | 5 |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"UInt16\")"]` | 2.099 ms (25%) | 0.000 ns | 960.88 KiB (1%) | 13 |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Bool\")"]` | 724.019 μs (25%) | 0.000 ns | 400 bytes (1%) | 5 |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Int8\")"]` | 1.234 ms (25%) | 0.000 ns | 1.05 KiB (1%) | 8 |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"Nothing\")"]` | 321.000 ns (25%) | 0.000 ns | 368 bytes (1%) | 5 |
| `["collection", "optimizations", "(\"Set\", \"concrete\", \"UInt16\")"]` | 2.135 ms (25%) | 0.000 ns | 960.88 KiB (1%) | 13 |
| `["collection", "optimizations", "(\"Vector\", \"abstract\", \"Nothing\")"]` | 40.000 ns (25%) | 0.000 ns | 80 bytes (1%) | 1 |
| `["collection", "optimizations", "(\"Vector\", \"concrete\", \"Nothing\")"]` | 262.000 ns (25%) | 0.000 ns | 80 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"first\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"false\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"in\", \"true\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"last\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"length\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"pop!\", \"specified\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"pop!\", \"unspecified\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"push!\", \"new\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"push!\", \"overwrite\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"getindex\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"in\", \"false\")"]` | 94.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"in\", \"true\")"]` | 50.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"specified\")"]` | 85.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 214.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"new\")"]` | 133.000 ns (25%) | 0.000 ns | 80 bytes (1%) | 5 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"push!\", \"overwrite\")"]` | 52.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"new\")"]` | 134.000 ns (25%) | 0.000 ns | 80 bytes (1%) | 5 |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"setindex!\", \"overwrite\")"]` | 54.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"first\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"getindex\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"in\", \"false\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"in\", \"true\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"length\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"specified\")"]` | 31.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"unspecified\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"push!\", \"new\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"push!\", \"overwrite\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"setindex!\", \"new\")"]` | 25.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"setindex!\", \"overwrite\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"getindex\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"in\", \"false\")"]` | 49.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"in\", \"true\")"]` | 44.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"specified\")"]` | 84.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"unspecified\")"]` | 64.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"push!\", \"new\")"]` | 64.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"push!\", \"overwrite\")"]` | 52.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"setindex!\", \"new\")"]` | 62.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"setindex!\", \"overwrite\")"]` | 49.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"getindex\")"]` | 48.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"in\", \"false\")"]` | 50.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"in\", \"true\")"]` | 66.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"pop!\", \"specified\")"]` | 97.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"push!\", \"new\")"]` | 68.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"push!\", \"overwrite\")"]` | 68.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"setindex!\", \"new\")"]` | 68.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Any\", \"setindex!\", \"overwrite\")"]` | 66.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"first\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"getindex\")"]` | 48.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"in\", \"false\")"]` | 52.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"in\", \"true\")"]` | 47.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"length\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"pop!\", \"specified\")"]` | 92.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"push!\", \"new\")"]` | 68.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"push!\", \"overwrite\")"]` | 62.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"new\")"]` | 67.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"Int\", \"setindex!\", \"overwrite\")"]` | 63.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"getindex\")"]` | 42.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"in\", \"false\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"in\", \"true\")"]` | 44.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"pop!\", \"specified\")"]` | 78.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"push!\", \"new\")"]` | 53.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"push!\", \"overwrite\")"]` | 54.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"setindex!\", \"new\")"]` | 52.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"IdDict\", \"String\", \"setindex!\", \"overwrite\")"]` | 53.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"false\")"]` | 88.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"in\", \"true\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"specified\")"]` | 52.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 191.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"new\")"]` | 105.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 4 |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 31.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"first\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"in\", \"false\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"in\", \"true\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"length\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"specified\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"unspecified\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"push!\", \"new\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"push!\", \"overwrite\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"false\")"]` | 47.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"true\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"specified\")"]` | 70.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"unspecified\")"]` | 67.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"new\")"]` | 57.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"overwrite\")"]` | 47.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"getindex\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"false\")"]` | 34.019 μs (25%) | 0.000 ns | 15.63 KiB (1%) | 1000 |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"in\", \"true\")"]` | 29.375 μs (25%) | 0.000 ns | 13.52 KiB (1%) | 865 |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"pop!\", \"unspecified\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"push!\")"]` | 713.000 ns (25%) | 0.000 ns | 15.70 KiB (1%) | 2 |
| `["collection", "queries & updates", "(\"Vector\", \"Any\", \"setindex!\")"]` | 19.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"first\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"getindex\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"in\", \"false\")"]` | 376.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"in\", \"true\")"]` | 146.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"last\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"length\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"pop!\", \"unspecified\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"push!\")"]` | 683.000 ns (25%) | 0.000 ns | 15.69 KiB (1%) | 1 |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"setindex!\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"getindex\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 959.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 404.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"pop!\", \"unspecified\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"push!\")"]` | 677.000 ns (25%) | 0.000 ns | 15.69 KiB (1%) | 1 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"setindex!\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"<\", \"BitSet\")"]` | 119.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"==\", \"BitSet\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"==\", \"self\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"big\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"small\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\")"]` | 93.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\")"]` | 111.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 123.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\")"]` | 325.000 ns (25%) | 0.000 ns | 736 bytes (1%) | 7 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 481.000 ns (25%) | 0.000 ns | 768 bytes (1%) | 9 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\")"]` | 243.000 ns (25%) | 0.000 ns | 656 bytes (1%) | 6 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 492.000 ns (25%) | 0.000 ns | 1.80 KiB (1%) | 12 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Set\")"]` | 140.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"Vector\")"]` | 56.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"big\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"small\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"BitSet\")"]` | 106.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Set\")"]` | 217.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff\", \"Vector\")"]` | 132.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"BitSet\")"]` | 61.000 ns (25%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"Set\")"]` | 321.000 ns (25%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"Vector\")"]` | 222.000 ns (25%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"big\")"]` | 2.016 μs (25%) | 0.000 ns | 128.06 KiB (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff!\", \"small\")"]` | 2.405 μs (25%) | 0.000 ns | 32.13 KiB (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\")"]` | 93.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\")"]` | 144.000 ns (25%) | 0.000 ns | 672 bytes (1%) | 6 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 612.000 ns (25%) | 0.000 ns | 720 bytes (1%) | 8 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\")"]` | 405.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 677.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\")"]` | 309.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 481.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"BitSet\")"]` | 60.000 ns (25%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Set\")"]` | 220.000 ns (25%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"Vector\")"]` | 129.000 ns (25%) | 0.000 ns | 336 bytes (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"big\")"]` | 2.057 μs (25%) | 0.000 ns | 128.06 KiB (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union!\", \"small\")"]` | 2.415 μs (25%) | 0.000 ns | 32.13 KiB (1%) | 1 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\")"]` | 92.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\")"]` | 139.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 207.000 ns (25%) | 0.000 ns | 672 bytes (1%) | 6 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\")"]` | 297.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 477.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\")"]` | 206.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 267.000 ns (25%) | 0.000 ns | 640 bytes (1%) | 5 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"BitSet\")"]` | 120.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"Set\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"Vector\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"⊆\", \"self\")"]` | 121.000 ns (25%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"<\", \"Set\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"Set\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"==\", \"self\")"]` | 5.029 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\")"]` | 919.000 ns (25%) | 0.000 ns | 9.44 KiB (1%) | 5 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\")"]` | 609.000 ns (25%) | 0.000 ns | 1.34 KiB (1%) | 9 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 694.000 ns (25%) | 0.000 ns | 1.38 KiB (1%) | 11 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\")"]` | 586.000 ns (25%) | 0.000 ns | 1.34 KiB (1%) | 9 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 728.000 ns (25%) | 0.000 ns | 1.38 KiB (1%) | 11 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\")"]` | 501.000 ns (25%) | 0.000 ns | 1.34 KiB (1%) | 9 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 1.263 μs (25%) | 0.000 ns | 3.68 KiB (1%) | 22 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 382.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Set\")"]` | 387.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff!\", \"Vector\")"]` | 290.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"BitSet\")"]` | 1.227 μs (25%) | 0.000 ns | 9.44 KiB (1%) | 5 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Set\")"]` | 1.241 μs (25%) | 0.000 ns | 9.44 KiB (1%) | 5 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"setdiff\", \"Vector\")"]` | 1.209 μs (25%) | 0.000 ns | 9.44 KiB (1%) | 5 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\")"]` | 873.000 ns (25%) | 0.000 ns | 9.44 KiB (1%) | 5 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\")"]` | 14.427 μs (25%) | 0.000 ns | 13.30 KiB (1%) | 15 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 15.837 μs (25%) | 0.000 ns | 13.34 KiB (1%) | 17 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\")"]` | 14.489 μs (25%) | 0.000 ns | 13.27 KiB (1%) | 14 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 15.147 μs (25%) | 0.000 ns | 13.27 KiB (1%) | 14 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\")"]` | 14.362 μs (25%) | 0.000 ns | 13.30 KiB (1%) | 15 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 15.497 μs (25%) | 0.000 ns | 13.34 KiB (1%) | 17 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"BitSet\")"]` | 444.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Set\")"]` | 380.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union!\", \"Vector\")"]` | 284.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\")"]` | 898.000 ns (25%) | 0.000 ns | 9.44 KiB (1%) | 5 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\")"]` | 8.712 μs (25%) | 0.000 ns | 9.65 KiB (1%) | 9 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 9.191 μs (25%) | 0.000 ns | 9.65 KiB (1%) | 9 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\")"]` | 8.666 μs (25%) | 0.000 ns | 9.62 KiB (1%) | 8 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 9.012 μs (25%) | 0.000 ns | 9.62 KiB (1%) | 8 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\")"]` | 8.517 μs (25%) | 0.000 ns | 9.65 KiB (1%) | 9 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 8.947 μs (25%) | 0.000 ns | 9.65 KiB (1%) | 9 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"BitSet\")"]` | 29.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Set\")"]` | 31.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"Vector\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Set\", \"Int\", \"⊆\", \"self\")"]` | 4.917 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\")"]` | 19.678 μs (25%) | 0.000 ns | 29.73 KiB (1%) | 25 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\")"]` | 44.166 μs (25%) | 0.000 ns | 10.01 KiB (1%) | 15 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"BitSet\", \"BitSet\")"]` | 45.155 μs (25%) | 0.000 ns | 10.07 KiB (1%) | 18 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\")"]` | 49.454 μs (25%) | 0.000 ns | 10.01 KiB (1%) | 15 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Set\", \"Set\")"]` | 50.734 μs (25%) | 0.000 ns | 10.07 KiB (1%) | 18 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\")"]` | 50.660 μs (25%) | 0.000 ns | 12.33 KiB (1%) | 27 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"intersect\", \"Vector\", \"Vector\")"]` | 52.203 μs (25%) | 0.000 ns | 14.65 KiB (1%) | 39 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"BitSet\")"]` | 41.625 μs (25%) | 0.000 ns | 26.09 KiB (1%) | 19 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Set\")"]` | 41.678 μs (25%) | 0.000 ns | 26.09 KiB (1%) | 19 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"setdiff\", \"Vector\")"]` | 42.267 μs (25%) | 0.000 ns | 26.10 KiB (1%) | 20 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\")"]` | 47.109 μs (25%) | 0.000 ns | 21.22 KiB (1%) | 16 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\")"]` | 50.856 μs (25%) | 0.000 ns | 21.73 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"BitSet\", \"BitSet\")"]` | 52.808 μs (25%) | 0.000 ns | 21.73 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\")"]` | 50.747 μs (25%) | 0.000 ns | 21.73 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Set\", \"Set\")"]` | 52.487 μs (25%) | 0.000 ns | 21.73 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\")"]` | 49.347 μs (25%) | 0.000 ns | 21.67 KiB (1%) | 24 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"symdiff\", \"Vector\", \"Vector\")"]` | 51.823 μs (25%) | 0.000 ns | 21.73 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\")"]` | 19.521 μs (25%) | 0.000 ns | 29.73 KiB (1%) | 25 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\")"]` | 20.116 μs (25%) | 0.000 ns | 29.77 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"BitSet\", \"BitSet\")"]` | 20.430 μs (25%) | 0.000 ns | 29.77 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\")"]` | 20.047 μs (25%) | 0.000 ns | 29.77 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Set\", \"Set\")"]` | 20.341 μs (25%) | 0.000 ns | 29.77 KiB (1%) | 26 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\")"]` | 19.947 μs (25%) | 0.000 ns | 29.73 KiB (1%) | 25 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"union\", \"Vector\", \"Vector\")"]` | 20.400 μs (25%) | 0.000 ns | 29.73 KiB (1%) | 25 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"BitSet\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"Set\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"Vector\", \"Int\", \"⊆\", \"Vector\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"empty\", \"Int\", \"<\", \"BitSet\")"]` | 83.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["collection", "set operations", "(\"empty\", \"Int\", \"<\", \"Set\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "set operations", "(\"empty\", \"Int\", \"⊆\", \"BitSet\")"]` | 72.000 ns (25%) | 0.000 ns | 160 bytes (1%) | 3 |
| `["collection", "set operations", "(\"empty\", \"Int\", \"⊆\", \"Set\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "day"]` | 12.851 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "hour"]` | 4.132 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "millisecond"]` | 2.070 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "minute"]` | 4.127 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "month"]` | 10.884 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "second"]` | 4.129 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "accessor", "year"]` | 9.670 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Day\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Hour\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Millisecond\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Minute\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Month\")"]` | 69.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Second\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"DateTime\", \"Year\")"]` | 59.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"Date\", \"Day\")"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "arithmetic", "(\"Date\", \"Year\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "construction", "Date"]` | 5.664 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "construction", "DateTime"]` | 5.923 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "conversion", "Date -> DateTime"]` | 1.297 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "conversion", "DateTime -> Date"]` | 2.068 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "parse", "(\"DateTime\", \"DateFormat\")"]` | 18.345 μs (5%) | 0.000 ns | 6.11 KiB (1%) | 119 |
| `["dates", "parse", "(\"DateTime\", \"ISODateTimeFormat\")"]` | 134.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Lowercase\")"]` | 350.000 ns (5%) | 0.000 ns | 256 bytes (1%) | 6 |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Mixedcase\")"]` | 464.000 ns (5%) | 0.000 ns | 512 bytes (1%) | 11 |
| `["dates", "parse", "(\"DateTime\", \"RFC1123Format\", \"Titlecase\")"]` | 356.000 ns (5%) | 0.000 ns | 256 bytes (1%) | 6 |
| `["dates", "parse", "(\"Date\", \"DateFormat\")"]` | 14.480 μs (5%) | 0.000 ns | 3.08 KiB (1%) | 61 |
| `["dates", "parse", "(\"Date\", \"ISODateFormat\")"]` | 97.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "parse", "Date"]` | 58.290 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "parse", "DateTime"]` | 90.610 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofweek\", \"DateTime\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofweek\", \"Date\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofweekofmonth\", \"DateTime\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofweekofmonth\", \"Date\")"]` | 29.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofyear\", \"DateTime\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"dayofyear\", \"Date\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"daysofweekinmonth\", \"DateTime\")"]` | 43.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"daysofweekinmonth\", \"Date\")"]` | 39.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofmonth\", \"DateTime\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofmonth\", \"Date\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofweek\", \"DateTime\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"firstdayofweek\", \"Date\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"isleapyear\", \"DateTime\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"isleapyear\", \"Date\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofmonth\", \"DateTime\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofmonth\", \"Date\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofweek\", \"DateTime\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "query", "(\"lastdayofweek\", \"Date\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["dates", "string", "Date"]` | 209.642 ns (5%) | 0.000 ns | 352 bytes (1%) | 8 |
| `["dates", "string", "DateTime"]` | 629.722 ns (5%) | 0.000 ns | 1008 bytes (1%) | 18 |
| `["find", "findall", "(\"Array{Bool,1}\", \"10-90\")"]` | 918.000 ns (5%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["find", "findall", "(\"Array{Bool,1}\", \"50-50\")"]` | 1.125 μs (5%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["find", "findall", "(\"Array{Bool,1}\", \"90-10\")"]` | 1.208 μs (5%) | 0.000 ns | 7.19 KiB (1%) | 1 |
| `["find", "findall", "(\"BitArray{1}\", \"10-90\")"]` | 678.000 ns (5%) | 0.000 ns | 896 bytes (1%) | 1 |
| `["find", "findall", "(\"BitArray{1}\", \"50-50\")"]` | 918.000 ns (5%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["find", "findall", "(\"BitArray{1}\", \"90-10\")"]` | 841.000 ns (5%) | 0.000 ns | 7.19 KiB (1%) | 1 |
| `["find", "findall", "(\"ispos\", \"Array{Bool,1}\")"]` | 4.129 μs (5%) | 0.000 ns | 8.53 KiB (1%) | 13 |
| `["find", "findall", "(\"ispos\", \"Array{Float32,1}\")"]` | 6.947 μs (5%) | 0.000 ns | 16.59 KiB (1%) | 14 |
| `["find", "findall", "(\"ispos\", \"Array{Float64,1}\")"]` | 7.123 μs (5%) | 0.000 ns | 16.59 KiB (1%) | 14 |
| `["find", "findall", "(\"ispos\", \"Array{Int64,1}\")"]` | 4.933 μs (5%) | 0.000 ns | 16.59 KiB (1%) | 14 |
| `["find", "findall", "(\"ispos\", \"Array{Int8,1}\")"]` | 4.131 μs (5%) | 0.000 ns | 8.53 KiB (1%) | 13 |
| `["find", "findall", "(\"ispos\", \"Array{UInt64,1}\")"]` | 7.070 μs (5%) | 0.000 ns | 16.59 KiB (1%) | 14 |
| `["find", "findall", "(\"ispos\", \"Array{UInt8,1}\")"]` | 6.906 μs (5%) | 0.000 ns | 16.59 KiB (1%) | 14 |
| `["find", "findnext", "(\"Array{Bool,1}\", \"50-50\")"]` | 579.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findnext", "(\"BitArray{1}\", \"10-90\")"]` | 659.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findnext", "(\"BitArray{1}\", \"50-50\")"]` | 3.287 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findnext", "(\"BitArray{1}\", \"90-10\")"]` | 5.803 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findnext", "(\"ispos\", \"Array{Bool,1}\")"]` | 13.480 μs (5%) | 0.000 ns | 7.72 KiB (1%) | 494 |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 20.124 μs (5%) | 0.000 ns | 15.30 KiB (1%) | 979 |
| `["find", "findnext", "(\"ispos\", \"Array{Float64,1}\")"]` | 19.846 μs (5%) | 0.000 ns | 15.30 KiB (1%) | 979 |
| `["find", "findnext", "(\"ispos\", \"Array{Int64,1}\")"]` | 14.156 μs (5%) | 0.000 ns | 8.22 KiB (1%) | 526 |
| `["find", "findnext", "(\"ispos\", \"Array{Int8,1}\")"]` | 13.451 μs (5%) | 0.000 ns | 7.86 KiB (1%) | 503 |
| `["find", "findnext", "(\"ispos\", \"Array{UInt64,1}\")"]` | 20.771 μs (5%) | 0.000 ns | 15.30 KiB (1%) | 979 |
| `["find", "findnext", "(\"ispos\", \"Array{UInt8,1}\")"]` | 20.084 μs (5%) | 0.000 ns | 15.27 KiB (1%) | 977 |
| `["find", "findprev", "(\"Array{Bool,1}\", \"50-50\")"]` | 661.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findprev", "(\"BitArray{1}\", \"10-90\")"]` | 704.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findprev", "(\"BitArray{1}\", \"50-50\")"]` | 3.181 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findprev", "(\"BitArray{1}\", \"90-10\")"]` | 5.487 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["find", "findprev", "(\"ispos\", \"Array{Bool,1}\")"]` | 15.718 μs (5%) | 0.000 ns | 7.73 KiB (1%) | 495 |
| `["find", "findprev", "(\"ispos\", \"Array{Float32,1}\")"]` | 20.544 μs (5%) | 0.000 ns | 15.28 KiB (1%) | 978 |
| `["find", "findprev", "(\"ispos\", \"Array{Float64,1}\")"]` | 23.828 μs (5%) | 0.000 ns | 15.28 KiB (1%) | 978 |
| `["find", "findprev", "(\"ispos\", \"Array{Int64,1}\")"]` | 13.954 μs (5%) | 0.000 ns | 8.22 KiB (1%) | 526 |
| `["find", "findprev", "(\"ispos\", \"Array{Int8,1}\")"]` | 12.921 μs (5%) | 0.000 ns | 7.86 KiB (1%) | 503 |
| `["find", "findprev", "(\"ispos\", \"Array{UInt64,1}\")"]` | 19.175 μs (5%) | 0.000 ns | 15.28 KiB (1%) | 978 |
| `["find", "findprev", "(\"ispos\", \"Array{UInt8,1}\")"]` | 18.947 μs (5%) | 0.000 ns | 15.25 KiB (1%) | 976 |
| `["io", "read", "read"]` | 6.187 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["io", "read", "readstring"]` | 30.207 ns (5%) | 0.000 ns | 96 bytes (1%) | 2 |
| `["io", "serialization", "(\"deserialize\", \"Matrix{Float64}\")"]` | 649.000 μs (5%) | 0.000 ns | 7.63 MiB (1%) | 25 |
| `["io", "serialization", "(\"deserialize\", \"Vector{String}\")"]` | 88.523 μs (5%) | 0.000 ns | 122.28 KiB (1%) | 2992 |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 4.020 ms (5%) | 0.000 ns | 7.63 MiB (1%) | 12 |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 60.558 μs (5%) | 0.000 ns | 71.67 KiB (1%) | 22 |
| `["io", "skipchars"]` | 21.198 ms (5%) | 0.000 ns | 1.95 KiB (1%) | 29 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 64.250 ms (45%) | 13.805 ms | 24.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 923.267 μs (45%) | 0.000 ns | 1.50 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Vector\", 1024)"]` | 1.114 ms (45%) | 0.000 ns | 8.01 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"Bidiagonal\", \"Vector\", 256)"]` | 54.986 μs (45%) | 0.000 ns | 514.20 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 1024)"]` | 864.000 ns (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Diagonal\", 256)"]` | 409.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 1024)"]` | 938.000 ns (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Diagonal\", \"Vector\", 256)"]` | 304.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 29.185 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 696.994 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"Vector\", 1024)"]` | 113.575 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"LowerTriangular\", \"Vector\", 256)"]` | 9.196 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Matrix\", 1024)"]` | 47.914 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Matrix\", 256)"]` | 833.059 μs (45%) | 0.000 ns | 512.08 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Vector\", 1024)"]` | 226.710 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Matrix\", \"Vector\", 256)"]` | 11.576 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 64.069 ms (45%) | 13.554 ms | 24.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 924.405 μs (45%) | 0.000 ns | 1.50 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"Vector\", 1024)"]` | 1.297 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"SymTridiagonal\", \"Vector\", 256)"]` | 480.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 63.856 ms (45%) | 13.654 ms | 24.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 923.612 μs (45%) | 0.000 ns | 1.50 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 1024)"]` | 1.459 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"Tridiagonal\", \"Vector\", 256)"]` | 512.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 29.536 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 721.845 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"Vector\", 1024)"]` | 141.857 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"*\", \"UpperTriangular\", \"Vector\", 256)"]` | 9.152 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.823 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 765.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 1024)"]` | 886.000 ns (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"Diagonal\", \"Diagonal\", 256)"]` | 394.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.156 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 50.095 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 1024)"]` | 1.153 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"Matrix\", \"Matrix\", 256)"]` | 49.607 μs (45%) | 0.000 ns | 512.08 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.827 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 757.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 2.797 μs (45%) | 0.000 ns | 24.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"+\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.313 μs (45%) | 0.000 ns | 6.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.153 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 49.080 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 1024)"]` | 824.000 ns (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 391.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 1024)"]` | 1.914 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Bidiagonal\", \"Bidiagonal\", 256)"]` | 772.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 1024)"]` | 897.000 ns (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"Diagonal\", \"Diagonal\", 256)"]` | 301.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 1.155 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 50.322 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 1024)"]` | 1.157 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"Matrix\", \"Matrix\", 256)"]` | 49.512 μs (45%) | 0.000 ns | 512.08 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 1024)"]` | 1.960 μs (45%) | 0.000 ns | 16.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"SymTridiagonal\", \"SymTridiagonal\", 256)"]` | 791.000 ns (45%) | 0.000 ns | 4.28 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 1024)"]` | 2.736 μs (45%) | 0.000 ns | 24.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"-\", \"Tridiagonal\", \"Tridiagonal\", 256)"]` | 1.239 μs (45%) | 0.000 ns | 6.42 KiB (1%) | 4 |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 1.155 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 49.709 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 1024)"]` | 814.000 ns (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"-\", \"Vector\", \"Vector\", 256)"]` | 314.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 1024)"]` | 2.103 μs (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"/\", \"Diagonal\", \"Diagonal\", 256)"]` | 688.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"/\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 33.412 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"/\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 937.019 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 1024)"]` | 113.695 ms (45%) | 14.734 ms | 24.01 MiB (1%) | 10 |
| `["linalg", "arithmetic", "(\"/\", \"Matrix\", \"Matrix\", 256)"]` | 2.513 ms (45%) | 0.000 ns | 1.50 MiB (1%) | 10 |
| `["linalg", "arithmetic", "(\"/\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 28.312 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"/\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 674.401 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Bidiagonal\", \"Vector\", 1024)"]` | 6.918 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Bidiagonal\", \"Vector\", 256)"]` | 1.854 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 1024)"]` | 2.106 μs (45%) | 0.000 ns | 8.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Diagonal\", 256)"]` | 681.000 ns (45%) | 0.000 ns | 2.14 KiB (1%) | 2 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 1024)"]` | 2.120 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Diagonal\", \"Vector\", 256)"]` | 661.000 ns (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 1024)"]` | 654.208 μs (45%) | 0.000 ns | 600.38 KiB (1%) | 62 |
| `["linalg", "arithmetic", "(\"\\\\\", \"HermitianSparseWithNonZeroPivots\", \"Vector\", 256)"]` | 152.213 μs (45%) | 0.000 ns | 149.58 KiB (1%) | 62 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"LowerTriangular\", 1024)"]` | 32.084 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"LowerTriangular\", 256)"]` | 850.813 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"Vector\", 1024)"]` | 510.838 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"LowerTriangular\", \"Vector\", 256)"]` | 33.329 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Matrix\", 1024)"]` | 87.458 ms (45%) | 0.000 ns | 16.01 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Matrix\", 256)"]` | 2.250 ms (45%) | 0.000 ns | 1.00 MiB (1%) | 6 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Vector\", 1024)"]` | 25.221 ms (45%) | 0.000 ns | 8.02 MiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Matrix\", \"Vector\", 256)"]` | 689.123 μs (45%) | 0.000 ns | 516.36 KiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"SymTridiagonal\", \"Vector\", 1024)"]` | 17.195 μs (45%) | 0.000 ns | 24.42 KiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"SymTridiagonal\", \"Vector\", 256)"]` | 4.795 μs (45%) | 0.000 ns | 6.42 KiB (1%) | 5 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Tridiagonal\", \"Vector\", 1024)"]` | 27.519 μs (45%) | 0.000 ns | 48.88 KiB (1%) | 9 |
| `["linalg", "arithmetic", "(\"\\\\\", \"Tridiagonal\", \"Vector\", 256)"]` | 7.613 μs (45%) | 0.000 ns | 12.88 KiB (1%) | 9 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"UpperTriangular\", 1024)"]` | 32.119 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"UpperTriangular\", 256)"]` | 861.876 μs (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"Vector\", 1024)"]` | 530.320 μs (45%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"\\\\\", \"UpperTriangular\", \"Vector\", 256)"]` | 32.744 μs (45%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 1024)"]` | 1.064 μs (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float32, 256)"]` | 287.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 1024)"]` | 1.056 μs (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Float64, 256)"]` | 286.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 1024)"]` | 541.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int32, 256)"]` | 158.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 1024)"]` | 397.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"cumsum!\", Int64, 256)"]` | 120.000 ns (45%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "arithmetic", "(\"exp\", \"Hermitian\", 1024)"]` | 994.046 ms (45%) | 28.472 ms | 80.82 MiB (1%) | 24 |
| `["linalg", "arithmetic", "(\"exp\", \"Hermitian\", 256)"]` | 21.198 ms (45%) | 0.000 ns | 5.21 MiB (1%) | 24 |
| `["linalg", "arithmetic", "(\"log\", \"Hermitian\", 1024)"]` | 1.008 s (45%) | 29.371 ms | 80.85 MiB (1%) | 24 |
| `["linalg", "arithmetic", "(\"log\", \"Hermitian\", 256)"]` | 21.229 ms (45%) | 0.000 ns | 5.21 MiB (1%) | 24 |
| `["linalg", "arithmetic", "(\"mul!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 1024)"]` | 747.415 ms (45%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["linalg", "arithmetic", "(\"mul!\", \"Matrix{Float32}\", \"Matrix{Float64}\", \"Matrix{Float64}\", 256)"]` | 11.149 ms (45%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["linalg", "arithmetic", "(\"sqrt\", \"Hermitian\", 1024)"]` | 997.128 ms (45%) | 28.379 ms | 80.85 MiB (1%) | 24 |
| `["linalg", "arithmetic", "(\"sqrt\", \"Hermitian\", 256)"]` | 21.186 ms (45%) | 0.000 ns | 5.21 MiB (1%) | 24 |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.002 s (45%) | 0.000 ns | 16.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 256)"]` | 5.221 ms (45%) | 0.000 ns | 1.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 1024)"]` | 592.632 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"UnitUpperTriangular\", 256)"]` | 3.690 ms (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 599.193 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 256)"]` | 3.818 ms (45%) | 0.000 ns | 512.09 KiB (1%) | 3 |
| `["linalg", "blas", "asum"]` | 135.928 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "axpy!"]` | 197.455 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "blascopy!"]` | 137.997 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "dot"]` | 100.389 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "dotc"]` | 234.818 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "dotu"]` | 234.788 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gbmv!"]` | 193.274 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gbmv"]` | 197.822 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "gemm!"]` | 47.713 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gemm"]` | 48.058 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "gemv!"]` | 243.136 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "gemv"]` | 231.634 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "ger!"]` | 725.125 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "her!"]` | 1.922 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "herk!"]` | 112.076 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "herk"]` | 113.020 ms (40%) | 0.000 ns | 16.00 MiB (1%) | 2 |
| `["linalg", "blas", "nrm2"]` | 270.211 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "sbmv!"]` | 197.516 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "sbmv"]` | 198.720 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "scal!"]` | 212.764 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "scal"]` | 967.000 ns (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "symm!"]` | 47.671 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "symm"]` | 47.854 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "symv!"]` | 113.383 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "symv"]` | 114.082 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "syr!"]` | 536.722 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "syrk!"]` | 28.446 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "syrk"]` | 28.818 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "trmm!"]` | 28.275 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trmm"]` | 29.355 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "trmv!"]` | 114.295 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trmv"]` | 111.821 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "blas", "trsm!"]` | 30.815 ms (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trsm"]` | 31.748 ms (40%) | 0.000 ns | 8.00 MiB (1%) | 2 |
| `["linalg", "blas", "trsv!"]` | 114.420 μs (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["linalg", "blas", "trsv"]` | 111.654 μs (40%) | 0.000 ns | 8.13 KiB (1%) | 1 |
| `["linalg", "factorization", "(\"cholesky\", \"Matrix\", 1024)"]` | 16.102 ms (45%) | 0.000 ns | 8.00 MiB (1%) | 6 |
| `["linalg", "factorization", "(\"cholesky\", \"Matrix\", 256)"]` | 442.174 μs (45%) | 0.000 ns | 512.19 KiB (1%) | 6 |
| `["linalg", "factorization", "(\"eigen\", \"Bidiagonal\", 1024)"]` | 5.263 ms (45%) | 0.000 ns | 8.01 MiB (1%) | 75 |
| `["linalg", "factorization", "(\"eigen\", \"Bidiagonal\", 256)"]` | 341.716 μs (45%) | 0.000 ns | 516.81 KiB (1%) | 70 |
| `["linalg", "factorization", "(\"eigen\", \"Diagonal\", 1024)"]` | 734.053 μs (45%) | 0.000 ns | 8.00 MiB (1%) | 3 |
| `["linalg", "factorization", "(\"eigen\", \"Diagonal\", 256)"]` | 40.052 μs (45%) | 0.000 ns | 512.11 KiB (1%) | 3 |
| `["linalg", "factorization", "(\"eigen\", \"LowerTriangular\", 1024)"]` | 88.653 ms (45%) | 13.601 ms | 32.03 MiB (1%) | 14 |
| `["linalg", "factorization", "(\"eigen\", \"LowerTriangular\", 256)"]` | 2.232 ms (45%) | 0.000 ns | 2.01 MiB (1%) | 13 |
| `["linalg", "factorization", "(\"eigen\", \"Matrix\", 1024)"]` | 1.427 s (45%) | 14.524 ms | 33.07 MiB (1%) | 45 |
| `["linalg", "factorization", "(\"eigen\", \"Matrix\", 256)"]` | 50.422 ms (45%) | 0.000 ns | 2.27 MiB (1%) | 39 |
| `["linalg", "factorization", "(\"eigen\", \"SymTridiagonal\", 1024)"]` | 106.783 ms (45%) | 0.000 ns | 8.27 MiB (1%) | 42 |
| `["linalg", "factorization", "(\"eigen\", \"SymTridiagonal\", 256)"]` | 5.617 ms (45%) | 0.000 ns | 582.03 KiB (1%) | 36 |
| `["linalg", "factorization", "(\"eigen\", \"UpperTriangular\", 1024)"]` | 73.657 ms (45%) | 13.635 ms | 24.03 MiB (1%) | 12 |
| `["linalg", "factorization", "(\"eigen\", \"UpperTriangular\", 256)"]` | 1.848 ms (45%) | 0.000 ns | 1.51 MiB (1%) | 11 |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 1024)"]` | 24.686 ms (45%) | 0.000 ns | 8.01 MiB (1%) | 4 |
| `["linalg", "factorization", "(\"lu\", \"Matrix\", 256)"]` | 669.885 μs (45%) | 0.000 ns | 514.23 KiB (1%) | 4 |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 1024)"]` | 13.241 μs (45%) | 0.000 ns | 40.75 KiB (1%) | 8 |
| `["linalg", "factorization", "(\"lu\", \"Tridiagonal\", 256)"]` | 3.954 μs (45%) | 0.000 ns | 10.75 KiB (1%) | 8 |
| `["linalg", "factorization", "(\"qr\", \"Matrix\", 1024)"]` | 65.155 ms (45%) | 0.000 ns | 8.56 MiB (1%) | 8 |
| `["linalg", "factorization", "(\"qr\", \"Matrix\", 256)"]` | 1.796 ms (45%) | 0.000 ns | 656.30 KiB (1%) | 8 |
| `["linalg", "factorization", "(\"schur\", \"Matrix\", 1024)"]` | 1.272 s (45%) | 0.000 ns | 16.30 MiB (1%) | 12 |
| `["linalg", "factorization", "(\"schur\", \"Matrix\", 256)"]` | 47.272 ms (45%) | 0.000 ns | 1.08 MiB (1%) | 12 |
| `["linalg", "factorization", "(\"svd\", \"Bidiagonal\", 1024)"]` | 76.545 ms (45%) | 13.563 ms | 40.11 MiB (1%) | 14 |
| `["linalg", "factorization", "(\"svd\", \"Bidiagonal\", 256)"]` | 5.291 ms (45%) | 0.000 ns | 2.53 MiB (1%) | 13 |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 9.292 ms (45%) | 0.000 ns | 755.38 KiB (1%) | 10280 |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 256)"]` | 636.300 μs (45%) | 0.000 ns | 182.88 KiB (1%) | 2596 |
| `["linalg", "factorization", "(\"svd\", \"LowerTriangular\", 1024)"]` | 640.368 ms (45%) | 28.163 ms | 56.13 MiB (1%) | 15 |
| `["linalg", "factorization", "(\"svd\", \"LowerTriangular\", 256)"]` | 16.622 ms (45%) | 0.000 ns | 3.53 MiB (1%) | 14 |
| `["linalg", "factorization", "(\"svd\", \"Matrix\", 1024)"]` | 664.110 ms (45%) | 28.264 ms | 48.13 MiB (1%) | 13 |
| `["linalg", "factorization", "(\"svd\", \"Matrix\", 256)"]` | 17.512 ms (45%) | 0.000 ns | 3.03 MiB (1%) | 12 |
| `["linalg", "factorization", "(\"svd\", \"UpperTriangular\", 1024)"]` | 654.458 ms (45%) | 27.141 ms | 56.13 MiB (1%) | 15 |
| `["linalg", "factorization", "(\"svd\", \"UpperTriangular\", 256)"]` | 16.770 ms (45%) | 0.000 ns | 3.53 MiB (1%) | 14 |
| `["micro", "fib"]` | 29.328 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["micro", "mandel"]` | 108.030 μs (5%) | 0.000 ns | 4.44 KiB (1%) | 1 |
| `["micro", "parseint"]` | 141.044 μs (5%) | 0.000 ns | 109.38 KiB (1%) | 3000 |
| `["micro", "pisum"]` | 18.103 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["micro", "printfd"]` | 501.722 μs (5%) | 0.000 ns | 400 bytes (1%) | 5 |
| `["micro", "quicksort"]` | 265.879 μs (5%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["micro", "randmatmul"]` | 60.119 ms (5%) | 13.839 ms | 22.89 MiB (1%) | 6 |
| `["micro", "randmatstat"]` | 7.368 ms (5%) | 0.000 ns | 15.14 MiB (1%) | 13002 |
| `["misc", "18129"]` | 16.683 ms (5%) | 0.000 ns | 3.10 MiB (1%) | 5415 |
| `["misc", "20517"]` | 347.729 μs (5%) | 0.000 ns | 536.92 KiB (1%) | 33656 |
| `["misc", "23042", "Complex{Float32}"]` | 6.636 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "23042", "Complex{Float64}"]` | 13.704 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "23042", "Float32"]` | 2.108 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "23042", "Float64"]` | 5.121 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "afoldl", "Complex{Float64}"]` | 337.281 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "afoldl", "Float64"]` | 334.072 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "afoldl", "Int"]` | 306.453 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"Int\", \"Int\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"Int\", \"UInt\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"UInt32\", \"UInt32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "bitshift", "(\"UInt\", \"UInt\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "issue 12165", "Float16"]` | 3.946 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "issue 12165", "Float32"]` | 3.851 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "issue 12165", "Float64"]` | 3.326 ms (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "julia", "(\"macroexpand\", \"evalpoly\")"]` | 439.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 1.399 ms (5%) | 0.000 ns | 15.25 KiB (1%) | 214 |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 162.189 μs (5%) | 0.000 ns | 2.30 KiB (1%) | 42 |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 2.457 ms (5%) | 0.000 ns | 28.41 KiB (1%) | 412 |
| `["misc", "parse", "DateTime"]` | 18.296 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "parse", "Float64"]` | 37.870 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "parse", "Int"]` | 38.183 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["misc", "repeat", "(200, 1, 24)"]` | 12.773 μs (5%) | 0.000 ns | 81.02 KiB (1%) | 101 |
| `["misc", "repeat", "(200, 24, 1)"]` | 16.274 μs (5%) | 0.000 ns | 56.45 KiB (1%) | 605 |
| `["misc", "splatting", "(3, 3, 3)"]` | 23.600 μs (5%) | 0.000 ns | 6.25 KiB (1%) | 300 |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 54.373 μs (5%) | 0.000 ns | 3.86 KiB (1%) | 51 |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 52.674 μs (5%) | 0.000 ns | 1.69 KiB (1%) | 47 |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 60.780 μs (5%) | 0.000 ns | 9.94 KiB (1%) | 51 |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 53.833 μs (5%) | 0.000 ns | 2.83 KiB (1%) | 51 |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 53.086 μs (5%) | 0.000 ns | 1.86 KiB (1%) | 49 |
| `["problem", "chaosgame", "chaosgame"]` | 86.151 ms (5%) | 0.000 ns | 512.19 KiB (1%) | 4 |
| `["problem", "fem", "sparse_fem"]` | 270.420 ms (5%) | 50.020 ms | 121.02 MiB (1%) | 172 |
| `["problem", "go", "go_game"]` | 648.968 ms (5%) | 298.348 ms | 386.84 MiB (1%) | 2932663 |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 3.944 s (5%) | 2.867 s | 3.56 GiB (1%) | 1950237 |
| `["problem", "imdb", "centrality"]` | 706.320 ms (5%) | 100.119 ms | 95.25 MiB (1%) | 1316501 |
| `["problem", "json", "parse_json"]` | 526.183 μs (5%) | 0.000 ns | 205.89 KiB (1%) | 9390 |
| `["problem", "laplacian", "laplace_iter_devec"]` | 11.444 ms (5%) | 0.000 ns | 64.16 KiB (1%) | 4 |
| `["problem", "laplacian", "laplace_iter_sub"]` | 122.764 ms (5%) | 84.171 ms | 120.84 MiB (1%) | 12295 |
| `["problem", "laplacian", "laplace_iter_vec"]` | 105.400 ms (5%) | 84.180 ms | 120.59 MiB (1%) | 8194 |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 28.145 ms (5%) | 16.992 ms | 24.71 MiB (1%) | 98492 |
| `["problem", "monte carlo", "euro_option_devec"]` | 31.494 ms (5%) | 0.000 ns | 156.41 KiB (1%) | 4 |
| `["problem", "monte carlo", "euro_option_vec"]` | 29.301 ms (5%) | 0.000 ns | 234.61 KiB (1%) | 6 |
| `["problem", "raytrace", "raytrace"]` | 521.731 ms (5%) | 173.030 ms | 198.95 MiB (1%) | 3841801 |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 1.017 ms (5%) | 0.000 ns | 937.97 KiB (1%) | 12 |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.296 ms (5%) | 0.000 ns | 1.83 MiB (1%) | 12 |
| `["problem", "simplex", "simplex"]` | 17.559 ms (5%) | 0.000 ns | 251.02 KiB (1%) | 11 |
| `["problem", "spellcheck", "spellcheck"]` | 10.695 s (5%) | 4.425 s | 4.24 GiB (1%) | 88987108 |
| `["problem", "stockcorr", "stockcorr"]` | 648.496 ms (5%) | 442.179 ms | 231.32 MiB (1%) | 20015 |
| `["problem", "ziggurat", "ziggurat"]` | 21.615 s (5%) | 15.174 s | 18.90 GiB (1%) | 10000002 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"'a':'z'\")"]` | 7.830 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large BitSet\")"]` | 6.682 μs (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Dict\")"]` | 31.881 μs (25%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Set\")"]` | 31.793 μs (25%) | 0.000 ns | 80 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large String\")"]` | 7.959 μs (25%) | 0.000 ns | 3.69 KiB (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"large Vector\")"]` | 5.836 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small BitSet\")"]` | 8.297 μs (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Dict\")"]` | 35.001 μs (25%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Set\")"]` | 37.167 μs (25%) | 0.000 ns | 80 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small String\")"]` | 7.635 μs (25%) | 0.000 ns | 112 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"ImplicitRNG\", \"small Vector\")"]` | 7.229 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"'a':'z'\")"]` | 7.757 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large BitSet\")"]` | 7.203 μs (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Dict\")"]` | 32.008 μs (25%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Set\")"]` | 31.643 μs (25%) | 0.000 ns | 80 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large String\")"]` | 7.997 μs (25%) | 0.000 ns | 3.69 KiB (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"large Vector\")"]` | 5.780 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small BitSet\")"]` | 9.061 μs (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Dict\")"]` | 34.657 μs (25%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Set\")"]` | 34.591 μs (25%) | 0.000 ns | 80 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small String\")"]` | 7.548 μs (25%) | 0.000 ns | 112 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"MersenneTwister\", \"small Vector\")"]` | 7.367 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"'a':'z'\")"]` | 20.477 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large BitSet\")"]` | 19.356 μs (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Dict\")"]` | 92.380 μs (25%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Set\")"]` | 90.148 μs (25%) | 0.000 ns | 80 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large String\")"]` | 20.304 μs (25%) | 0.000 ns | 3.69 KiB (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"large Vector\")"]` | 18.729 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small BitSet\")"]` | 19.546 μs (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Dict\")"]` | 105.083 μs (25%) | 0.000 ns | 64 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Set\")"]` | 104.131 μs (25%) | 0.000 ns | 80 bytes (1%) | 2 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small String\")"]` | 18.444 μs (25%) | 0.000 ns | 112 bytes (1%) | 1 |
| `["random", "collections", "(\"rand!\", \"RandomDevice\", \"small Vector\")"]` | 18.763 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"'a':'z'\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large BitSet\")"]` | 45.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Dict\")"]` | 45.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Set\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large String\")"]` | 30.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"large Vector\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small BitSet\")"]` | 47.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Dict\")"]` | 40.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Set\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small String\")"]` | 30.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"ImplicitRNG\", \"small Vector\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"'a':'z'\")"]` | 42.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large BitSet\")"]` | 43.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Dict\")"]` | 41.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Set\")"]` | 45.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large String\")"]` | 29.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"large Vector\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small BitSet\")"]` | 46.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Dict\")"]` | 38.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Set\")"]` | 33.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small String\")"]` | 30.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"MersenneTwister\", \"small Vector\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"'a':'z'\")"]` | 68.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large BitSet\")"]` | 70.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Dict\")"]` | 70.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Set\")"]` | 60.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large String\")"]` | 58.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"large Vector\")"]` | 59.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small BitSet\")"]` | 70.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Dict\")"]` | 67.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Set\")"]` | 67.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small String\")"]` | 58.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 1 |
| `["random", "collections", "(\"rand\", \"RandomDevice\", \"small Vector\")"]` | 55.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\")"]` | 91.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 2 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", 100)"]` | 513.000 ns (25%) | 0.000 ns | 320 bytes (1%) | 2 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\")"]` | 281.000 ns (25%) | 0.000 ns | 400 bytes (1%) | 6 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"\\\"qwèrtï\\\"\", 100)"]` | 1.846 μs (25%) | 0.000 ns | 1.13 KiB (1%) | 7 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\")"]` | 92.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 2 |
| `["random", "randstring", "(\"randstring\", \"MersenneTwister\", \"collect(UInt8, \\\"qwerty\\\"\", 100)"]` | 628.000 ns (25%) | 0.000 ns | 320 bytes (1%) | 2 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:170141183460469231731687303715884105728\")"]` | 169.000 ns (25%) | 0.000 ns | 104 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551615\")"]` | 168.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:18446744073709551616\")"]` | 171.000 ns (25%) | 0.000 ns | 104 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:1\")"]` | 164.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:2^10000\")"]` | 291.000 ns (25%) | 0.000 ns | 1.31 KiB (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967295\")"]` | 160.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"BigInt\", \"1:4294967297\")"]` | 170.000 ns (25%) | 0.000 ns | 96 bytes (1%) | 4 |
| `["random", "ranges", "(\"RangeGenerator\", \"Bool\", \"true:true\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551615\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:18446744073709551616\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:1\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967295\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int128\", \"1:4294967297\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int16\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int32\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967295\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967297\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"Int8\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:170141183460469231731687303715884105728\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551615\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:18446744073709551616\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:1\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967295\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt128\", \"1:4294967297\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt16\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt32\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt32\", \"1:4294967295\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:18446744073709551615\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967295\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967297\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt8\", \"1:1\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand!\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 803.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand!\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 799.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand!\", \"RandomDevice\", \"Int\", \"1:1000\")"]` | 3.358 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"ImplicitRNG\", \"Int\", \"1:1000\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:1)\")"]` | 205.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 4 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 161.000 ns (25%) | 0.000 ns | 56 bytes (1%) | 4 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 192.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 4 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551616)\")"]` | 179.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:2^10000)\")"]` | 401.000 ns (25%) | 0.000 ns | 1.27 KiB (1%) | 4 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 168.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 4 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967297)\")"]` | 203.000 ns (25%) | 0.000 ns | 48 bytes (1%) | 4 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Bool\", \"RangeGenerator(true:true)\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:1)\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967295)\")"]` | 25.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int128\", \"RangeGenerator(1:4294967297)\")"]` | 25.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int16\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int32\", \"RangeGenerator(1:1)\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:1)\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:4294967295)\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int64\", \"RangeGenerator(1:4294967297)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int8\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"Int\", \"1:1000\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:1)\")"]` | 25.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:170141183460469231731687303715884105728)\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551615)\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:18446744073709551616)\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967295)\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt128\", \"RangeGenerator(1:4294967297)\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt16\", \"RangeGenerator(1:1)\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt32\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt32\", \"RangeGenerator(1:4294967295)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:18446744073709551615)\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967295)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt64\", \"RangeGenerator(1:4294967297)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"UInt8\", \"RangeGenerator(1:1)\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "ranges", "(\"rand\", \"RandomDevice\", \"Int\", \"1:1000\")"]` | 48.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "sequences", "(\"randcycle\", \"MersenneTwister\", \"1000\")"]` | 5.643 μs (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["random", "sequences", "(\"randcycle\", \"MersenneTwister\", \"5\")"]` | 57.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 1 |
| `["random", "sequences", "(\"randperm\", \"MersenneTwister\", \"1000\")"]` | 6.190 μs (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["random", "sequences", "(\"randperm\", \"MersenneTwister\", \"5\")"]` | 56.000 ns (25%) | 0.000 ns | 128 bytes (1%) | 1 |
| `["random", "sequences", "(\"randsubseq!\", \"MersenneTwister\", \"0.2\")"]` | 4.170 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "sequences", "(\"randsubseq!\", \"MersenneTwister\", \"0.8\")"]` | 6.680 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "sequences", "(\"shuffle!\", \"MersenneTwister\")"]` | 5.773 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"ImplicitRNG\", \"Float64\")"]` | 732.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"ImplicitRNG\", \"Int64\")"]` | 1.132 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Bool\")"]` | 810.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 16.076 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 4.697 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 4.985 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 14.012 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int16}\")"]` | 4.334 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int32}\")"]` | 4.443 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int64}\")"]` | 10.156 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int8}\")"]` | 4.321 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 14.030 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 4.335 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 4.457 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt64}\")"]` | 10.162 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt8}\")"]` | 4.310 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float16\")"]` | 7.419 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float32\")"]` | 774.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Float64\")"]` | 736.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int128\")"]` | 2.321 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int16\")"]` | 222.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int32\")"]` | 659.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int64\")"]` | 1.122 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Int8\")"]` | 173.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt128\")"]` | 2.314 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt16\")"]` | 226.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt32\")"]` | 659.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt64\")"]` | 1.122 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"UInt8\")"]` | 169.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"RandomDevice\", \"Float64\")"]` | 8.505 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand!\", \"RandomDevice\", \"Int64\")"]` | 238.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Float64\")"]` | 17.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"ImplicitRNG\", \"Int64\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Bool\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int16}\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int32}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int64}\")"]` | 26.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{Int8}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt16}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt32}\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt64}\")"]` | 25.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Complex{UInt8}\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float16\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float32\")"]` | 17.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Float64\")"]` | 17.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int128\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int16\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int32\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int64\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"Int8\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt128\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt16\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt32\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt64\")"]` | 19.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"MersenneTwister\", \"UInt8\")"]` | 18.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Float64\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"rand\", \"RandomDevice\", \"Int64\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"ImplicitRNG\", \"Float64\")"]` | 4.670 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float16\")"]` | 16.883 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float32\")"]` | 4.853 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"MersenneTwister\", \"Float64\")"]` | 4.535 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp!\", \"RandomDevice\", \"Float64\")"]` | 11.286 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"Float64\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float16\")"]` | 28.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float32\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"Float64\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"Float64\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randexp\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 33.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"ImplicitRNG\", \"Float64\")"]` | 4.731 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 79.937 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 10.788 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 9.816 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float16\")"]` | 16.846 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float32\")"]` | 4.991 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"MersenneTwister\", \"Float64\")"]` | 4.772 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn!\", \"RandomDevice\", \"Float64\")"]` | 11.672 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"Float64\")"]` | 23.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"ImplicitRNG\", \"ImplicitFloat64\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float16}\")"]` | 72.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float32}\")"]` | 25.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Complex{Float64}\")"]` | 25.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float16\")"]` | 27.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float32\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"Float64\")"]` | 20.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"MersenneTwister\", \"ImplicitFloat64\")"]` | 22.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"RandomDevice\", \"Float64\")"]` | 38.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["random", "types", "(\"randn\", \"RandomDevice\", \"ImplicitFloat64\")"]` | 32.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 110.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 160.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 37.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 37.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"negative argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"one\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"negative argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"zero\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acos", "(\"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"1 <= abs(x) < 2\", \"positive argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"1 <= abs(x) < 2\", \"positive argument\", \"Float64\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float64\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"one\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"one\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "acosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigFloat\")"]` | 60.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"BigInt\")"]` | 93.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 63.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{BigInt}\")"]` | 123.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float32}\")"]` | 136.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Float64}\")"]` | 135.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{Int64}\")"]` | 108.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Complex{UInt64}\")"]` | 107.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float32\")"]` | 106.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Float64\")"]` | 104.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"Int64\")"]` | 87.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigFloat\", \"UInt64\")"]` | 86.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigFloat\")"]` | 94.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"BigInt\")"]` | 140.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigFloat}\")"]` | 99.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{BigInt}\")"]` | 145.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float32}\")"]` | 165.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Float64}\")"]` | 165.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{Int64}\")"]` | 242.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Complex{UInt64}\")"]` | 247.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float32\")"]` | 138.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Float64\")"]` | 138.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"Int64\")"]` | 100.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"BigInt\", \"UInt64\")"]` | 136.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 65.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"BigInt\")"]` | 99.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 90.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 131.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 152.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 159.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 119.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 120.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float32\")"]` | 112.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Float64\")"]` | 111.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"Int64\")"]` | 92.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigFloat}\", \"UInt64\")"]` | 90.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigFloat\")"]` | 124.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"BigInt\")"]` | 143.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 136.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 252.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 209.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 209.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 246.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 250.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float32\")"]` | 164.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Float64\")"]` | 165.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"Int64\")"]` | 87.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{BigInt}\", \"UInt64\")"]` | 138.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigFloat\")"]` | 135.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"BigInt\")"]` | 165.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 150.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 210.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float32}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigFloat\")"]` | 136.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"BigInt\")"]` | 165.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 150.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 210.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Float64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigFloat\")"]` | 108.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"BigInt\")"]` | 246.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 119.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 245.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{Int64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigFloat\")"]` | 108.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"BigInt\")"]` | 236.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 112.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 242.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Complex{UInt64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigFloat\")"]` | 105.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"BigInt\")"]` | 138.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigFloat}\")"]` | 110.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{BigInt}\")"]` | 165.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float32\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigFloat\")"]` | 105.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"BigInt\")"]` | 138.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigFloat}\")"]` | 111.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{BigInt}\")"]` | 165.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Float64\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigFloat\")"]` | 91.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"BigInt\")"]` | 135.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigFloat}\")"]` | 93.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{BigInt}\")"]` | 137.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"Int64\", \"UInt64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigFloat\")"]` | 86.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"BigInt\")"]` | 134.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigFloat}\")"]` | 90.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{BigInt}\")"]` | 92.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"Int64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"add\", \"UInt64\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigFloat\")"]` | 172.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"BigInt\")"]` | 51.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 459.000 ns (50%) | 0.000 ns | 992 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{BigInt}\")"]` | 499.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float32}\")"]` | 509.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Float64}\")"]` | 507.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{Int64}\")"]` | 486.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Complex{UInt64}\")"]` | 483.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float32\")"]` | 95.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Float64\")"]` | 95.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"Int64\")"]` | 45.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigFloat\", \"UInt64\")"]` | 44.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigFloat\")"]` | 208.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"BigInt\")"]` | 244.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigFloat}\")"]` | 416.000 ns (50%) | 0.000 ns | 992 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{BigInt}\")"]` | 489.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float32}\")"]` | 482.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Float64}\")"]` | 511.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{Int64}\")"]` | 727.000 ns (50%) | 0.000 ns | 1.27 KiB (1%) | 27 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Complex{UInt64}\")"]` | 689.000 ns (50%) | 0.000 ns | 1.27 KiB (1%) | 27 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float32\")"]` | 252.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Float64\")"]` | 254.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"Int64\")"]` | 83.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"BigInt\", \"UInt64\")"]` | 81.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 203.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"BigInt\")"]` | 87.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 445.000 ns (50%) | 0.000 ns | 1.23 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 499.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 504.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 509.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 491.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 486.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float32\")"]` | 177.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Float64\")"]` | 164.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"Int64\")"]` | 70.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigFloat}\", \"UInt64\")"]` | 69.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigFloat\")"]` | 255.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"BigInt\")"]` | 328.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 497.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 548.000 ns (50%) | 0.000 ns | 1.23 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 569.000 ns (50%) | 0.000 ns | 1.73 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 581.000 ns (50%) | 0.000 ns | 1.73 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 709.000 ns (50%) | 0.000 ns | 1.34 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 708.000 ns (50%) | 0.000 ns | 1.34 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float32\")"]` | 339.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Float64\")"]` | 338.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"Int64\")"]` | 128.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{BigInt}\", \"UInt64\")"]` | 127.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigFloat\")"]` | 257.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"BigInt\")"]` | 334.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 511.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 576.000 ns (50%) | 0.000 ns | 1.73 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 39.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 29.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 41.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 42.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Float32\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"Int64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float32}\", \"UInt64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigFloat\")"]` | 256.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"BigInt\")"]` | 335.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 523.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 566.000 ns (50%) | 0.000 ns | 1.73 KiB (1%) | 33 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 30.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 30.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 30.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 30.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Float32\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Float64}\", \"UInt64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigFloat\")"]` | 212.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"BigInt\")"]` | 285.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 483.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 707.000 ns (50%) | 0.000 ns | 1.34 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 32.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 32.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 21.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 23.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Float64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"Int64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{Int64}\", \"UInt64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigFloat\")"]` | 204.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"BigInt\")"]` | 271.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 488.000 ns (50%) | 0.000 ns | 1.48 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 700.000 ns (50%) | 0.000 ns | 1.34 KiB (1%) | 28 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 32.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 31.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 25.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 24.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Float32\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Float64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"Int64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Complex{UInt64}\", \"UInt64\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigFloat\")"]` | 205.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"BigInt\")"]` | 251.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigFloat}\")"]` | 498.000 ns (50%) | 0.000 ns | 992 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{BigInt}\")"]` | 550.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{Float32}\")"]` | 20.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{Float64}\")"]` | 32.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{Int64}\")"]` | 21.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Complex{UInt64}\")"]` | 22.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float32\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigFloat\")"]` | 203.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"BigInt\")"]` | 253.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigFloat}\")"]` | 499.000 ns (50%) | 0.000 ns | 992 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{BigInt}\")"]` | 551.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{Float32}\")"]` | 31.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{Float64}\")"]` | 31.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{Int64}\")"]` | 42.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Complex{UInt64}\")"]` | 40.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Float64\", \"UInt64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigFloat\")"]` | 184.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"BigInt\")"]` | 221.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigFloat}\")"]` | 405.000 ns (50%) | 0.000 ns | 992 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{BigInt}\")"]` | 459.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Float32}\")"]` | 20.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Float64}\")"]` | 30.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{Int64}\")"]` | 42.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Complex{UInt64}\")"]` | 42.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"Int64\", \"UInt64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigFloat\")"]` | 175.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"BigInt\")"]` | 214.000 ns (50%) | 0.000 ns | 224 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigFloat}\")"]` | 403.000 ns (50%) | 0.000 ns | 992 bytes (1%) | 19 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{BigInt}\")"]` | 467.000 ns (50%) | 0.000 ns | 1.19 KiB (1%) | 23 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Float32}\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Float64}\")"]` | 30.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{Int64}\")"]` | 40.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Complex{UInt64}\")"]` | 41.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Float64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"Int64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"div\", \"UInt64\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigFloat\")"]` | 89.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"BigInt\")"]` | 51.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 119.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{BigInt}\")"]` | 86.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float32}\")"]` | 143.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Float64}\")"]` | 145.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{Int64}\")"]` | 69.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Complex{UInt64}\")"]` | 67.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float32\")"]` | 100.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Float64\")"]` | 100.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"Int64\")"]` | 45.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigFloat\", \"UInt64\")"]` | 44.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigFloat\")"]` | 50.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"BigInt\")"]` | 137.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigFloat}\")"]` | 101.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{BigInt}\")"]` | 250.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float32}\")"]` | 250.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Float64}\")"]` | 250.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{Int64}\")"]` | 247.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Complex{UInt64}\")"]` | 246.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float32\")"]` | 171.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Float64\")"]` | 168.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"Int64\")"]` | 136.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"BigInt\", \"UInt64\")"]` | 139.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 119.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"BigInt\")"]` | 86.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 218.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 189.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 290.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 291.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 166.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 163.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float32\")"]` | 169.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Float64\")"]` | 166.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"Int64\")"]` | 70.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigFloat}\", \"UInt64\")"]` | 69.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigFloat\")"]` | 85.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"BigInt\")"]` | 256.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 189.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 733.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 446.000 ns (50%) | 0.000 ns | 1.56 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 448.000 ns (50%) | 0.000 ns | 1.56 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 730.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 717.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float32\")"]` | 255.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Float64\")"]` | 256.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"Int64\")"]` | 245.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{BigInt}\", \"UInt64\")"]` | 247.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigFloat\")"]` | 144.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"BigInt\")"]` | 250.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 288.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 448.000 ns (50%) | 0.000 ns | 1.56 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float32}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigFloat\")"]` | 145.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"BigInt\")"]` | 249.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 292.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 447.000 ns (50%) | 0.000 ns | 1.56 KiB (1%) | 29 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Float64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigFloat\")"]` | 70.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"BigInt\")"]` | 243.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 165.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 739.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{Int64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigFloat\")"]` | 68.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"BigInt\")"]` | 231.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 165.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 729.000 ns (50%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 18.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Float64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Complex{UInt64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigFloat\")"]` | 100.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"BigInt\")"]` | 166.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigFloat}\")"]` | 167.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{BigInt}\")"]` | 256.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float32\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigFloat\")"]` | 99.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"BigInt\")"]` | 167.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigFloat}\")"]` | 166.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{BigInt}\")"]` | 254.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Complex{UInt64}\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Float64\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigFloat\")"]` | 46.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"BigInt\")"]` | 97.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigFloat}\")"]` | 68.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{BigInt}\")"]` | 250.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"Int64\", \"UInt64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigFloat\")"]` | 44.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"BigInt\")"]` | 136.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigFloat}\")"]` | 68.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{BigInt}\")"]` | 249.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{Float64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Float64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"Int64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"mul\", \"UInt64\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"BigInt\")"]` | 144.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"Bool\")"]` | 163.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"Int64\")"]` | 186.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"BigInt\", \"UInt64\")"]` | 133.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"BigInt\")"]` | 204.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Bool\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"Int64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Bool\", \"UInt64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"BigInt\")"]` | 309.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"Bool\")"]` | 87.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"Int64\")"]` | 66.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Char\", \"UInt64\")"]` | 110.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"BigInt\")"]` | 219.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Bool\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"Int64\", \"UInt64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"BigInt\")"]` | 196.000 ns (40%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Bool\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"Int64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"rem type\", \"UInt64\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigFloat\")"]` | 48.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"BigInt\")"]` | 69.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigFloat}\")"]` | 71.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{BigInt}\")"]` | 122.000 ns (50%) | 0.000 ns | 368 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float32}\")"]` | 135.000 ns (50%) | 0.000 ns | 368 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Float64}\")"]` | 138.000 ns (50%) | 0.000 ns | 368 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{Int64}\")"]` | 107.000 ns (50%) | 0.000 ns | 368 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Complex{UInt64}\")"]` | 107.000 ns (50%) | 0.000 ns | 368 bytes (1%) | 7 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float32\")"]` | 88.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Float64\")"]` | 87.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"Int64\")"]` | 62.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigFloat\", \"UInt64\")"]` | 61.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigFloat\")"]` | 71.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"BigInt\")"]` | 138.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigFloat}\")"]` | 99.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{BigInt}\")"]` | 252.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float32}\")"]` | 175.000 ns (50%) | 0.000 ns | 592 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Float64}\")"]` | 173.000 ns (50%) | 0.000 ns | 592 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{Int64}\")"]` | 357.000 ns (50%) | 0.000 ns | 160 bytes (1%) | 8 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Complex{UInt64}\")"]` | 344.000 ns (50%) | 0.000 ns | 160 bytes (1%) | 8 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float32\")"]` | 127.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Float64\")"]` | 128.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"Int64\")"]` | 134.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"BigInt\", \"UInt64\")"]` | 135.000 ns (50%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigFloat\")"]` | 53.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"BigInt\")"]` | 81.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigFloat}\")"]` | 73.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{BigInt}\")"]` | 105.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float32}\")"]` | 133.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Float64}\")"]` | 132.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{Int64}\")"]` | 95.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Complex{UInt64}\")"]` | 95.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float32\")"]` | 93.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Float64\")"]` | 91.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"Int64\")"]` | 66.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigFloat}\", \"UInt64\")"]` | 65.000 ns (50%) | 0.000 ns | 144 bytes (1%) | 3 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigFloat\")"]` | 99.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"BigInt\")"]` | 150.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigFloat}\")"]` | 109.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{BigInt}\")"]` | 237.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float32}\")"]` | 200.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Float64}\")"]` | 198.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{Int64}\")"]` | 252.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Complex{UInt64}\")"]` | 219.000 ns (50%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float32\")"]` | 148.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Float64\")"]` | 148.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"Int64\")"]` | 88.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{BigInt}\", \"UInt64\")"]` | 138.000 ns (50%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigFloat\")"]` | 112.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"BigInt\")"]` | 150.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigFloat}\")"]` | 132.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{BigInt}\")"]` | 193.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Float64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float32}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigFloat\")"]` | 112.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"BigInt\")"]` | 150.000 ns (50%) | 0.000 ns | 480 bytes (1%) | 9 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigFloat}\")"]` | 132.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{BigInt}\")"]` | 198.000 ns (50%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{Float64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Float64}\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigFloat\")"]` | 89.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"BigInt\")"]` | 229.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigFloat}\")"]` | 96.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{BigInt}\")"]` | 217.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{Int64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigFloat\")"]` | 148.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"BigInt\")"]` | 227.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigFloat}\")"]` | 93.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{BigInt}\")"]` | 222.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Float32\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Float64\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Complex{UInt64}\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigFloat\")"]` | 93.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"BigInt\")"]` | 128.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigFloat}\")"]` | 118.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{BigInt}\")"]` | 172.000 ns (50%) | 0.000 ns | 592 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{Float32}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{Float64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Complex{UInt64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float32\", \"UInt64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigFloat\")"]` | 86.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"BigInt\")"]` | 128.000 ns (50%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigFloat}\")"]` | 118.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{BigInt}\")"]` | 172.000 ns (50%) | 0.000 ns | 592 bytes (1%) | 11 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{Int64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Complex{UInt64}\")"]` | 16.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"Int64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Float64\", \"UInt64\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigFloat\")"]` | 63.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"BigInt\")"]` | 118.000 ns (50%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigFloat}\")"]` | 91.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{BigInt}\")"]` | 227.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Float64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Float64\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"Int64\", \"UInt64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigFloat\")"]` | 62.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"BigInt\")"]` | 109.000 ns (50%) | 0.000 ns | 40 bytes (1%) | 2 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigFloat}\")"]` | 90.000 ns (50%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{BigInt}\")"]` | 202.000 ns (50%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{Float32}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{Float64}\")"]` | 15.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{Int64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Complex{UInt64}\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Float32\")"]` | 14.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Float64\")"]` | 17.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"Int64\")"]` | 13.000 ns (50%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "arithmetic", "(\"sub\", \"UInt64\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float32\")"]` | 111.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"negative argument\", \"Float64\")"]` | 191.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"0.975 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 48.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 38.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"negative argument\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"one\", \"positive argument\", \"Float64\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"small\", \"positive argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"zero\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asin", "(\"zero\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"negative argument\", \"Float32\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float32\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"0 <= abs(x) < 2^-28\", \"positive argument\", \"Float64\")"]` | 47.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2 <= abs(x) < 2^28\", \"negative argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2 <= abs(x) < 2^28\", \"negative argument\", \"Float64\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float32\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2 <= abs(x) < 2^28\", \"positive argument\", \"Float64\")"]` | 45.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"negative argument\", \"Float32\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"negative argument\", \"Float64\")"]` | 48.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"positive argument\", \"Float32\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"2^-28 <= abs(x) < 2\", \"positive argument\", \"Float64\")"]` | 47.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"zero\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "asinh", "(\"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"negative argument\", \"Float64\")"]` | 33.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"0 <= abs(x) < 7/16\", \"positive argument\", \"Float64\")"]` | 33.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"negative argument\", \"Float64\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"11/16 <= abs(x) < 19/16\", \"positive argument\", \"Float64\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float32\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"negative argument\", \"Float64\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"39/16 <= abs(x) < 2^66\", \"positive argument\", \"Float64\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float32\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"positive argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"negative argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very large\", \"positive argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"zero\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan", "(\"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float64\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float64\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float64\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float64\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 39.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float64\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float64\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 33.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float64\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float64\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"negative argument\", \"Float32\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"negative argument\", \"Float64\")"]` | 45.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"positive argument\", \"Float32\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"2^-28 <= abs(x) < 0.5\", \"positive argument\", \"Float64\")"]` | 45.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"one\", \"Float32\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"one\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"zero\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "atanh", "(\"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"large\", \"negative argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"large\", \"negative argument\", \"Float64\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"large\", \"positive argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"large\", \"positive argument\", \"Float64\")"]` | 50.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"medium\", \"negative argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"medium\", \"negative argument\", \"Float64\")"]` | 50.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"medium\", \"positive argument\", \"Float32\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"medium\", \"positive argument\", \"Float64\")"]` | 50.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"one\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"one\", \"Float64\")"]` | 49.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"small\", \"negative argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"small\", \"negative argument\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"small\", \"positive argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"small\", \"positive argument\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"very small\", \"negative argument\", \"Float32\")"]` | 102.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"very small\", \"negative argument\", \"Float64\")"]` | 169.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"very small\", \"positive argument\", \"Float32\")"]` | 102.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"very small\", \"positive argument\", \"Float64\")"]` | 170.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"zero\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cbrt", "(\"zero\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 34.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 35.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 35.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 35.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 35.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 35.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 35.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 35.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 39.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 64.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 50.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 54.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"negative argument\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"0 <= abs(x) < 0.00024414062f0\", \"positive argument\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"0 <= abs(x) < 2.7755602085408512e-17\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 49.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"2.7755602085408512e-17 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 47.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"zero\", \"Float32\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "cosh", "(\"zero\", \"Float64\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow1023\", \"negative argument\", Float64)"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow1023\", \"positive argument\", Float64)"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow127\", \"negative argument\", Float32)"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow127\", \"positive argument\", Float32)"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow35\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow35\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow35\", \"positive argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow3\", \"negative argument\", \"Float64\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"2pow3\", \"positive argument\", \"Float64\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"one\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"one\", \"Float64\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"small\", \"negative argument\", \"Float64\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"small\", \"positive argument\", \"Float64\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"very small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"very small\", \"negative argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"very small\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"very small\", \"positive argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"zero\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "exp2", "(\"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction II\", \"positive argument\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction I\", \"negative argument\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float32\")"]` | 31.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"arg reduction I\", \"positive argument\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float3\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"huge\", \"positive argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"large\", \"negative argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"large\", \"positive argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float32\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"medium\", \"negative argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"medium\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"medium\", \"positive argument\", \"Float64\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"one\", \"Float32\")"]` | 32.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"one\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"small\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"small\", \"negative argument\", \"Float64\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"small\", \"positive argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"small\", \"positive argument\", \"Float64\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"very small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"very small\", \"negative argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"very small\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"very small\", \"positive argument\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"zero\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "expm1", "(\"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"BigFloat\")"]` | 59.000 ns (40%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"add\", \"BigInt\")"]` | 137.000 ns (40%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigFloat}\")"]` | 89.000 ns (40%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "fastmath", "(\"add\", \"Complex{BigInt}\")"]` | 260.000 ns (40%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "fastmath", "(\"add\", \"Complex{Float32}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Complex{Float64}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Complex{Int64}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Complex{UInt64}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"add\", \"UInt64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"BigFloat\")"]` | 172.000 ns (40%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"div\", \"BigInt\")"]` | 245.000 ns (40%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigFloat}\")"]` | 440.000 ns (40%) | 0.000 ns | 1.23 KiB (1%) | 23 |
| `["scalar", "fastmath", "(\"div\", \"Complex{BigInt}\")"]` | 481.000 ns (40%) | 0.000 ns | 1.23 KiB (1%) | 23 |
| `["scalar", "fastmath", "(\"div\", \"Complex{Float32}\")"]` | 17.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Complex{Float64}\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Complex{Int64}\")"]` | 23.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Complex{UInt64}\")"]` | 24.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"div\", \"UInt64\")"]` | 17.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"BigFloat\")"]` | 122.000 ns (40%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"mul\", \"BigInt\")"]` | 139.000 ns (40%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigFloat}\")"]` | 209.000 ns (40%) | 0.000 ns | 704 bytes (1%) | 13 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{BigInt}\")"]` | 747.000 ns (40%) | 0.000 ns | 288 bytes (1%) | 15 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{Float32}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{Float64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{Int64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Complex{UInt64}\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"mul\", \"UInt64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"BigFloat\")"]` | 48.000 ns (40%) | 0.000 ns | 112 bytes (1%) | 2 |
| `["scalar", "fastmath", "(\"sub\", \"BigInt\")"]` | 140.000 ns (40%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigFloat}\")"]` | 71.000 ns (40%) | 0.000 ns | 256 bytes (1%) | 5 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{BigInt}\")"]` | 254.000 ns (40%) | 0.000 ns | 120 bytes (1%) | 6 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{Float32}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{Float64}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{Int64}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Complex{UInt64}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"Int64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "(\"sub\", \"UInt64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "fastmath", "13786"]` | 14.546 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float32\")"]` | 27.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 2\", \"Float64\")"]` | 41.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float32\")"]` | 25.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"agument reduction, k = 83\", \"Float64\")"]` | 41.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float32\")"]` | 20.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"direct approx, k = 0\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float32\")"]` | 24.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"no agument reduction, k = 1\", \"Float64\")"]` | 31.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"normal path -> small, k = -1075\", \"Float64\")"]` | 80.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"normal path -> small, k = -150\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"overflow\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"overflow\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"taylor expansion\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"underflow\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp10\", \"underflow\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"fast path, k = 1\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"fast path, k = 1\", \"Float64\")"]` | 31.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"no agument reduction, k = 9\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"no agument reduction, k = 9\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path -> small, k = -1045\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path -> small, k = -1045\", \"Float64\")"]` | 72.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path, k = 2\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"normal path, k = 2\", \"Float64\")"]` | 40.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"overflow\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"overflow\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"small argument path\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"small argument path\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"underflow\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exp\", \"underflow\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"norm\", \"Float32\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"norm\", \"Float64\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"subnorm\", \"Float32\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"exponent\", \"subnorm\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"inf\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"inf\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"norm\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"norm\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"subnorm\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"frexp\", \"subnorm\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"inf -> inf\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"inf -> inf\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> inf\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> inf\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> norm\", \"Float32\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> norm\", \"Float64\")"]` | 15.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> subnorm\", \"Float32\")"]` | 52.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"norm -> subnorm\", \"Float64\")"]` | 52.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> norm\", \"Float32\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> norm\", \"Float64\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> subnorm\", \"Float32\")"]` | 53.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"ldexp\", \"subnorm -> subnorm\", \"Float64\")"]` | 53.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"norm\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"norm\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"subnorm\", \"Float32\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "floatexp", "(\"significand\", \"subnorm\", \"Float64\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"BaseBenchmarks.ScalarBenchmarks.__nextpow2\", \"BigInt\", \"+\")"]` | 1.205 μs (40%) | 0.000 ns | 656 bytes (1%) | 18 |
| `["scalar", "intfuncs", "(\"BaseBenchmarks.ScalarBenchmarks.__nextpow2\", \"Int64\", \"+\")"]` | 83.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"BaseBenchmarks.ScalarBenchmarks.__nextpow2\", \"UInt64\", \"+\")"]` | 93.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"BaseBenchmarks.ScalarBenchmarks.__prevpow2\", \"BigInt\", \"+\")"]` | 1.735 μs (40%) | 0.000 ns | 1.19 KiB (1%) | 30 |
| `["scalar", "intfuncs", "(\"BaseBenchmarks.ScalarBenchmarks.__prevpow2\", \"Int64\", \"+\")"]` | 71.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "intfuncs", "(\"BaseBenchmarks.ScalarBenchmarks.__prevpow2\", \"UInt64\", \"+\")"]` | 83.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "iteration", "in"]` | 4.632 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "iteration", "indexed"]` | 4.630 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 49.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (easy) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 49.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "mod2pi", "(\"no reduction\", \"zero\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"BigFloat\")"]` | 27.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"BigInt\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{BigFloat}\")"]` | 47.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{BigInt}\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{Float32}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{Float64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isequal\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"iseven\", \"BigInt\")"]` | 234.000 ns (40%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "predicate", "(\"iseven\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"iseven\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"BigFloat\")"]` | 17.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"BigInt\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{BigFloat}\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{BigInt}\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{Float64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{Int64}\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Complex{UInt64}\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isfinite\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"BigFloat\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"BigInt\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{BigFloat}\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{BigInt}\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{Float32}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{Float64}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{Int64}\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Complex{UInt64}\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinf\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"BigFloat\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"BigInt\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigFloat}\")"]` | 25.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{BigInt}\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{Float32}\")"]` | 15.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{Float64}\")"]` | 16.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{Int64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Complex{UInt64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isinteger\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"BigFloat\")"]` | 26.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"BigInt\")"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isless\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"BigFloat\")"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"BigInt\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{BigFloat}\")"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{BigInt}\")"]` | 13.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{Float32}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{Float64}\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{Int64}\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Complex{UInt64}\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Float32\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Float64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"Int64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isnan\", \"UInt64\")"]` | 13.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isodd\", \"BigInt\")"]` | 236.000 ns (40%) | 0.000 ns | 80 bytes (1%) | 4 |
| `["scalar", "predicate", "(\"isodd\", \"Int64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "predicate", "(\"isodd\", \"UInt64\")"]` | 14.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 47.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "rem_pio2", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 34.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 34.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 34.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 34.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"cos_kernel\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 50.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"cos_kernel\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 53.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"cos_kernel\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 54.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float32\", \"sin_kernel\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"negative argument\", \"Float64\", \"sin_kernel\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float32\", \"sin_kernel\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"positive argument\", \"Float64\", \"sin_kernel\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sin", "(\"no reduction\", \"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float32\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"negative argument\", \"Float64\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float32\")"]` | 26.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float32\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"negative argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 3π/4\", \"positive argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"negative argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 5π/4\", \"positive argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"negative argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 7π/4\", \"positive argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float32\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"negative argument\", \"Float64\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float32\")"]` | 27.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 9π/4\", \"positive argument\", \"Float64\")"]` | 28.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 2π/4\", \"positive argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float32\")"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float32\")"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 4π/4\", \"positive argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float32\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 6π/4\", \"positive argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"negative argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float32\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (hard) abs(x) < 8π/4\", \"positive argument\", \"Float64\")"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float32\")"]` | 58.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"negative argument\", \"Float64\")"]` | 57.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float32\")"]` | 56.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"argument reduction (paynehanek) abs(x) > 2.0^20*π/2\", \"positive argument\", \"Float64\")"]` | 56.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float32\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"negative argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float32\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"positive argument\", \"Float64\")"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float32\")"]` | 19.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sincos", "(\"no reduction\", \"zero\", \"Float64\")"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2.0^-28\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2.0^-28\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"negative argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"0 <= abs(x) < 2f-12\", \"positive argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"2.0^-28 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 59.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"2.0^-28 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 59.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"negative argument\", \"Float64\")"]` | 44.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"22.0 <= abs(x) < 709.7822265633563\", \"positive argument\", \"Float64\")"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"2f-12 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"2f-12 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 51.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"negative argument\", \"Float32\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"9f0 <= abs(x) < 88.72283f0\", \"positive argument\", \"Float32\")"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"zero\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "sinh", "(\"zero\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float32\")"]` | 110.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"large\", \"negative argument\", \"Float64\")"]` | 160.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float32\")"]` | 104.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"large\", \"positive argument\", \"Float64\")"]` | 160.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float32\")"]` | 125.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"negative argument\", \"Float64\")"]` | 151.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float32\")"]` | 121.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"medium\", \"positive argument\", \"Float64\")"]` | 161.000 ns (5%) | 0.000 ns | 32 bytes (1%) | 2 |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"very small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"zero\", \"Float32\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tan", "(\"zero\", \"Float64\")"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2.0^-28\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2f0^-12\", \"negative argument\", \"Float32\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"0 <= abs(x) < 2f0^-12\", \"positive argument\", \"Float32\")"]` | 41.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"1.0 <= abs(x) < 22.0\", \"negative argument\", \"Float64\")"]` | 60.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"1.0 <= abs(x) < 22.0\", \"positive argument\", \"Float64\")"]` | 59.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"1f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"1f0 <= abs(x) < 9f0\", \"positive argument\", \"Float32\")"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"negative argument\", \"Float64\")"]` | 54.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"2.0^-28 <= abs(x) < 1.0\", \"positive argument\", \"Float64\")"]` | 54.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"2f0^-12 <= abs(x) < 1f0\", \"negative argument\", \"Float32\")"]` | 45.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"2f0^-12 <= abs(x) < 1f0\", \"positive argument\", \"Float32\")"]` | 46.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very large\", \"negative argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very large\", \"negative argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very large\", \"positive argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very large\", \"positive argument\", \"Float64\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very small\", \"negative argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"very small\", \"positive argument\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"zero\", \"Float32\")"]` | 13.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["scalar", "tanh", "(\"zero\", \"Float64\")"]` | 16.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["shootout", "binary_trees"]` | 14.295 ms (5%) | 0.000 ns | 13.96 MiB (1%) | 783717 |
| `["shootout", "fannkuch"]` | 124.627 μs (5%) | 0.000 ns | 336 bytes (1%) | 3 |
| `["shootout", "fasta"]` | 11.790 μs (5%) | 0.000 ns | 14.11 KiB (1%) | 806 |
| `["shootout", "k_nucleotide"]` | 31.504 ms (5%) | 0.000 ns | 9.07 MiB (1%) | 254311 |
| `["shootout", "mandelbrot"]` | 3.212 ms (5%) | 0.000 ns | 8.36 KiB (1%) | 32 |
| `["shootout", "meteor_contest"]` | 1.689 s (5%) | 623.467 ms | 782.78 MiB (1%) | 34788044 |
| `["shootout", "nbody"]` | 99.317 μs (5%) | 0.000 ns | 448 bytes (1%) | 6 |
| `["shootout", "nbody_vec"]` | 274.050 μs (5%) | 0.000 ns | 110.86 KiB (1%) | 1017 |
| `["shootout", "pidigits"]` | 45.355 ms (5%) | 29.415 ms | 62.89 MiB (1%) | 98969 |
| `["shootout", "regex_dna"]` | 3.706 ms (5%) | 0.000 ns | 1.70 MiB (1%) | 306 |
| `["shootout", "revcomp"]` | 118.166 μs (25%) | 0.000 ns | 79.80 KiB (1%) | 888 |
| `["shootout", "spectralnorm"]` | 1.437 ms (5%) | 0.000 ns | 2.63 KiB (1%) | 3 |
| `["simd", "(\"auto_axpy!\", \"Float32\", 4095)"]` | 466.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_axpy!\", \"Float32\", 4096)"]` | 440.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_axpy!\", \"Float64\", 4095)"]` | 1.071 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_axpy!\", \"Float64\", 4096)"]` | 1.256 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_axpy!\", \"Int32\", 4095)"]` | 449.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_axpy!\", \"Int32\", 4096)"]` | 429.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_axpy!\", \"Int64\", 4095)"]` | 1.515 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_axpy!\", \"Int64\", 4096)"]` | 1.505 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Float32\", 4095)"]` | 1.814 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Float32\", 4096)"]` | 1.797 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Float64\", 4095)"]` | 3.583 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Float64\", 4096)"]` | 3.580 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Int32\", 4095)"]` | 361.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Int32\", 4096)"]` | 374.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Int64\", 4095)"]` | 700.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_conditional_loop!\", \"Int64\", 4096)"]` | 699.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_inner\", \"Int32\", 4095)"]` | 372.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_inner\", \"Int32\", 4096)"]` | 365.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_inner\", \"Int64\", 4095)"]` | 1.610 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_inner\", \"Int64\", 4096)"]` | 1.607 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4095)"]` | 30.090 μs (20%) | 0.000 ns | 107.77 KiB (1%) | 30 |
| `["simd", "(\"auto_local_arrays\", \"Float32\", 4096)"]` | 29.887 μs (20%) | 0.000 ns | 107.77 KiB (1%) | 30 |
| `["simd", "(\"auto_local_arrays\", \"Float64\", 4095)"]` | 38.388 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"auto_local_arrays\", \"Float64\", 4096)"]` | 38.242 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"auto_local_arrays\", \"Int32\", 4095)"]` | 28.518 μs (20%) | 0.000 ns | 108.00 KiB (1%) | 42 |
| `["simd", "(\"auto_local_arrays\", \"Int32\", 4096)"]` | 28.719 μs (20%) | 0.000 ns | 108.00 KiB (1%) | 42 |
| `["simd", "(\"auto_local_arrays\", \"Int64\", 4095)"]` | 41.051 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"auto_local_arrays\", \"Int64\", 4096)"]` | 37.132 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"auto_manual_example!\", \"Int32\", 4095)"]` | 641.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_manual_example!\", \"Int32\", 4096)"]` | 619.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_manual_example!\", \"Int64\", 4095)"]` | 1.451 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_manual_example!\", \"Int64\", 4096)"]` | 1.452 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_sum_reduce\", \"Int32\", 4095)"]` | 55.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_sum_reduce\", \"Int32\", 4096)"]` | 55.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_sum_reduce\", \"Int64\", 4095)"]` | 91.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_sum_reduce\", \"Int64\", 4096)"]` | 92.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_two_reductions\", \"Int32\", 4095)"]` | 4.396 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_two_reductions\", \"Int32\", 4096)"]` | 4.406 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_two_reductions\", \"Int64\", 4095)"]` | 954.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"auto_two_reductions\", \"Int64\", 4096)"]` | 895.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 520.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 446.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Float64\", 4095)"]` | 1.082 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Float64\", 4096)"]` | 1.247 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int32\", 4095)"]` | 451.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 433.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int64\", 4095)"]` | 1.511 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!\", \"Int64\", 4096)"]` | 1.504 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4095)"]` | 2.163 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Float32\", 4096)"]` | 2.166 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4095)"]` | 2.345 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Float64\", 4096)"]` | 2.336 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4095)"]` | 2.160 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Int32\", 4096)"]` | 2.160 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4095)"]` | 2.374 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"axpy!_aliased\", \"Int64\", 4096)"]` | 2.364 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4095)"]` | 1.813 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float32\", 4096)"]` | 1.798 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4095)"]` | 3.587 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Float64\", 4096)"]` | 3.585 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4095)"]` | 369.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 370.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 705.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4096)"]` | 696.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Float32\", 4095)"]` | 12.624 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Float32\", 4096)"]` | 12.626 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Float64\", 4095)"]` | 11.580 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Float64\", 4096)"]` | 11.581 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4095)"]` | 342.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Int32\", 4096)"]` | 370.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4095)"]` | 703.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"conditional_loop!_aliased\", \"Int64\", 4096)"]` | 703.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float32\", 4095)"]` | 423.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float32\", 4096)"]` | 382.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float64\", 4095)"]` | 712.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Float64\", 4096)"]` | 769.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int32\", 4095)"]` | 374.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int32\", 4096)"]` | 367.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int64\", 4095)"]` | 1.609 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner\", \"Int64\", 4096)"]` | 1.606 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Float32\", 4095)"]` | 253.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Float32\", 4096)"]` | 215.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Float64\", 4095)"]` | 645.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Float64\", 4096)"]` | 619.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Int32\", 4095)"]` | 294.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Int32\", 4096)"]` | 290.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Int64\", 4095)"]` | 1.608 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"inner_aliased\", \"Int64\", 4096)"]` | 1.606 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"local_arrays\", \"Float32\", 4095)"]` | 30.000 μs (20%) | 0.000 ns | 107.77 KiB (1%) | 30 |
| `["simd", "(\"local_arrays\", \"Float32\", 4096)"]` | 29.691 μs (20%) | 0.000 ns | 107.77 KiB (1%) | 30 |
| `["simd", "(\"local_arrays\", \"Float64\", 4095)"]` | 38.361 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"local_arrays\", \"Float64\", 4096)"]` | 38.261 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"local_arrays\", \"Int32\", 4095)"]` | 28.566 μs (20%) | 0.000 ns | 108.00 KiB (1%) | 42 |
| `["simd", "(\"local_arrays\", \"Int32\", 4096)"]` | 28.781 μs (20%) | 0.000 ns | 108.00 KiB (1%) | 42 |
| `["simd", "(\"local_arrays\", \"Int64\", 4095)"]` | 40.941 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"local_arrays\", \"Int64\", 4096)"]` | 37.885 μs (20%) | 0.000 ns | 155.86 KiB (1%) | 45 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 1.876 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 1.879 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 1.849 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 1.848 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.202 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.202 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.184 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Float64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.196 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 1.976 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 1.972 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 1.998 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int32\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.002 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4095)"]` | 2.230 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.ImmutableFields\", 4096)"]` | 2.229 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4095)"]` | 2.207 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"loop_fields!\", \"Int64\", \"BaseBenchmarks.SIMDBenchmarks.MutableFields\", 4096)"]` | 2.205 μs (20%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["simd", "(\"manual_example!\", \"Float32\", 4095)"]` | 700.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Float32\", 4096)"]` | 690.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Float64\", 4095)"]` | 1.409 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Float64\", 4096)"]` | 1.436 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int32\", 4095)"]` | 642.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int32\", 4096)"]` | 620.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int64\", 4095)"]` | 1.457 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!\", \"Int64\", 4096)"]` | 1.449 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Float32\", 4095)"]` | 5.264 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Float32\", 4096)"]` | 5.267 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Float64\", 4095)"]` | 5.270 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Float64\", 4096)"]` | 5.270 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Int32\", 4095)"]` | 2.453 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Int32\", 4096)"]` | 2.452 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Int64\", 4095)"]` | 2.686 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"manual_example!_aliased\", \"Int64\", 4096)"]` | 2.681 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float32\", 4095)"]` | 70.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float32\", 4096)"]` | 75.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float64\", 4095)"]` | 108.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Float64\", 4096)"]` | 107.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int32\", 4095)"]` | 54.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int32\", 4096)"]` | 53.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int64\", 4095)"]` | 92.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"sum_reduce\", \"Int64\", 4096)"]` | 92.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float32\", 4095)"]` | 563.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float32\", 4096)"]` | 537.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float64\", 4095)"]` | 1.083 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Float64\", 4096)"]` | 1.152 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int32\", 4095)"]` | 18.973 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int32\", 4096)"]` | 18.977 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int64\", 4095)"]` | 952.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions\", \"Int64\", 4096)"]` | 899.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Float32\", 4095)"]` | 490.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Float32\", 4096)"]` | 468.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Float64\", 4095)"]` | 865.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Float64\", 4096)"]` | 853.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Int32\", 4095)"]` | 18.922 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Int32\", 4096)"]` | 18.926 μs (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Int64\", 4095)"]` | 773.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["simd", "(\"two_reductions_aliased\", \"Int64\", 4096)"]` | 762.000 ns (20%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort forwards\", \"ascending\")"]` | 88.893 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort forwards\", \"descending\")"]` | 580.285 ms (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort forwards\", \"ones\")"]` | 130.548 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort forwards\", \"random\")"]` | 289.261 ms (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort reverse\", \"ascending\")"]` | 580.545 ms (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort reverse\", \"descending\")"]` | 74.027 μs (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort reverse\", \"ones\")"]` | 147.405 μs (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort reverse\", \"random\")"]` | 286.328 ms (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 49.152 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"descending\")"]` | 580.430 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ones\")"]` | 88.141 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort! forwards\", \"random\")"]` | 289.240 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 580.381 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 35.332 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 106.382 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 286.285 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ascending\")"]` | 116.978 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"descending\")"]` | 1.257 s (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"ones\")"]` | 192.779 μs (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "insertionsort", "(\"sortperm forwards\", \"random\")"]` | 922.343 ms (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ascending\")"]` | 1.257 s (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"descending\")"]` | 103.564 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"ones\")"]` | 208.601 μs (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "insertionsort", "(\"sortperm reverse\", \"random\")"]` | 876.909 ms (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 85.363 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 1.257 s (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 174.606 μs (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 922.886 ms (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.257 s (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 85.307 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 190.898 μs (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 880.329 ms (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sort", "issorted", "(\"forwards\", \"ascending\")"]` | 18.142 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"forwards\", \"descending\")"]` | 17.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"forwards\", \"ones\")"]` | 96.667 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"forwards\", \"random\")"]` | 18.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 94.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 18.641 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"reverse\", \"ones\")"]` | 92.851 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 92.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "mergesort", "(\"sort forwards\", \"ascending\")"]` | 451.358 μs (30%) | 0.000 ns | 586.17 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sort forwards\", \"descending\")"]` | 660.881 μs (30%) | 0.000 ns | 586.17 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sort forwards\", \"ones\")"]` | 493.472 μs (30%) | 0.000 ns | 586.25 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sort forwards\", \"random\")"]` | 2.799 ms (30%) | 0.000 ns | 586.25 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sort reverse\", \"ascending\")"]` | 633.206 μs (30%) | 0.000 ns | 586.19 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sort reverse\", \"descending\")"]` | 447.582 μs (30%) | 0.000 ns | 586.19 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sort reverse\", \"ones\")"]` | 516.304 μs (30%) | 0.000 ns | 586.27 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sort reverse\", \"random\")"]` | 2.846 ms (30%) | 0.000 ns | 586.27 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sort! forwards\", \"ascending\")"]` | 410.998 μs (30%) | 0.000 ns | 195.45 KiB (1%) | 2 |
| `["sort", "mergesort", "(\"sort! forwards\", \"descending\")"]` | 622.113 μs (30%) | 0.000 ns | 195.45 KiB (1%) | 2 |
| `["sort", "mergesort", "(\"sort! forwards\", \"ones\")"]` | 450.759 μs (30%) | 0.000 ns | 195.53 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sort! forwards\", \"random\")"]` | 2.756 ms (30%) | 0.000 ns | 195.53 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sort! reverse\", \"ascending\")"]` | 595.309 μs (30%) | 0.000 ns | 195.45 KiB (1%) | 2 |
| `["sort", "mergesort", "(\"sort! reverse\", \"descending\")"]` | 408.593 μs (30%) | 0.000 ns | 195.45 KiB (1%) | 2 |
| `["sort", "mergesort", "(\"sort! reverse\", \"ones\")"]` | 475.131 μs (30%) | 0.000 ns | 195.53 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sort! reverse\", \"random\")"]` | 2.806 ms (30%) | 0.000 ns | 195.53 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ascending\")"]` | 664.563 μs (30%) | 0.000 ns | 586.17 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"descending\")"]` | 923.910 μs (30%) | 0.000 ns | 586.17 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"ones\")"]` | 741.062 μs (30%) | 0.000 ns | 586.28 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm forwards\", \"random\")"]` | 3.684 ms (30%) | 0.000 ns | 586.28 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ascending\")"]` | 903.409 μs (30%) | 0.000 ns | 586.17 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"descending\")"]` | 653.766 μs (30%) | 0.000 ns | 586.17 KiB (1%) | 5 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"ones\")"]` | 765.019 μs (30%) | 0.000 ns | 586.28 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm reverse\", \"random\")"]` | 3.651 ms (30%) | 0.000 ns | 586.28 KiB (1%) | 8 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ascending\")"]` | 632.822 μs (30%) | 0.000 ns | 195.47 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"descending\")"]` | 893.195 μs (30%) | 0.000 ns | 195.47 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"ones\")"]` | 722.763 μs (30%) | 0.000 ns | 195.58 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sortperm! forwards\", \"random\")"]` | 3.662 ms (30%) | 0.000 ns | 195.58 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ascending\")"]` | 884.479 μs (30%) | 0.000 ns | 195.47 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"descending\")"]` | 634.513 μs (30%) | 0.000 ns | 195.47 KiB (1%) | 3 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"ones\")"]` | 744.024 μs (30%) | 0.000 ns | 195.58 KiB (1%) | 6 |
| `["sort", "mergesort", "(\"sortperm! reverse\", \"random\")"]` | 3.627 ms (30%) | 0.000 ns | 195.58 KiB (1%) | 6 |
| `["sort", "quicksort", "(\"sort forwards\", \"ascending\")"]` | 313.874 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort forwards\", \"descending\")"]` | 325.467 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort forwards\", \"ones\")"]` | 490.641 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort forwards\", \"random\")"]` | 2.215 ms (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort reverse\", \"ascending\")"]` | 337.733 μs (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort reverse\", \"descending\")"]` | 326.607 μs (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort reverse\", \"ones\")"]` | 494.811 μs (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort reverse\", \"random\")"]` | 2.251 ms (30%) | 0.000 ns | 390.73 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sort! forwards\", \"ascending\")"]` | 270.296 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sort! forwards\", \"descending\")"]` | 284.050 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sort! forwards\", \"ones\")"]` | 447.354 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sort! forwards\", \"random\")"]` | 2.171 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sort! reverse\", \"ascending\")"]` | 295.057 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sort! reverse\", \"descending\")"]` | 284.901 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sort! reverse\", \"ones\")"]` | 452.415 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sort! reverse\", \"random\")"]` | 2.208 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"ascending\")"]` | 644.494 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"descending\")"]` | 659.760 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"ones\")"]` | 775.958 μs (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "quicksort", "(\"sortperm forwards\", \"random\")"]` | 3.197 ms (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"ascending\")"]` | 645.340 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"descending\")"]` | 629.831 μs (30%) | 0.000 ns | 390.72 KiB (1%) | 3 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"ones\")"]` | 796.727 μs (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "quicksort", "(\"sortperm reverse\", \"random\")"]` | 3.179 ms (30%) | 0.000 ns | 390.75 KiB (1%) | 5 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ascending\")"]` | 612.463 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"descending\")"]` | 627.966 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 757.354 μs (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 3.177 ms (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ascending\")"]` | 627.303 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"descending\")"]` | 611.907 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 777.322 μs (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 3.160 ms (30%) | 0.000 ns | 48 bytes (1%) | 3 |
| `["sparse", "arithmetic", "(\"unary minus\", (20000, 20000))"]` | 43.386 ms (30%) | 31.039 ms | 61.18 MiB (1%) | 8 |
| `["sparse", "arithmetic", "(\"unary minus\", (600, 600))"]` | 5.581 μs (30%) | 0.000 ns | 60.59 KiB (1%) | 7 |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 471.000 ns (5%) | 0.000 ns | 2.19 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 2.294 μs (5%) | 0.000 ns | 14.84 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"Bidiagonal\", 1000)"]` | 23.530 μs (5%) | 0.000 ns | 134.30 KiB (1%) | 15 |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 95.000 ns (5%) | 0.000 ns | 544 bytes (1%) | 4 |
| `["sparse", "constructors", "(\"Diagonal\", 100)"]` | 148.000 ns (5%) | 0.000 ns | 2.67 KiB (1%) | 4 |
| `["sparse", "constructors", "(\"Diagonal\", 1000)"]` | 2.204 μs (5%) | 0.000 ns | 23.92 KiB (1%) | 4 |
| `["sparse", "constructors", "(\"IJV\", 10)"]` | 85.000 ns (5%) | 0.000 ns | 304 bytes (1%) | 4 |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 427.000 ns (5%) | 0.000 ns | 2.08 KiB (1%) | 10 |
| `["sparse", "constructors", "(\"IJV\", 1000)"]` | 6.433 μs (5%) | 0.000 ns | 27.39 KiB (1%) | 12 |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 82.000 ns (5%) | 0.000 ns | 192 bytes (1%) | 3 |
| `["sparse", "constructors", "(\"IV\", 100)"]` | 282.000 ns (5%) | 0.000 ns | 528 bytes (1%) | 7 |
| `["sparse", "constructors", "(\"IV\", 1000)"]` | 1.945 μs (5%) | 0.000 ns | 4.44 KiB (1%) | 8 |
| `["sparse", "constructors", "(\"SymTridiagonal\", 10)"]` | 568.000 ns (5%) | 0.000 ns | 2.81 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 4.432 μs (5%) | 0.000 ns | 20.20 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"SymTridiagonal\", 1000)"]` | 34.404 μs (5%) | 0.000 ns | 188.78 KiB (1%) | 22 |
| `["sparse", "constructors", "(\"Tridiagonal\", 10)"]` | 572.000 ns (5%) | 0.000 ns | 2.81 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"Tridiagonal\", 100)"]` | 4.310 μs (5%) | 0.000 ns | 20.20 KiB (1%) | 13 |
| `["sparse", "constructors", "(\"Tridiagonal\", 1000)"]` | 34.201 μs (5%) | 0.000 ns | 188.75 KiB (1%) | 20 |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 10)"]` | 145.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 100)"]` | 2.184 μs (30%) | 0.000 ns | 16.67 KiB (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"OneTo\", 1000)"]` | 57.783 μs (30%) | 0.000 ns | 501.95 KiB (1%) | 6 |
| `["sparse", "index", "(\"spmat\", \"array\", 10)"]` | 2.114 μs (30%) | 0.000 ns | 3.50 KiB (1%) | 38 |
| `["sparse", "index", "(\"spmat\", \"array\", 100)"]` | 50.810 μs (30%) | 0.000 ns | 40.13 KiB (1%) | 311 |
| `["sparse", "index", "(\"spmat\", \"array\", 1000)"]` | 1.107 ms (30%) | 0.000 ns | 727.84 KiB (1%) | 3013 |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 10)"]` | 89.000 ns (30%) | 0.000 ns | 352 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 100)"]` | 93.000 ns (30%) | 0.000 ns | 416 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 1000)"]` | 129.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 10)"]` | 641.000 ns (30%) | 0.000 ns | 1.55 KiB (1%) | 16 |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 100)"]` | 1.694 μs (30%) | 0.000 ns | 3.78 KiB (1%) | 16 |
| `["sparse", "index", "(\"spmat\", \"col\", \"array\", 1000)"]` | 25.824 μs (30%) | 0.000 ns | 26.22 KiB (1%) | 16 |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 10)"]` | 206.000 ns (30%) | 0.000 ns | 784 bytes (1%) | 8 |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 100)"]` | 427.000 ns (30%) | 0.000 ns | 1.95 KiB (1%) | 8 |
| `["sparse", "index", "(\"spmat\", \"col\", \"logical\", 1000)"]` | 3.407 μs (30%) | 0.000 ns | 12.67 KiB (1%) | 8 |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 90.000 ns (30%) | 0.000 ns | 352 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 100)"]` | 94.000 ns (30%) | 0.000 ns | 416 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 1000)"]` | 135.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"integer\", 10)"]` | 20.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spmat\", \"integer\", 100)"]` | 23.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spmat\", \"integer\", 1000)"]` | 26.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spmat\", \"logical\", 10)"]` | 245.000 ns (30%) | 0.000 ns | 816 bytes (1%) | 7 |
| `["sparse", "index", "(\"spmat\", \"logical\", 100)"]` | 6.130 μs (30%) | 0.000 ns | 7.02 KiB (1%) | 7 |
| `["sparse", "index", "(\"spmat\", \"logical\", 1000)"]` | 131.312 μs (30%) | 0.000 ns | 142.45 KiB (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"range\", 10)"]` | 149.000 ns (30%) | 0.000 ns | 896 bytes (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"range\", 100)"]` | 2.119 μs (30%) | 0.000 ns | 16.67 KiB (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"range\", 1000)"]` | 57.750 μs (30%) | 0.000 ns | 501.95 KiB (1%) | 6 |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 10)"]` | 129.000 ns (30%) | 0.000 ns | 288 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 100)"]` | 611.000 ns (30%) | 0.000 ns | 736 bytes (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 1000)"]` | 10.445 μs (30%) | 0.000 ns | 2.44 KiB (1%) | 13 |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 159.000 ns (30%) | 0.000 ns | 320 bytes (1%) | 6 |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 679.000 ns (30%) | 0.000 ns | 768 bytes (1%) | 10 |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 11.373 μs (30%) | 0.000 ns | 2.47 KiB (1%) | 14 |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 158.000 ns (30%) | 0.000 ns | 448 bytes (1%) | 7 |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 562.000 ns (30%) | 0.000 ns | 1.00 KiB (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 5.003 μs (30%) | 0.000 ns | 5.47 KiB (1%) | 13 |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 10)"]` | 130.000 ns (30%) | 0.000 ns | 288 bytes (1%) | 5 |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 100)"]` | 601.000 ns (30%) | 0.000 ns | 736 bytes (1%) | 9 |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 12.096 μs (30%) | 0.000 ns | 2.44 KiB (1%) | 13 |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 88.000 ns (30%) | 0.000 ns | 208 bytes (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 187.000 ns (30%) | 0.000 ns | 208 bytes (1%) | 4 |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 974.787 μs (30%) | 0.000 ns | 368 bytes (1%) | 4 |
| `["sparse", "index", "(\"spvec\", \"array\", 1000)"]` | 26.359 μs (30%) | 0.000 ns | 26.59 KiB (1%) | 18 |
| `["sparse", "index", "(\"spvec\", \"array\", 10000)"]` | 548.172 μs (30%) | 0.000 ns | 239.58 KiB (1%) | 21 |
| `["sparse", "index", "(\"spvec\", \"array\", 100000)"]` | 7.316 ms (30%) | 0.000 ns | 2.30 MiB (1%) | 21 |
| `["sparse", "index", "(\"spvec\", \"integer\", 1000)"]` | 18.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spvec\", \"integer\", 10000)"]` | 20.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spvec\", \"integer\", 100000)"]` | 21.000 ns (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "index", "(\"spvec\", \"logical\", 1000)"]` | 2.649 μs (30%) | 0.000 ns | 4.94 KiB (1%) | 9 |
| `["sparse", "index", "(\"spvec\", \"logical\", 10000)"]` | 49.946 μs (30%) | 0.000 ns | 39.98 KiB (1%) | 10 |
| `["sparse", "index", "(\"spvec\", \"logical\", 100000)"]` | 484.992 μs (30%) | 0.000 ns | 394.77 KiB (1%) | 10 |
| `["sparse", "index", "(\"spvec\", \"range\", 1000)"]` | 146.000 ns (30%) | 0.000 ns | 832 bytes (1%) | 3 |
| `["sparse", "index", "(\"spvec\", \"range\", 10000)"]` | 263.000 ns (30%) | 0.000 ns | 2.00 KiB (1%) | 3 |
| `["sparse", "index", "(\"spvec\", \"range\", 100000)"]` | 845.000 ns (30%) | 0.000 ns | 5.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 5.345 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x40, sparse 40x400 -> dense 400x400\")"]` | 5.488 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 5.139 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 53.047 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 6.768 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x400, sparse 400x4000 -> dense 40x4000\")"]` | 61.454 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x400 -> dense 40x400\")"]` | 55.819 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 593.899 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 133.153 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x400, dense 400x40 -> dense 4000x40\")"]` | 433.719 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 3.468 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x40, dense 40x400 -> dense 400x400\")"]` | 359.340 μs (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 2.992 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 400x4000, dense 4000x40 -> dense 400x40\")"]` | 3.190 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 2.370 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 2.923 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 13.366 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x5, sparse 5x50 -> dense 50x50\")"]` | 13.822 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 1.432 μs (30%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 13.272 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 19.195 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x50, sparse 50x500 -> dense 5x500\")"]` | 19.064 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x50 -> dense 5x50\")"]` | 1.450 μs (30%) | 0.000 ns | 2.13 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_B\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 19.499 μs (30%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 3.213 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 500x50, dense 50x5 -> dense 500x5\")"]` | 4.716 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 20.492 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x5, dense 5x50 -> dense 50x50\")"]` | 4.627 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 18.798 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 50x500, dense 500x5 -> dense 50x5\")"]` | 17.538 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 19.300 μs (30%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"A_mul_B\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 17.057 μs (30%) | 0.000 ns | 4.06 KiB (1%) | 1 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 2000x20, sparse 20x20 -> dense 2000x20\")"]` | 953.110 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x20, sparse 200x20 -> dense 200x200\")"]` | 1.102 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 9.012 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 838.515 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.672 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x200, sparse 2000x200 -> dense 20x2000\")"]` | 10.822 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 2000x2000 -> dense 20x2000\")"]` | 93.757 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"dense 20x2000, sparse 200x2000 -> dense 20x200\")"]` | 8.558 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x20, dense 20x20 -> dense 2000x20\")"]` | 944.293 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x200, dense 20x200 -> dense 2000x20\")"]` | 8.942 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 89.363 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x20, dense 200x20 -> dense 200x200\")"]` | 906.968 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 8.645 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 200x2000, dense 20x2000 -> dense 200x20\")"]` | 9.090 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 916.735 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc!\", \"sparse 20x200, dense 200x200 -> dense 20x200\")"]` | 955.720 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 457.118 μs (30%) | 0.000 ns | 217.13 KiB (1%) | 26 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 428.587 μs (30%) | 0.000 ns | 146.42 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 528.402 μs (30%) | 0.000 ns | 139.75 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 30.772 μs (30%) | 0.000 ns | 27.75 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.992 ms (30%) | 0.000 ns | 239.92 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 2.132 ms (30%) | 0.000 ns | 231.20 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 4.268 ms (30%) | 0.000 ns | 234.78 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 223.459 μs (30%) | 0.000 ns | 32.63 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 41.656 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 238.403 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.332 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 22.158 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 133.581 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 250.548 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 34.852 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bc\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 17.570 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 4000x40, sparse 40x40 -> dense 4000x40\")"]` | 5.411 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x40, sparse 400x40 -> dense 400x400\")"]` | 6.578 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 50.694 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 4.959 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 10.307 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x400, sparse 4000x400 -> dense 40x4000\")"]` | 68.973 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 4000x4000 -> dense 40x4000\")"]` | 567.730 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"dense 40x4000, sparse 400x4000 -> dense 40x400\")"]` | 50.143 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x40, dense 40x40 -> dense 4000x40\")"]` | 7.353 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x400, dense 40x400 -> dense 4000x40\")"]` | 70.897 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 708.494 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x40, dense 400x40 -> dense 400x400\")"]` | 7.102 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 68.576 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 400x4000, dense 40x4000 -> dense 400x40\")"]` | 71.920 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 7.164 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt!\", \"sparse 40x400, dense 400x400 -> dense 40x400\")"]` | 7.636 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 500x5, sparse 5x5 -> dense 500x5\")"]` | 326.021 μs (30%) | 0.000 ns | 145.22 KiB (1%) | 26 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x5, sparse 50x5 -> dense 50x50\")"]` | 307.988 μs (30%) | 0.000 ns | 197.94 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 382.734 μs (30%) | 0.000 ns | 188.84 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 22.431 μs (30%) | 0.000 ns | 9.72 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.105 ms (30%) | 0.000 ns | 224.44 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x50, sparse 500x50 -> dense 5x500\")"]` | 1.264 ms (30%) | 0.000 ns | 216.31 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 500x500 -> dense 5x500\")"]` | 2.843 ms (30%) | 0.000 ns | 219.69 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"dense 5x500, sparse 50x500 -> dense 5x50\")"]` | 165.288 μs (30%) | 0.000 ns | 22.22 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x5, dense 5x5 -> dense 500x5\")"]` | 32.912 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x50, dense 5x50 -> dense 500x5\")"]` | 220.578 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.162 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x5, dense 50x5 -> dense 50x50\")"]` | 20.541 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 130.040 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 50x500, dense 5x500 -> dense 50x5\")"]` | 232.122 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 26.049 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"A_mul_Bt\", \"sparse 5x50, dense 50x50 -> dense 5x50\")"]` | 15.992 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x200 -> dense 20x200\")"]` | 38.844 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 389.408 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x20, sparse 200x2000 -> dense 20x2000\")"]` | 42.302 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x20 -> dense 200x20\")"]` | 4.046 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 41.885 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x20, sparse 20x2000 -> dense 20x2000\")"]` | 7.476 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x200, sparse 20x200 -> dense 200x200\")"]` | 6.906 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 4.365 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x200, dense 2000x20 -> dense 200x20\")"]` | 494.530 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 2000x2000, dense 2000x20 -> dense 2000x20\")"]` | 677.315 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 445.188 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 574.729 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 200x2000, dense 200x20 -> dense 2000x20\")"]` | 164.936 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x20, dense 20x2000 -> dense 20x2000\")"]` | 495.309 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x200, dense 20x200 -> dense 200x200\")"]` | 138.519 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 96.272 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 523.048 μs (30%) | 0.000 ns | 32.30 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 6.208 ms (30%) | 0.000 ns | 234.45 KiB (1%) | 9 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.697 ms (30%) | 0.000 ns | 230.88 KiB (1%) | 9 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 71.500 μs (30%) | 0.000 ns | 27.42 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 1.115 ms (30%) | 0.000 ns | 139.42 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 1.236 ms (30%) | 0.000 ns | 239.59 KiB (1%) | 9 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 619.653 μs (30%) | 0.000 ns | 146.09 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 542.669 μs (30%) | 0.000 ns | 216.80 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 14.760 μs (30%) | 0.000 ns | 4.08 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 24.602 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 13.552 μs (30%) | 0.000 ns | 4.08 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 21.337 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 8.715 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 22.141 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 8.680 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"Ac_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 7.667 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 2000x2000 -> dense 20x2000\")"]` | 95.172 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 2000x20, sparse 200x2000 -> dense 20x200\")"]` | 8.699 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x20, sparse 2000x200 -> dense 20x2000\")"]` | 10.963 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 200x200 -> dense 200x200\")"]` | 9.086 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 200x200, sparse 20x200 -> dense 200x20\")"]` | 849.325 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x20, sparse 2000x20 -> dense 20x2000\")"]` | 1.694 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x200, sparse 200x20 -> dense 200x200\")"]` | 1.119 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"dense 20x2000, sparse 20x20 -> dense 2000x20\")"]` | 974.574 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x200, dense 20x2000 -> dense 200x20\")"]` | 10.717 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 2000x2000, dense 20x2000 -> dense 2000x20\")"]` | 96.108 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x20, dense 200x200 -> dense 20x200\")"]` | 1.314 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x200, dense 200x200 -> dense 200x200\")"]` | 9.233 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 200x2000, dense 20x200 -> dense 2000x20\")"]` | 8.314 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x20, dense 2000x20 -> dense 20x2000\")"]` | 939.366 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x200, dense 200x20 -> dense 200x200\")"]` | 865.844 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc!\", \"sparse 20x2000, dense 20x20 -> dense 2000x20\")"]` | 860.687 μs (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 4.393 ms (30%) | 0.000 ns | 234.78 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 237.409 μs (30%) | 0.000 ns | 32.63 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 2.149 ms (30%) | 0.000 ns | 231.20 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 529.064 μs (30%) | 0.000 ns | 139.75 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 31.285 μs (30%) | 0.000 ns | 27.75 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 2.004 ms (30%) | 0.000 ns | 239.92 KiB (1%) | 15 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 430.288 μs (30%) | 0.000 ns | 146.42 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 464.674 μs (30%) | 0.000 ns | 217.13 KiB (1%) | 26 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 353.575 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.423 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 20.394 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 135.105 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 204.869 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 43.767 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 23.089 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"Ac_mul_Bc\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 44.155 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x400 -> dense 40x400\")"]` | 267.714 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 2.677 s (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x40, sparse 400x4000 -> dense 40x4000\")"]` | 287.026 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x40 -> dense 400x40\")"]` | 28.592 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 286.870 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x40, sparse 40x4000 -> dense 40x4000\")"]` | 48.031 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x400, sparse 40x400 -> dense 400x400\")"]` | 47.765 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 34.127 ms (30%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x400, dense 4000x40 -> dense 400x40\")"]` | 2.672 ms (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 4000x4000, dense 4000x40 -> dense 4000x40\")"]` | 3.396 ms (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 2.232 ms (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 2.827 ms (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 400x4000, dense 400x40 -> dense 4000x40\")"]` | 720.315 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x40, dense 40x4000 -> dense 40x4000\")"]` | 2.375 ms (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x400, dense 40x400 -> dense 400x400\")"]` | 612.773 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 405.827 μs (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x50 -> dense 5x50\")"]` | 379.883 μs (30%) | 0.000 ns | 21.89 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 4.365 ms (30%) | 0.000 ns | 219.36 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x5, sparse 50x500 -> dense 5x500\")"]` | 1.157 ms (30%) | 0.000 ns | 215.98 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x5 -> dense 50x5\")"]` | 54.519 μs (30%) | 0.000 ns | 18.52 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 828.707 μs (30%) | 0.000 ns | 93.39 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x5, sparse 5x500 -> dense 5x500\")"]` | 798.501 μs (30%) | 0.000 ns | 224.11 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x50, sparse 5x50 -> dense 50x50\")"]` | 471.478 μs (30%) | 0.000 ns | 97.98 KiB (1%) | 12 |
| `["sparse", "matmul", "(\"At_mul_B\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 388.791 μs (30%) | 0.000 ns | 144.89 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x50, dense 500x5 -> dense 50x5\")"]` | 12.714 μs (30%) | 0.000 ns | 4.08 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 500x500, dense 500x5 -> dense 500x5\")"]` | 20.753 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 12.061 μs (30%) | 0.000 ns | 4.08 KiB (1%) | 2 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 18.701 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 50x500, dense 50x5 -> dense 500x5\")"]` | 8.400 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x5, dense 5x500 -> dense 5x500\")"]` | 19.570 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x50, dense 5x50 -> dense 50x50\")"]` | 8.268 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"At_mul_B\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 7.244 μs (30%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 4000x4000 -> dense 40x4000\")"]` | 558.777 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 4000x40, sparse 400x4000 -> dense 40x400\")"]` | 51.629 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x40, sparse 4000x400 -> dense 40x4000\")"]` | 68.001 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 400x400 -> dense 400x400\")"]` | 49.688 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 400x400, sparse 40x400 -> dense 400x40\")"]` | 4.679 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x40, sparse 4000x40 -> dense 40x4000\")"]` | 10.233 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x400, sparse 400x40 -> dense 400x400\")"]` | 6.497 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"dense 40x4000, sparse 40x40 -> dense 4000x40\")"]` | 5.254 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x400, dense 40x4000 -> dense 400x40\")"]` | 83.156 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 4000x4000, dense 40x4000 -> dense 4000x40\")"]` | 720.735 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x40, dense 400x400 -> dense 40x400\")"]` | 9.996 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x400, dense 400x400 -> dense 400x400\")"]` | 72.325 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 400x4000, dense 40x400 -> dense 4000x40\")"]` | 67.151 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x40, dense 4000x40 -> dense 40x4000\")"]` | 7.179 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x400, dense 400x40 -> dense 400x400\")"]` | 7.166 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt!\", \"sparse 40x4000, dense 40x40 -> dense 4000x40\")"]` | 6.237 ms (30%) | 0.000 ns | 336 bytes (1%) | 6 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 500x500 -> dense 5x500\")"]` | 2.819 ms (30%) | 0.000 ns | 219.69 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 500x5, sparse 50x500 -> dense 5x50\")"]` | 162.230 μs (30%) | 0.000 ns | 22.22 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x5, sparse 500x50 -> dense 5x500\")"]` | 1.261 ms (30%) | 0.000 ns | 216.31 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 50x50 -> dense 50x50\")"]` | 379.763 μs (30%) | 0.000 ns | 188.84 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 50x50, sparse 5x50 -> dense 50x5\")"]` | 21.110 μs (30%) | 0.000 ns | 9.72 KiB (1%) | 18 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x5, sparse 500x5 -> dense 5x500\")"]` | 1.104 ms (30%) | 0.000 ns | 224.44 KiB (1%) | 14 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x50, sparse 50x5 -> dense 50x50\")"]` | 307.461 μs (30%) | 0.000 ns | 197.94 KiB (1%) | 20 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"dense 5x500, sparse 5x5 -> dense 500x5\")"]` | 325.589 μs (30%) | 0.000 ns | 145.22 KiB (1%) | 26 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x50, dense 5x500 -> dense 50x5\")"]` | 319.202 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 500x500, dense 5x500 -> dense 500x5\")"]` | 2.088 ms (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x5, dense 50x50 -> dense 5x50\")"]` | 16.970 μs (30%) | 0.000 ns | 4.39 KiB (1%) | 7 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x50, dense 50x50 -> dense 50x50\")"]` | 128.871 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 50x500, dense 5x50 -> dense 500x5\")"]` | 171.546 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x5, dense 500x5 -> dense 5x500\")"]` | 25.992 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x50, dense 50x5 -> dense 50x50\")"]` | 19.742 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "matmul", "(\"At_mul_Bt\", \"sparse 5x500, dense 5x5 -> dense 500x5\")"]` | 26.775 μs (30%) | 0.000 ns | 39.47 KiB (1%) | 8 |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 10000))"]` | 33.879 ms (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"adjoint!\", (20000, 20000))"]` | 62.928 ms (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"adjoint!\", (600, 400))"]` | 11.402 μs (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"adjoint!\", (600, 600))"]` | 18.527 μs (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"adjoint\", (20000, 10000))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"adjoint\", (20000, 20000))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"adjoint\", (600, 400))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"adjoint\", (600, 600))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose!\", (20000, 10000))"]` | 29.898 ms (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose!\", (20000, 20000))"]` | 60.266 ms (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose!\", (600, 400))"]` | 9.296 μs (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose!\", (600, 600))"]` | 15.998 μs (30%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose\", (20000, 10000))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose\", (20000, 20000))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose\", (600, 400))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["sparse", "transpose", "(\"transpose\", (600, 600))"]` | 17.000 ns (30%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["string", "findfirst", "Char"]` | 16.967 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string", "findfirst", "String"]` | 30.319 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string", "join"]` | 145.064 ms (40%) | 0.000 ns | 156.27 MiB (1%) | 21 |
| `["string", "readuntil", "backtracking"]` | 526.629 μs (5%) | 0.000 ns | 105.78 KiB (1%) | 20 |
| `["string", "readuntil", "barbarian backtrack"]` | 508.954 μs (5%) | 0.000 ns | 73.77 KiB (1%) | 19 |
| `["string", "readuntil", "no backtracking"]` | 349.529 μs (5%) | 0.000 ns | 66.58 KiB (1%) | 18 |
| `["string", "readuntil", "target length 1"]` | 47.561 ns (5%) | 0.000 ns | 160 bytes (1%) | 2 |
| `["string", "readuntil", "target length 1000"]` | 2.611 μs (5%) | 0.000 ns | 112 bytes (1%) | 3 |
| `["string", "readuntil", "target length 2"]` | 43.757 ns (5%) | 0.000 ns | 112 bytes (1%) | 3 |
| `["string", "readuntil", "target length 50000"]` | 127.737 μs (5%) | 0.000 ns | 112 bytes (1%) | 3 |
| `["string", "replace"]` | 149.313 μs (5%) | 0.000 ns | 12.09 KiB (1%) | 7 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 3, Float32)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 3, Float64)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 30, Float32)"]` | 30.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 30, Float64)"]` | 32.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 60, Float32)"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 60, Float64)"]` | 56.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 8, Float32)"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"NTuple\", 8, Float64)"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 3, Float32)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 3, Float64)"]` | 14.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 30, Float32)"]` | 30.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 30, Float64)"]` | 32.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 60, Float32)"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 60, Float64)"]` | 58.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 8, Float32)"]` | 16.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "index", "(\"sumelt\", \"TupleWrapper\", 8, Float64)"]` | 18.000 ns (40%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (16, 16), (16, 16))"]` | 1.480 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (2, 2), (2, 2))"]` | 21.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (4, 4), (4, 4))"]` | 29.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matmat\", (8, 8), (8, 8))"]` | 76.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (16, 16), (16,))"]` | 52.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (2, 2), (2,))"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (4, 4), (4,))"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "linear algebra", "(\"matvec\", (8, 8), (8,))"]` | 30.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "misc", "11899"]` | 1.548 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (16, 16))"]` | 470.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (16,))"]` | 42.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (2, 2))"]` | 18.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (2,))"]` | 15.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (4, 4))"]` | 40.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (4,))"]` | 17.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (8, 8))"]` | 129.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"minimum\", (8,))"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 43.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (16,))"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (2, 2))"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (2,))"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 25.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (4,))"]` | 20.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (8, 8))"]` | 45.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sum\", (8,))"]` | 23.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (16, 16))"]` | 210.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (16,))"]` | 22.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (2, 2))"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (2,))"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (4, 4))"]` | 24.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (4,))"]` | 14.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (8, 8))"]` | 60.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["tuple", "reduction", "(\"sumabs\", (8,))"]` | 19.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, false))"]` | 834.358 μs (5%) | 0.000 ns | 1.14 MiB (1%) | 20008 |
| `["union", "array", "(\"broadcast\", *, BigFloat, (false, true))"]` | 1.351 ms (5%) | 0.000 ns | 1.11 MiB (1%) | 17844 |
| `["union", "array", "(\"broadcast\", *, BigFloat, (true, true))"]` | 1.341 ms (5%) | 0.000 ns | 1.11 MiB (1%) | 17844 |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, false))"]` | 1.194 ms (5%) | 0.000 ns | 703.39 KiB (1%) | 30008 |
| `["union", "array", "(\"broadcast\", *, BigInt, (false, true))"]` | 1.692 ms (5%) | 0.000 ns | 713.91 KiB (1%) | 26761 |
| `["union", "array", "(\"broadcast\", *, BigInt, (true, true))"]` | 1.696 ms (5%) | 0.000 ns | 713.91 KiB (1%) | 26761 |
| `["union", "array", "(\"broadcast\", *, Bool, (false, false))"]` | 107.571 μs (5%) | 0.000 ns | 1.55 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", *, Bool, (false, true))"]` | 651.569 μs (5%) | 0.000 ns | 21.19 KiB (1%) | 10 |
| `["union", "array", "(\"broadcast\", *, Bool, (true, true))"]` | 650.769 μs (5%) | 0.000 ns | 21.19 KiB (1%) | 10 |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, false))"]` | 107.247 μs (5%) | 0.000 ns | 156.55 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (false, true))"]` | 678.269 μs (5%) | 0.000 ns | 322.88 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Complex{Float64}, (true, true))"]` | 678.227 μs (5%) | 0.000 ns | 322.88 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Float32, (false, false))"]` | 96.360 μs (5%) | 0.000 ns | 39.34 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", *, Float32, (false, true))"]` | 649.119 μs (5%) | 0.000 ns | 88.39 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Float32, (true, true))"]` | 649.820 μs (5%) | 0.000 ns | 88.39 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Float64, (false, false))"]` | 93.078 μs (5%) | 0.000 ns | 78.41 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", *, Float64, (false, true))"]` | 655.276 μs (5%) | 0.000 ns | 166.52 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Float64, (true, true))"]` | 654.975 μs (5%) | 0.000 ns | 166.52 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Int64, (false, false))"]` | 96.218 μs (5%) | 0.000 ns | 78.41 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", *, Int64, (false, true))"]` | 656.348 μs (5%) | 0.000 ns | 166.52 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Int64, (true, true))"]` | 658.700 μs (5%) | 0.000 ns | 166.52 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", *, Int8, (false, false))"]` | 95.314 μs (5%) | 0.000 ns | 10.13 KiB (1%) | 7 |
| `["union", "array", "(\"broadcast\", *, Int8, (false, true))"]` | 654.333 μs (5%) | 0.000 ns | 29.77 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", *, Int8, (true, true))"]` | 658.494 μs (5%) | 0.000 ns | 29.77 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", abs, BigFloat, false)"]` | 371.819 μs (5%) | 0.000 ns | 1.14 MiB (1%) | 20007 |
| `["union", "array", "(\"broadcast\", abs, BigFloat, true)"]` | 912.141 μs (5%) | 0.000 ns | 1.11 MiB (1%) | 17843 |
| `["union", "array", "(\"broadcast\", abs, BigInt, false)"]` | 536.662 μs (5%) | 0.000 ns | 312.14 KiB (1%) | 14971 |
| `["union", "array", "(\"broadcast\", abs, BigInt, true)"]` | 1.331 ms (5%) | 0.000 ns | 364.14 KiB (1%) | 13296 |
| `["union", "array", "(\"broadcast\", abs, Bool, false)"]` | 81.466 μs (5%) | 0.000 ns | 1.48 KiB (1%) | 7 |
| `["union", "array", "(\"broadcast\", abs, Bool, true)"]` | 665.661 μs (5%) | 0.000 ns | 21.13 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, false)"]` | 129.019 μs (5%) | 0.000 ns | 78.34 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", abs, Complex{Float64}, true)"]` | 774.966 μs (5%) | 0.000 ns | 166.47 KiB (1%) | 17 |
| `["union", "array", "(\"broadcast\", abs, Float32, false)"]` | 72.349 μs (5%) | 0.000 ns | 39.28 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", abs, Float32, true)"]` | 659.538 μs (5%) | 0.000 ns | 88.33 KiB (1%) | 16 |
| `["union", "array", "(\"broadcast\", abs, Float64, false)"]` | 74.483 μs (5%) | 0.000 ns | 78.34 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", abs, Float64, true)"]` | 679.833 μs (5%) | 0.000 ns | 166.45 KiB (1%) | 16 |
| `["union", "array", "(\"broadcast\", abs, Int64, false)"]` | 75.053 μs (5%) | 0.000 ns | 78.34 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", abs, Int64, true)"]` | 660.733 μs (5%) | 0.000 ns | 166.45 KiB (1%) | 16 |
| `["union", "array", "(\"broadcast\", abs, Int8, false)"]` | 72.208 μs (5%) | 0.000 ns | 10.06 KiB (1%) | 6 |
| `["union", "array", "(\"broadcast\", abs, Int8, true)"]` | 642.851 μs (5%) | 0.000 ns | 29.70 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", identity, BigFloat, false)"]` | 89.236 μs (5%) | 0.000 ns | 78.33 KiB (1%) | 7 |
| `["union", "array", "(\"broadcast\", identity, BigFloat, true)"]` | 701.000 μs (5%) | 0.000 ns | 156.53 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", identity, BigInt, false)"]` | 113.210 μs (5%) | 0.000 ns | 78.33 KiB (1%) | 7 |
| `["union", "array", "(\"broadcast\", identity, BigInt, true)"]` | 760.786 μs (5%) | 0.000 ns | 156.53 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", identity, Bool, false)"]` | 81.480 μs (5%) | 0.000 ns | 1.48 KiB (1%) | 7 |
| `["union", "array", "(\"broadcast\", identity, Bool, true)"]` | 662.144 μs (5%) | 0.000 ns | 21.13 KiB (1%) | 9 |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, false)"]` | 74.436 μs (5%) | 0.000 ns | 156.48 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", identity, Complex{Float64}, true)"]` | 653.474 μs (5%) | 0.000 ns | 322.81 KiB (1%) | 16 |
| `["union", "array", "(\"broadcast\", identity, Float32, false)"]` | 69.840 μs (5%) | 0.000 ns | 39.28 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", identity, Float32, true)"]` | 648.619 μs (5%) | 0.000 ns | 88.33 KiB (1%) | 16 |
| `["union", "array", "(\"broadcast\", identity, Float64, false)"]` | 70.122 μs (5%) | 0.000 ns | 78.34 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", identity, Float64, true)"]` | 664.762 μs (5%) | 0.000 ns | 166.45 KiB (1%) | 16 |
| `["union", "array", "(\"broadcast\", identity, Int64, false)"]` | 70.019 μs (5%) | 0.000 ns | 78.34 KiB (1%) | 8 |
| `["union", "array", "(\"broadcast\", identity, Int64, true)"]` | 652.212 μs (5%) | 0.000 ns | 166.45 KiB (1%) | 16 |
| `["union", "array", "(\"broadcast\", identity, Int8, false)"]` | 71.046 μs (5%) | 0.000 ns | 10.06 KiB (1%) | 6 |
| `["union", "array", "(\"broadcast\", identity, Int8, true)"]` | 655.674 μs (5%) | 0.000 ns | 29.70 KiB (1%) | 8 |
| `["union", "array", "(\"map\", *, BigFloat, (false, false))"]` | 748.397 μs (5%) | 0.000 ns | 1.14 MiB (1%) | 20004 |
| `["union", "array", "(\"map\", *, BigFloat, (false, true))"]` | 707.604 μs (5%) | 0.000 ns | 1.11 MiB (1%) | 17841 |
| `["union", "array", "(\"map\", *, BigFloat, (true, true))"]` | 687.392 μs (5%) | 0.000 ns | 1.11 MiB (1%) | 17841 |
| `["union", "array", "(\"map\", *, BigInt, (false, false))"]` | 1.121 ms (5%) | 0.000 ns | 703.25 KiB (1%) | 30004 |
| `["union", "array", "(\"map\", *, BigInt, (false, true))"]` | 1.002 ms (5%) | 0.000 ns | 713.80 KiB (1%) | 26758 |
| `["union", "array", "(\"map\", *, BigInt, (true, true))"]` | 1.006 ms (5%) | 0.000 ns | 713.80 KiB (1%) | 26758 |
| `["union", "array", "(\"map\", *, Bool, (false, false))"]` | 18.319 μs (5%) | 0.000 ns | 9.98 KiB (1%) | 3 |
| `["union", "array", "(\"map\", *, Bool, (false, true))"]` | 29.792 μs (5%) | 0.000 ns | 29.66 KiB (1%) | 6 |
| `["union", "array", "(\"map\", *, Bool, (true, true))"]` | 28.399 μs (5%) | 0.000 ns | 29.66 KiB (1%) | 6 |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, false))"]` | 49.715 μs (5%) | 0.000 ns | 156.38 KiB (1%) | 4 |
| `["union", "array", "(\"map\", *, Complex{Float64}, (false, true))"]` | 76.253 μs (5%) | 0.000 ns | 322.55 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Complex{Float64}, (true, true))"]` | 77.189 μs (5%) | 0.000 ns | 322.55 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Float32, (false, false))"]` | 31.693 μs (5%) | 0.000 ns | 39.19 KiB (1%) | 4 |
| `["union", "array", "(\"map\", *, Float32, (false, true))"]` | 45.555 μs (5%) | 0.000 ns | 88.17 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Float32, (true, true))"]` | 45.503 μs (5%) | 0.000 ns | 88.17 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Float64, (false, false))"]` | 32.002 μs (5%) | 0.000 ns | 78.25 KiB (1%) | 4 |
| `["union", "array", "(\"map\", *, Float64, (false, true))"]` | 48.681 μs (5%) | 0.000 ns | 166.30 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Float64, (true, true))"]` | 48.754 μs (5%) | 0.000 ns | 166.30 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Int64, (false, false))"]` | 33.436 μs (5%) | 0.000 ns | 78.25 KiB (1%) | 4 |
| `["union", "array", "(\"map\", *, Int64, (false, true))"]` | 52.018 μs (5%) | 0.000 ns | 166.30 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Int64, (true, true))"]` | 49.742 μs (5%) | 0.000 ns | 166.30 KiB (1%) | 7 |
| `["union", "array", "(\"map\", *, Int8, (false, false))"]` | 18.340 μs (5%) | 0.000 ns | 9.98 KiB (1%) | 3 |
| `["union", "array", "(\"map\", *, Int8, (false, true))"]` | 31.954 μs (5%) | 0.000 ns | 29.66 KiB (1%) | 6 |
| `["union", "array", "(\"map\", *, Int8, (true, true))"]` | 28.610 μs (5%) | 0.000 ns | 29.66 KiB (1%) | 6 |
| `["union", "array", "(\"map\", abs, BigFloat, false)"]` | 330.459 μs (5%) | 0.000 ns | 1.14 MiB (1%) | 20003 |
| `["union", "array", "(\"map\", abs, BigFloat, true)"]` | 289.053 μs (5%) | 0.000 ns | 1.11 MiB (1%) | 17839 |
| `["union", "array", "(\"map\", abs, BigInt, false)"]` | 444.037 μs (5%) | 0.000 ns | 312.03 KiB (1%) | 14967 |
| `["union", "array", "(\"map\", abs, BigInt, true)"]` | 597.246 μs (5%) | 0.000 ns | 364.03 KiB (1%) | 13292 |
| `["union", "array", "(\"map\", abs, Bool, false)"]` | 13.114 μs (5%) | 0.000 ns | 9.95 KiB (1%) | 2 |
| `["union", "array", "(\"map\", abs, Bool, true)"]` | 16.180 μs (5%) | 0.000 ns | 29.59 KiB (1%) | 4 |
| `["union", "array", "(\"map\", abs, Complex{Float64}, false)"]` | 72.346 μs (5%) | 0.000 ns | 78.22 KiB (1%) | 3 |
| `["union", "array", "(\"map\", abs, Complex{Float64}, true)"]` | 74.066 μs (5%) | 0.000 ns | 166.23 KiB (1%) | 5 |
| `["union", "array", "(\"map\", abs, Float32, false)"]` | 13.225 μs (5%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["union", "array", "(\"map\", abs, Float32, true)"]` | 19.749 μs (5%) | 0.000 ns | 88.11 KiB (1%) | 5 |
| `["union", "array", "(\"map\", abs, Float64, false)"]` | 13.481 μs (5%) | 0.000 ns | 78.22 KiB (1%) | 3 |
| `["union", "array", "(\"map\", abs, Float64, true)"]` | 26.674 μs (5%) | 0.000 ns | 166.23 KiB (1%) | 5 |
| `["union", "array", "(\"map\", abs, Int64, false)"]` | 15.959 μs (5%) | 0.000 ns | 78.22 KiB (1%) | 3 |
| `["union", "array", "(\"map\", abs, Int64, true)"]` | 25.611 μs (5%) | 0.000 ns | 166.23 KiB (1%) | 5 |
| `["union", "array", "(\"map\", abs, Int8, false)"]` | 15.680 μs (5%) | 0.000 ns | 9.95 KiB (1%) | 2 |
| `["union", "array", "(\"map\", abs, Int8, true)"]` | 18.507 μs (5%) | 0.000 ns | 29.59 KiB (1%) | 4 |
| `["union", "array", "(\"map\", identity, BigFloat, false)"]` | 34.122 μs (5%) | 0.000 ns | 78.22 KiB (1%) | 3 |
| `["union", "array", "(\"map\", identity, BigFloat, true)"]` | 43.094 μs (5%) | 0.000 ns | 156.42 KiB (1%) | 5 |
| `["union", "array", "(\"map\", identity, BigInt, false)"]` | 44.716 μs (5%) | 0.000 ns | 78.22 KiB (1%) | 3 |
| `["union", "array", "(\"map\", identity, BigInt, true)"]` | 50.433 μs (5%) | 0.000 ns | 156.42 KiB (1%) | 5 |
| `["union", "array", "(\"map\", identity, Bool, false)"]` | 13.118 μs (5%) | 0.000 ns | 9.95 KiB (1%) | 2 |
| `["union", "array", "(\"map\", identity, Bool, true)"]` | 16.392 μs (5%) | 0.000 ns | 29.59 KiB (1%) | 4 |
| `["union", "array", "(\"map\", identity, Complex{Float64}, false)"]` | 17.635 μs (5%) | 0.000 ns | 156.34 KiB (1%) | 3 |
| `["union", "array", "(\"map\", identity, Complex{Float64}, true)"]` | 45.301 μs (5%) | 0.000 ns | 322.48 KiB (1%) | 5 |
| `["union", "array", "(\"map\", identity, Float32, false)"]` | 13.224 μs (5%) | 0.000 ns | 39.16 KiB (1%) | 3 |
| `["union", "array", "(\"map\", identity, Float32, true)"]` | 19.670 μs (5%) | 0.000 ns | 88.11 KiB (1%) | 5 |
| `["union", "array", "(\"map\", identity, Float64, false)"]` | 13.370 μs (5%) | 0.000 ns | 78.22 KiB (1%) | 3 |
| `["union", "array", "(\"map\", identity, Float64, true)"]` | 21.966 μs (5%) | 0.000 ns | 166.23 KiB (1%) | 5 |
| `["union", "array", "(\"map\", identity, Int64, false)"]` | 13.419 μs (5%) | 0.000 ns | 78.22 KiB (1%) | 3 |
| `["union", "array", "(\"map\", identity, Int64, true)"]` | 21.537 μs (5%) | 0.000 ns | 166.23 KiB (1%) | 5 |
| `["union", "array", "(\"map\", identity, Int8, false)"]` | 13.116 μs (5%) | 0.000 ns | 9.95 KiB (1%) | 2 |
| `["union", "array", "(\"map\", identity, Int8, true)"]` | 16.501 μs (5%) | 0.000 ns | 29.59 KiB (1%) | 4 |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, false))"]` | 721.040 μs (5%) | 0.000 ns | 1.14 MiB (1%) | 20008 |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (false, true))"]` | 666.495 μs (5%) | 0.000 ns | 1.03 MiB (1%) | 17842 |
| `["union", "array", "(\"perf_binaryop\", *, BigFloat, (true, true))"]` | 654.588 μs (5%) | 0.000 ns | 1.03 MiB (1%) | 17842 |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, false))"]` | 1.078 ms (5%) | 0.000 ns | 703.32 KiB (1%) | 30008 |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (false, true))"]` | 969.336 μs (5%) | 0.000 ns | 635.63 KiB (1%) | 26759 |
| `["union", "array", "(\"perf_binaryop\", *, BigInt, (true, true))"]` | 975.618 μs (5%) | 0.000 ns | 635.63 KiB (1%) | 26759 |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, false))"]` | 22.312 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (false, true))"]` | 27.890 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Bool, (true, true))"]` | 26.955 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, false))"]` | 51.380 μs (5%) | 0.000 ns | 166.14 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (false, true))"]` | 57.714 μs (5%) | 0.000 ns | 166.14 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Complex{Float64}, (true, true))"]` | 57.913 μs (5%) | 0.000 ns | 166.14 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, false))"]` | 24.922 μs (5%) | 0.000 ns | 48.95 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (false, true))"]` | 30.529 μs (5%) | 0.000 ns | 48.95 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Float32, (true, true))"]` | 30.353 μs (5%) | 0.000 ns | 48.95 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, false))"]` | 28.107 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (false, true))"]` | 34.338 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Float64, (true, true))"]` | 33.291 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, false))"]` | 28.469 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (false, true))"]` | 34.399 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Int64, (true, true))"]` | 33.576 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, false))"]` | 22.316 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (false, true))"]` | 28.439 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_binaryop\", *, Int8, (true, true))"]` | 27.571 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_countequals\", \"BigFloat\")"]` | 183.283 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countequals\", \"BigInt\")"]` | 100.639 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countequals\", \"Bool\")"]` | 24.252 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countequals\", \"Complex{Float64}\")"]` | 36.205 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countequals\", \"Float32\")"]` | 20.334 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countequals\", \"Float64\")"]` | 19.612 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countequals\", \"Int64\")"]` | 26.016 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countequals\", \"Int8\")"]` | 24.052 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 5.848 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 5.850 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", BigInt, false)"]` | 5.843 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", BigInt, true)"]` | 5.845 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Bool, false)"]` | 2.160 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Bool, true)"]` | 2.160 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, false)"]` | 2.162 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Complex{Float64}, true)"]` | 2.165 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Float32, false)"]` | 2.166 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Float32, true)"]` | 2.164 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Float64, false)"]` | 2.166 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Float64, true)"]` | 2.169 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Int64, false)"]` | 2.162 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Int64, true)"]` | 2.168 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Int8, false)"]` | 2.165 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_countnothing\", Int8, true)"]` | 2.160 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, false)"]` | 26.743 μs (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", BigFloat, true)"]` | 31.286 μs (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", BigInt, false)"]` | 31.621 μs (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", BigInt, true)"]` | 35.962 μs (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Bool, false)"]` | 8.201 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Bool, true)"]` | 11.724 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, false)"]` | 31.844 μs (5%) | 0.000 ns | 166.14 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Complex{Float64}, true)"]` | 32.294 μs (5%) | 0.000 ns | 166.14 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Float32, false)"]` | 11.965 μs (5%) | 0.000 ns | 48.95 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Float32, true)"]` | 13.917 μs (5%) | 0.000 ns | 48.95 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Float64, false)"]` | 17.554 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Float64, true)"]` | 19.624 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Int64, false)"]` | 17.718 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Int64, true)"]` | 19.927 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Int8, false)"]` | 8.150 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_simplecopy\", Int8, true)"]` | 11.434 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"perf_sum2\", BigFloat, false)"]` | 461.117 μs (5%) | 0.000 ns | 1.07 MiB (1%) | 20006 |
| `["union", "array", "(\"perf_sum2\", BigFloat, true)"]` | 407.268 μs (5%) | 0.000 ns | 975.63 KiB (1%) | 17840 |
| `["union", "array", "(\"perf_sum2\", BigInt, false)"]` | 1.136 ms (5%) | 0.000 ns | 616.76 KiB (1%) | 30006 |
| `["union", "array", "(\"perf_sum2\", BigInt, true)"]` | 1.071 ms (5%) | 0.000 ns | 546.33 KiB (1%) | 26757 |
| `["union", "array", "(\"perf_sum2\", Bool, false)"]` | 5.214 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Bool, true)"]` | 12.271 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, false)"]` | 7.713 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Complex{Float64}, true)"]` | 9.592 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Float32, false)"]` | 7.710 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Float32, true)"]` | 11.477 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Float64, false)"]` | 7.708 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Float64, true)"]` | 10.728 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Int64, false)"]` | 3.560 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Int64, true)"]` | 3.561 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Int8, false)"]` | 4.071 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum2\", Int8, true)"]` | 9.563 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", BigFloat, false)"]` | 458.545 μs (5%) | 0.000 ns | 1.07 MiB (1%) | 20006 |
| `["union", "array", "(\"perf_sum3\", BigFloat, true)"]` | 406.252 μs (5%) | 0.000 ns | 975.63 KiB (1%) | 17840 |
| `["union", "array", "(\"perf_sum3\", BigInt, false)"]` | 1.139 ms (5%) | 0.000 ns | 616.76 KiB (1%) | 30006 |
| `["union", "array", "(\"perf_sum3\", BigInt, true)"]` | 1.076 ms (5%) | 0.000 ns | 546.33 KiB (1%) | 26757 |
| `["union", "array", "(\"perf_sum3\", Bool, false)"]` | 7.768 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Bool, true)"]` | 10.970 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, false)"]` | 11.578 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Complex{Float64}, true)"]` | 14.090 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Float32, false)"]` | 7.720 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Float32, true)"]` | 10.906 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Float64, false)"]` | 7.718 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Float64, true)"]` | 10.865 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Int64, false)"]` | 7.733 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Int64, true)"]` | 10.431 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Int8, false)"]` | 5.162 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum3\", Int8, true)"]` | 8.744 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", BigFloat, false)"]` | 669.765 μs (5%) | 0.000 ns | 2.14 MiB (1%) | 40006 |
| `["union", "array", "(\"perf_sum4\", BigFloat, true)"]` | 649.211 μs (5%) | 0.000 ns | 2.14 MiB (1%) | 40006 |
| `["union", "array", "(\"perf_sum4\", BigInt, false)"]` | 3.075 ms (5%) | 0.000 ns | 1007.38 KiB (1%) | 50006 |
| `["union", "array", "(\"perf_sum4\", BigInt, true)"]` | 3.058 ms (5%) | 0.000 ns | 1003.42 KiB (1%) | 50006 |
| `["union", "array", "(\"perf_sum4\", Bool, false)"]` | 3.707 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Bool, true)"]` | 3.706 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, false)"]` | 7.740 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Complex{Float64}, true)"]` | 11.806 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Float32, false)"]` | 1.654 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Float32, true)"]` | 1.653 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Float64, false)"]` | 1.981 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Float64, true)"]` | 1.975 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Int64, false)"]` | 1.762 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Int64, true)"]` | 1.760 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Int8, false)"]` | 212.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum4\", Int8, true)"]` | 211.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", BigFloat, false)"]` | 443.671 μs (5%) | 0.000 ns | 1.07 MiB (1%) | 20006 |
| `["union", "array", "(\"perf_sum\", BigFloat, true)"]` | 395.800 μs (5%) | 0.000 ns | 975.63 KiB (1%) | 17840 |
| `["union", "array", "(\"perf_sum\", BigInt, false)"]` | 1.113 ms (5%) | 0.000 ns | 616.76 KiB (1%) | 30006 |
| `["union", "array", "(\"perf_sum\", BigInt, true)"]` | 1.038 ms (5%) | 0.000 ns | 546.33 KiB (1%) | 26757 |
| `["union", "array", "(\"perf_sum\", Bool, false)"]` | 5.220 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Bool, true)"]` | 9.918 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, false)"]` | 7.712 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 11.002 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Float32, false)"]` | 7.710 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Float32, true)"]` | 11.467 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Float64, false)"]` | 7.708 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Float64, true)"]` | 9.405 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Int64, false)"]` | 1.763 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Int64, true)"]` | 1.759 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Int8, false)"]` | 215.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"perf_sum\", Int8, true)"]` | 209.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"skipmissing\", collect, BigFloat, false)"]` | 76.205 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, BigFloat, true)"]` | 84.430 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, BigInt, false)"]` | 72.746 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, BigInt, true)"]` | 83.698 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Bool, false)"]` | 48.107 μs (5%) | 0.000 ns | 32.88 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Bool, true)"]` | 62.166 μs (5%) | 0.000 ns | 32.88 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, false)"]` | 74.213 μs (5%) | 0.000 ns | 512.73 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, true)"]` | 86.717 μs (5%) | 0.000 ns | 512.73 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Float32, false)"]` | 52.308 μs (5%) | 0.000 ns | 128.69 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Float32, true)"]` | 64.979 μs (5%) | 0.000 ns | 128.69 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Float64, false)"]` | 58.746 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Float64, true)"]` | 70.672 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Int64, false)"]` | 57.795 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Int64, true)"]` | 71.227 μs (5%) | 0.000 ns | 256.72 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Int8, false)"]` | 47.931 μs (5%) | 0.000 ns | 32.88 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", collect, Int8, true)"]` | 62.351 μs (5%) | 0.000 ns | 32.88 KiB (1%) | 15 |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, false)"]` | 439.851 μs (5%) | 0.000 ns | 1.07 MiB (1%) | 19998 |
| `["union", "array", "(\"skipmissing\", sum, BigFloat, true)"]` | 400.277 μs (5%) | 0.000 ns | 975.72 KiB (1%) | 17866 |
| `["union", "array", "(\"skipmissing\", sum, BigInt, false)"]` | 1.192 ms (5%) | 0.000 ns | 609.67 KiB (1%) | 29997 |
| `["union", "array", "(\"skipmissing\", sum, BigInt, true)"]` | 1.101 ms (5%) | 0.000 ns | 542.33 KiB (1%) | 26782 |
| `["union", "array", "(\"skipmissing\", sum, Bool, false)"]` | 2.318 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"skipmissing\", sum, Bool, true)"]` | 12.203 μs (5%) | 0.000 ns | 80 bytes (1%) | 5 |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, false)"]` | 7.507 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"skipmissing\", sum, Complex{Float64}, true)"]` | 9.935 μs (5%) | 0.000 ns | 112 bytes (1%) | 5 |
| `["union", "array", "(\"skipmissing\", sum, Float32, false)"]` | 793.000 ns (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"skipmissing\", sum, Float32, true)"]` | 10.784 μs (5%) | 0.000 ns | 80 bytes (1%) | 5 |
| `["union", "array", "(\"skipmissing\", sum, Float64, false)"]` | 1.252 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"skipmissing\", sum, Float64, true)"]` | 9.734 μs (5%) | 0.000 ns | 80 bytes (1%) | 5 |
| `["union", "array", "(\"skipmissing\", sum, Int64, false)"]` | 1.095 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"skipmissing\", sum, Int64, true)"]` | 2.664 μs (5%) | 0.000 ns | 80 bytes (1%) | 5 |
| `["union", "array", "(\"skipmissing\", sum, Int8, false)"]` | 1.117 μs (5%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["union", "array", "(\"skipmissing\", sum, Int8, true)"]` | 2.970 μs (5%) | 0.000 ns | 80 bytes (1%) | 5 |
| `["union", "array", "(\"sort\", BigFloat, false)"]` | 2.873 ms (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", BigFloat, true)"]` | 2.806 ms (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", BigInt, false)"]` | 1.593 ms (5%) | 0.000 ns | 78.35 KiB (1%) | 10 |
| `["union", "array", "(\"sort\", BigInt, true)"]` | 1.630 ms (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Bool, false)"]` | 44.083 μs (5%) | 0.000 ns | 10.03 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Bool, true)"]` | 379.753 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Float32, false)"]` | 369.235 μs (5%) | 0.000 ns | 39.14 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Float32, true)"]` | 870.059 μs (5%) | 0.000 ns | 48.95 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Float64, false)"]` | 372.066 μs (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Float64, true)"]` | 872.667 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Int64, false)"]` | 366.188 μs (5%) | 0.000 ns | 78.20 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Int64, true)"]` | 628.133 μs (5%) | 0.000 ns | 88.02 KiB (1%) | 2 |
| `["union", "array", "(\"sort\", Int8, false)"]` | 291.318 μs (5%) | 0.000 ns | 9.94 KiB (1%) | 1 |
| `["union", "array", "(\"sort\", Int8, true)"]` | 543.774 μs (5%) | 0.000 ns | 19.64 KiB (1%) | 2 |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "accumulate"]`
- `["array", "any/all"]`
- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "equality"]`
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
- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "optimizations"]`
- `["collection", "queries & updates"]`
- `["collection", "set operations"]`
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["find", "findall"]`
- `["find", "findnext"]`
- `["find", "findprev"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["io"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["micro"]`
- `["misc"]`
- `["misc", "23042"]`
- `["misc", "afoldl"]`
- `["misc", "bitshift"]`
- `["misc", "issue 12165"]`
- `["misc", "julia"]`
- `["misc", "parse"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
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
- `["scalar", "acosh"]`
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "asinh"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "atanh"]`
- `["scalar", "cbrt"]`
- `["scalar", "cos"]`
- `["scalar", "cosh"]`
- `["scalar", "exp2"]`
- `["scalar", "expm1"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "sinh"]`
- `["scalar", "tan"]`
- `["scalar", "tanh"]`
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
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "misc"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-DEV.210
Commit a572504 (2018-09-08 03:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   48170552 s       4998 s    5254822 s  1367675137 s         19 s
       #2  3501 MHz  223058526 s        203 s    3466975 s  1197115663 s          9 s
       #3  3501 MHz   32559934 s       3194 s    2886797 s  1388180743 s         22 s
       #4  3501 MHz   30207818 s          0 s    3537928 s  1389702189 s         10 s
       
  Memory: 31.383651733398438 GB (4207.01171875 MB free)
  Uptime: 1.424881e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
