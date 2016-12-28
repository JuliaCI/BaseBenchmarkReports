# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7a24cea31e3eee1e297e10e6156adac26241675e](https://github.com/JuliaLang/julia/commit/7a24cea31e3eee1e297e10e6156adac26241675e) vs [JuliaLang/julia@309657f69c1a54fedfda5764b5b106286389383c](https://github.com/JuliaLang/julia/commit/309657f69c1a54fedfda5764b5b106286389383c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-269540439)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

