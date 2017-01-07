# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@16c0ed5f893a848cce620a958a9c88be1d193b4d](https://github.com/JuliaLang/julia/commit/16c0ed5f893a848cce620a958a9c88be1d193b4d) vs [JuliaLang/julia@f4ed16b36bf300fd1192b7a473f9b0270cad816a](https://github.com/JuliaLang/julia/commit/f4ed16b36bf300fd1192b7a473f9b0270cad816a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-271064606)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

