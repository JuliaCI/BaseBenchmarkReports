# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ed6f9ec4c9f883f09adfe094b9a51a5422977edc](https://github.com/JuliaLang/julia/commit/ed6f9ec4c9f883f09adfe094b9a51a5422977edc) vs [JuliaLang/julia@46dcb35e1b92bf252aee078a90e42557b48376bc](https://github.com/JuliaLang/julia/commit/46dcb35e1b92bf252aee078a90e42557b48376bc)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26435#issuecomment-372523031)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

