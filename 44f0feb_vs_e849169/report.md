# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@44f0feb75adcf8264d05eefeb98edc45d86c3845](https://github.com/JuliaLang/julia/commit/44f0feb75adcf8264d05eefeb98edc45d86c3845) vs [JuliaLang/julia@e849169bcf8ef79bd7c1dbfb6200a5a218496ceb](https://github.com/JuliaLang/julia/commit/e849169bcf8ef79bd7c1dbfb6200a5a218496ceb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20485#issuecomment-278334515)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

