# Benchmark Report

## Job Properties

*Commit(s):* [haampie/julia@b0b82b811c1047c39210a79a908d9af2eb6af83b](https://github.com/haampie/julia/commit/b0b82b811c1047c39210a79a908d9af2eb6af83b) vs [JuliaLang/julia@c8ce43ad173a9126e902dda246b74cb6e83eaded](https://github.com/JuliaLang/julia/commit/c8ce43ad173a9126e902dda246b74cb6e83eaded)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27386#issuecomment-394103577)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

