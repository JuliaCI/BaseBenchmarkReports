# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fd54c4cb21b2a1f78ab02728979a0cdbec8d3e0f](https://github.com/JuliaLang/julia/commit/fd54c4cb21b2a1f78ab02728979a0cdbec8d3e0f) vs [JuliaLang/julia@b6e4e700f03acc0e39325f3590f52d4a6f63f699](https://github.com/JuliaLang/julia/commit/b6e4e700f03acc0e39325f3590f52d4a6f63f699)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21670#issuecomment-298740655)

*Tag Predicate:* `"array" && "bool" || "simd"`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`/home/nanosoldier/workdir/tmp430hB7/julia -e 'Pkg.add("BaseBenchmarks")'`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

