# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b8e4cc6eaa383596b4346ede02eda8106ee3f757](https://github.com/JuliaLang/julia/commit/b8e4cc6eaa383596b4346ede02eda8106ee3f757) vs [JuliaLang/julia@63c269e8fa04cafb8e38a122df979333cd1c2995](https://github.com/JuliaLang/julia/commit/63c269e8fa04cafb8e38a122df979333cd1c2995)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21670#issuecomment-298671257)

*Tag Predicate:* `"array" && "bool" || "simd"`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

