# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@04b22eb0c5233add842f424bb1a86371abc34ab0](https://github.com/JuliaLang/julia/commit/04b22eb0c5233add842f424bb1a86371abc34ab0) vs [JuliaLang/julia@6ad62c4d2e902fc017b67e10bcf7722b6d37687f](https://github.com/JuliaLang/julia/commit/6ad62c4d2e902fc017b67e10bcf7722b6d37687f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19730#issuecomment-269775294)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(139)) [139]")
```

Check the logs folder in this directory for more detailed output.

