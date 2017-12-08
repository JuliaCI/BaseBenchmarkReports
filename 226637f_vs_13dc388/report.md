# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@226637fd0b5b64783770ee73345a152bc4455c33](https://github.com/JuliaLang/julia/commit/226637fd0b5b64783770ee73345a152bc4455c33) vs [JuliaLang/julia@13dc388b11c7c14b4e263384e16118e0e3377cbe](https://github.com/JuliaLang/julia/commit/13dc388b11c7c14b4e263384e16118e0e3377cbe)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24774#issuecomment-350386426)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

