# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c6467fc76a3587adabc17bf780cf40f46a96ecd3](https://github.com/JuliaLang/julia/commit/c6467fc76a3587adabc17bf780cf40f46a96ecd3) vs [JuliaLang/julia@22590d529dceed93ae1dd8f32d569edba3be9f50](https://github.com/JuliaLang/julia/commit/22590d529dceed93ae1dd8f32d569edba3be9f50)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27337#issuecomment-393667820)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

