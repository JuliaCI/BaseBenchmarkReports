# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7aad26a57ddcb8cf7c3d6373ffe9fd48a8b02caf](https://github.com/JuliaLang/julia/commit/7aad26a57ddcb8cf7c3d6373ffe9fd48a8b02caf) vs [JuliaLang/julia@13b22540b7b85cc29e62f15bbad7c2b29a82afeb](https://github.com/JuliaLang/julia/commit/13b22540b7b85cc29e62f15bbad7c2b29a82afeb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-270123633)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

