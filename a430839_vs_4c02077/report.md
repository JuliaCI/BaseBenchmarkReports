# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a4308398f6e958b1574ea78dbdc9367c461c55fd](https://github.com/JuliaLang/julia/commit/a4308398f6e958b1574ea78dbdc9367c461c55fd) vs [JuliaLang/julia@4c02077a3a88f7d28dfa6f8d839f3483dceda84b](https://github.com/JuliaLang/julia/commit/4c02077a3a88f7d28dfa6f8d839f3483dceda84b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28857#issuecomment-418966607)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`/home/nanosoldier/workdir/tmpUm6l0O/julia -e '
    if VERSION >= v"0.7.0-beta2.203"
        import BaseBenchmarks
        print(dirname(dirname(pathof(BaseBenchmarks))))
    else
        print(Pkg.dir("BaseBenchmarks"))
    end
'`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

