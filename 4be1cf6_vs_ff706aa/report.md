# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4be1cf60cb83559280cdb23a6277ee25ebc43de0](https://github.com/JuliaLang/julia/commit/4be1cf60cb83559280cdb23a6277ee25ebc43de0) vs [JuliaLang/julia@ff706aa0dc3e7b74ffd290a247e8cc91e4fe9197](https://github.com/JuliaLang/julia/commit/ff706aa0dc3e7b74ffd290a247e8cc91e4fe9197)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23490#issuecomment-325435914)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

