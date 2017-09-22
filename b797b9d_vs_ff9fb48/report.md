# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b797b9dea1a73fd38cb2df2ffa9762a6014324fe](https://github.com/JuliaLang/julia/commit/b797b9dea1a73fd38cb2df2ffa9762a6014324fe) vs [JuliaLang/julia@ff9fb483172ad792c47b7652eff1173044f3b9ae](https://github.com/JuliaLang/julia/commit/ff9fb483172ad792c47b7652eff1173044f3b9ae)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20621#issuecomment-331321260)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

