# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@b38bfefd8321cb9c5559af7ecaeb514e458109f3](https://github.com/mbauman/julia/commit/b38bfefd8321cb9c5559af7ecaeb514e458109f3) vs [JuliaLang/julia@f8243b7d203a28c1ac4374f883fcb6d4d9667418](https://github.com/JuliaLang/julia/commit/f8243b7d203a28c1ac4374f883fcb6d4d9667418)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15558#issuecomment-346921538)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

