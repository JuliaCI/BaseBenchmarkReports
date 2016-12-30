# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e336472a5bf6733e06f67174b59d0d4e1c607ae6](https://github.com/JuliaLang/julia/commit/e336472a5bf6733e06f67174b59d0d4e1c607ae6) vs [JuliaLang/julia@6ad62c4d2e902fc017b67e10bcf7722b6d37687f](https://github.com/JuliaLang/julia/commit/6ad62c4d2e902fc017b67e10bcf7722b6d37687f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269775164)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

