# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6a05484929b6356171f856105d527f0ad00c9af2](https://github.com/JuliaLang/julia/commit/6a05484929b6356171f856105d527f0ad00c9af2) vs [JuliaLang/julia@c67c523ec50fea8aa503dc644e006fb712d688d2](https://github.com/JuliaLang/julia/commit/c67c523ec50fea8aa503dc644e006fb712d688d2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20005#issuecomment-313879562)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

