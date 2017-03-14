# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@e4b45ec0773c482a2e5d86ada3d98e56814aad8e](https://github.com/pabloferz/julia/commit/e4b45ec0773c482a2e5d86ada3d98e56814aad8e) vs [JuliaLang/julia@64409a0cae8b52d3f7953a4f9571f9987c7fbdfd](https://github.com/JuliaLang/julia/commit/64409a0cae8b52d3f7953a4f9571f9987c7fbdfd)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20720#issuecomment-286527393)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

