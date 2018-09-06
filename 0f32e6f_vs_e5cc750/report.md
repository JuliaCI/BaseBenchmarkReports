# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0f32e6fd95c13ca2dd268a4241e8958a3f7188b1](https://github.com/JuliaLang/julia/commit/0f32e6fd95c13ca2dd268a4241e8958a3f7188b1) vs [JuliaLang/julia@e5cc7506d335089469f7be026ef954e684274e7f](https://github.com/JuliaLang/julia/commit/e5cc7506d335089469f7be026ef954e684274e7f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28857#issuecomment-419154482)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

