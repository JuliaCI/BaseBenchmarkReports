# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ee4d27c0bbe9180656d8d8372f2e3d7a1badd0a6](https://github.com/JuliaLang/julia/commit/ee4d27c0bbe9180656d8d8372f2e3d7a1badd0a6) vs [JuliaLang/julia@018fb61ff6da94a27fb93da8febbb8ddee4ecceb](https://github.com/JuliaLang/julia/commit/018fb61ff6da94a27fb93da8febbb8ddee4ecceb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25890#issuecomment-368120627)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

