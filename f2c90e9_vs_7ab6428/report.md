# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f2c90e9663718b02a4698a76c9ae854ca7652b42](https://github.com/JuliaLang/julia/commit/f2c90e9663718b02a4698a76c9ae854ca7652b42) vs [JuliaLang/julia@7ab6428050466fa20cde4e06869d9a926919ff2c](https://github.com/JuliaLang/julia/commit/7ab6428050466fa20cde4e06869d9a926919ff2c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16378#issuecomment-280424078)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

