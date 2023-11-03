## GCC Optimization Levels

| Flag     | Description |
|----------|-------------|
| `-O0`    | No optimization. Prioritizes compilation speed and debuggability over execution speed. Default if no `-O` option is specified. |
| `-O1`    | Provides a balance between compilation time and execution speed. Applies a set of optimizations that don't take a lot of time to perform and don't greatly increase the size of the generated code. |
| `-O2`    | Applies further optimizations in addition to those applied by `-O1`. Prioritizes execution speed over compilation time, without incurring the larger binary sizes of `-O3`. |
| `-O3`    | Highest standard optimization level. Applies all the optimizations of `-O2` and additional aggressive optimizations that may increase the size of the generated code. |
| `-Os`    | Similar to `-O2`, but prioritizes code size over execution speed. Useful for systems with limited memory, like embedded systems. |
| `-Ofast` | Applies all the optimizations of `-O3` and also enables optimizations that break strict compliance with language standards. |
| `-Og`    | Provides a good level of optimization while still keeping the code debuggable. Middle ground between `-O0` and `-O1`. |

Note: The exact set of optimizations applied at each level can vary between compiler versions and different compilers. Always test thoroughly when changing optimization levels.
