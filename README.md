# SAM Optimizer (Saddle-point Avoidance Mechanism)

An optimization algorithm that detects and escapes saddle points during gradient descent, improving convergence stability in non-convex loss landscapes.

## Overview

Gradient descent can slow down or stall near saddle points, where the gradient is close to zero but the point is not a true minimum. SAM (Saddle-point Avoidance Mechanism) is designed to detect when training is stuck near such a point and move away from it, so the optimizer keeps making progress and is less likely to converge prematurely.

## Benchmarking

SAM is benchmarked against two widely used optimizers:

- **Adam**
- **Adagrad**

The comparison focuses on convergence behaviour and resistance to premature convergence on non-convex loss surfaces.

## Project Structure

```
SAM_optimizer/
├── SAM_bench.py   # Benchmark script comparing SAM with Adam and Adagrad
├── LICENSE        # MIT license
└── README.md
```

## Getting Started

1. Clone the repository
   ```
   git clone https://github.com/M-Sufiyan-Mithawala/SAM_optimizer.git
   cd SAM_optimizer
   ```
2. Install Python 3.8 or newer, then install the libraries the benchmark imports (for example `pip install numpy matplotlib`).
3. Run the benchmark
   ```
   python SAM_bench.py
   ```

## Team

| Name | GitHub |
|------|--------|
| M Sufiyan Mithawala | [M-Sufiyan-Mithawala](https://github.com/M-Sufiyan-Mithawala) |
| winnermarvi | [winnermarvi](https://github.com/winnermarvi) |

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
