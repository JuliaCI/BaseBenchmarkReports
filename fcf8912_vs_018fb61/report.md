# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fcf891265ece881230e42052790494a7171058e7](https://github.com/JuliaLang/julia/commit/fcf891265ece881230e42052790494a7171058e7) vs [JuliaLang/julia@018fb61ff6da94a27fb93da8febbb8ddee4ecceb](https://github.com/JuliaLang/julia/commit/018fb61ff6da94a27fb93da8febbb8ddee4ecceb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/26133#issuecomment-368129394)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

