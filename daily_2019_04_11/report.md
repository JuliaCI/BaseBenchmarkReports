# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@62d7ec55fd8063c722bc79b72c6d20b34a887c39](https://github.com/JuliaLang/julia/commit/62d7ec55fd8063c722bc79b72c6d20b34a887c39)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/62d7ec55fd8063c722bc79b72c6d20b34a887c39#commitcomment-33133362)

*Tag Predicate:* `ALL`

*Daily Job:* 2019-04-11

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`/home/nanosoldier/workdir/tmprhIleE/julia -e '
    if VERSION >= v"0.7.0-beta2.203"
        import BaseBenchmarks
        print(dirname(dirname(pathof(BaseBenchmarks))))
    else
        print(Pkg.dir("BaseBenchmarks"))
    end
'`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

