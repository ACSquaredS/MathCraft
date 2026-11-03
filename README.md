# MathCraft

**MathCraft** is an open-source, numerical computing environment inspired by MathLab. This repository is the entry point for the whole project: the module map, the roadmap and the shared documentation.

> **Status:** Early stage. Module repositories are created; implementation has not started.

## Modules

| Repository | Layer | Purpose | Depends on |
|---|---|---|---|
| [MathCore](https://github.com/ACSquaredS/MathCore) | Foundation | Shared types, arrays and matrices, runtime primitives | — |
| [MathNumerical](https://github.com/ACSquaredS/MathNumerical) | Algorithms | Linear algebra, solvers, interpolation, ODE integrators | MathCore |
| [MathSymbolic](https://github.com/ACSquaredS/MathSymbolic) | Algorithms | Symbolic expressions, simplification, calculus, equation solving | MathCore |
| [MathStatistics](https://github.com/ACSquaredS/MathStatistics) | Analysis | Descriptive statistics, distributions, tests, regression | MathCore, MathNumerical |
| [MathVisualization](https://github.com/ACSquaredS/MathVisualization) | Output | 2D and 3D plots, figures, image export | MathCore |
| [MathSimulation](https://github.com/ACSquaredS/MathSimulation) | Application | Dynamic system simulation | MathCore, MathNumerical |

Dependencies flow downward: a module depends only on the layers above it in this table, never on a module that depends on it.

## Planned additions

These repositories are proposed and do not exist yet:

- **MathLanguage**: parser and interpreter for the MathCraft scripting language. This is the piece that makes MathCraft usable as a language.
- **MathIO**: reading and writing data files (CSV, JSON, binary formats).
- **MathApp**: command-line REPL and, later, a graphical interface.

## Contributing

1. Open an issue describing the change before starting large work.
2. Fork the module repository, create a branch, and open a pull request.
3. Keep each pull request focused on one module.

## License

Released under the [MIT License](LICENSE).
