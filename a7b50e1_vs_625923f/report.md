# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a7b50e173ac9000f3f04748caf8074c906716c9b](https://github.com/JuliaLang/julia/commit/a7b50e173ac9000f3f04748caf8074c906716c9b) vs [JuliaLang/julia@625923f99374093d708b31e34bdacd6375bc9be7](https://github.com/JuliaLang/julia/commit/625923f99374093d708b31e34bdacd6375bc9be7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25630#issuecomment-359076153)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

