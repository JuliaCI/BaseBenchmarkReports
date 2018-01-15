# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e16aedde6c6515434c25968958e24fdbddea2337](https://github.com/JuliaLang/julia/commit/e16aedde6c6515434c25968958e24fdbddea2337) vs [JuliaLang/julia@5e2ff127f861ead7b08ce782b830069d77c97f2f](https://github.com/JuliaLang/julia/commit/5e2ff127f861ead7b08ce782b830069d77c97f2f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25496#issuecomment-357776987)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

