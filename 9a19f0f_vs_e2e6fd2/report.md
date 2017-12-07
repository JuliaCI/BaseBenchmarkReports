# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@9a19f0f21ea618a3365500c9e343bdb34a72d6a9](https://github.com/JuliaLang/julia/commit/9a19f0f21ea618a3365500c9e343bdb34a72d6a9) vs [JuliaLang/julia@e2e6fd2f424ff7903a56bcabc3484acca83ddf49](https://github.com/JuliaLang/julia/commit/e2e6fd2f424ff7903a56bcabc3484acca83ddf49)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24774#issuecomment-350055180)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

