# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a0317aedebe82cc70cbf45c1dea53beb7b6a76c3](https://github.com/JuliaLang/julia/commit/a0317aedebe82cc70cbf45c1dea53beb7b6a76c3) vs [JuliaLang/julia@b7634bec45dc6ca7b4317fc862cf632c0bcea27f](https://github.com/JuliaLang/julia/commit/b7634bec45dc6ca7b4317fc862cf632c0bcea27f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17057#issuecomment-256242132)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

