# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@8f965d9809b32936806ac893cab2f4a66a59d096](https://github.com/JuliaLang/julia/commit/8f965d9809b32936806ac893cab2f4a66a59d096) vs [JuliaLang/julia@8d752a07f44fd81b7a2a273d27124352186cfa8c](https://github.com/JuliaLang/julia/commit/8d752a07f44fd81b7a2a273d27124352186cfa8c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22974#issuecomment-318798363)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

