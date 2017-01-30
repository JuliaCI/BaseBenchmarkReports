# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a45b4f9847b4618bd4c9db7370058d7cd40276d9](https://github.com/JuliaLang/julia/commit/a45b4f9847b4618bd4c9db7370058d7cd40276d9) vs [JuliaLang/julia@65afe479cfd5afd6c782aafc2a18dac5a55cb4de](https://github.com/JuliaLang/julia/commit/65afe479cfd5afd6c782aafc2a18dac5a55cb4de)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19890#issuecomment-275980514)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

