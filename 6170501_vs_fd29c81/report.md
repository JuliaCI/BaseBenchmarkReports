# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6170501932061e332075009c6bccc87e0ae1fb97](https://github.com/JuliaLang/julia/commit/6170501932061e332075009c6bccc87e0ae1fb97) vs [JuliaLang/julia@fd29c81f961b2090f8f3f71d4ca9fb309f95f218](https://github.com/JuliaLang/julia/commit/fd29c81f961b2090f8f3f71d4ca9fb309f95f218)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27221#issuecomment-392871687)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

