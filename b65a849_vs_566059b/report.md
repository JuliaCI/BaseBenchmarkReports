# Benchmark Report

## Job Properties

*Commit(s):* [abraunst/julia@b65a849ee22e37e304d946a2f042ab5c2da2caa6](https://github.com/abraunst/julia/commit/b65a849ee22e37e304d946a2f042ab5c2da2caa6) vs [JuliaLang/julia@566059bf389d9d0ab886b4cbdfce5f046a040f5a](https://github.com/JuliaLang/julia/commit/566059bf389d9d0ab886b4cbdfce5f046a040f5a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30676#issuecomment-459320551)

*Tag Predicate:* `"array"`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

