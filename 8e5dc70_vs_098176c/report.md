# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8e5dc70bba5ae938130903744030a7fa8952e476](https://github.com/JuliaLang/julia/commit/8e5dc70bba5ae938130903744030a7fa8952e476) vs [JuliaLang/julia@098176c959a80ccbada168b63decd481045c4c60](https://github.com/JuliaLang/julia/commit/098176c959a80ccbada168b63decd481045c4c60)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24406#issuecomment-341511012)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

