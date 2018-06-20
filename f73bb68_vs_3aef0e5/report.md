# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f73bb682e56cd00b0d6da05280338b80727cf59b](https://github.com/JuliaLang/julia/commit/f73bb682e56cd00b0d6da05280338b80727cf59b) vs [JuliaLang/julia@3aef0e53858c82d5751a991a30d967b27519e13f](https://github.com/JuliaLang/julia/commit/3aef0e53858c82d5751a991a30d967b27519e13f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27691#issuecomment-398852065)

*Tag Predicate:* `"shootout" || ("string" || "problem")`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against comparison commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(139)) [139]
```

Check the logs folder in this directory for more detailed output.

