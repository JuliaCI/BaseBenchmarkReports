# Benchmark Report

## Job Properties

*Commit(s):* [tkoolen/julia@e46825a0b17505588b5e4263ef6590778556b783](https://github.com/tkoolen/julia/commit/e46825a0b17505588b5e4263ef6590778556b783) vs [JuliaLang/julia@0658a119725d7347513b4cc7e1111d961cd7eb51](https://github.com/JuliaLang/julia/commit/0658a119725d7347513b4cc7e1111d961cd7eb51)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27302#issuecomment-396997989)

*Tag Predicate:* `"array" || ("collection" || ("dates" || ("find" || "random")))`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against comparison commit: failed process: Process(`make -j3`, ProcessExited(2)) [2]
```

Check the logs folder in this directory for more detailed output.

