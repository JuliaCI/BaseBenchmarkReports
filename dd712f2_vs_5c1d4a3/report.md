# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@dd712f2a1c9b448da045a8890e3c38fd8c627f4c](https://github.com/JuliaLang/julia/commit/dd712f2a1c9b448da045a8890e3c38fd8c627f4c) vs [JuliaLang/julia@5c1d4a33b2b2850282297c69e15601bbad669073](https://github.com/JuliaLang/julia/commit/5c1d4a33b2b2850282297c69e15601bbad669073)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28857#issuecomment-419447145)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

