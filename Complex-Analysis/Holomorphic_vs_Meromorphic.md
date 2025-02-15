# Holomorphic and Meromorphic Functions in Complex Analysis

## Holomorphic Functions
A function `f(z)` is **holomorphic** if it is complex differentiable at every point in an open subset `U ⊆ ℂ`. If `f(z)` is holomorphic throughout `U`, then:

- `f(z)` satisfies the **Cauchy-Riemann equations** in `U`:
  - `∂u/∂x = ∂v/∂y, ∂u/∂y = -∂v/∂x`,
    where `f(z) = u(x, y) + i v(x, y)` with `z = x + i y`.
- `f(z)` is infinitely differentiable and analytic, meaning it can be represented as a power series in `z` in `U`:
  - `f(z) = Σ (a_n (z - z₀)ⁿ)`.

### Examples:
1. `f(z) = z², e^z, sin(z)` are holomorphic functions on `ℂ`.
2. `f(z) = 1/z` is holomorphic on `ℂ \ {0}`.

---

## Meromorphic Functions
A function `f(z)` is **meromorphic** on a domain `U` if:
- `f(z)` is holomorphic on `U`, except at a discrete set of points called **poles**.
- At each pole `z₀`, `f(z)` can be written as:
  - `f(z) = g(z) / (z - z₀)ⁿ`,
    where `g(z)` is holomorphic and `g(z₀) ≠ 0`.

### Key Features:
1. **Poles**: A pole is a type of singularity where `f(z) → ∞` as `z → z₀`.
2. **Isolated Singularities**: Poles are isolated, meaning there exists a neighborhood around `z₀` where `f(z)` is holomorphic except at `z₀`.

### Examples:
1. `f(z) = 1/z` is meromorphic on `ℂ` with a pole at `z = 0`.
2. `f(z) = tan(z) = sin(z) / cos(z)` is meromorphic on `ℂ \ {z = π/2 + nπ, n ∈ ℤ}` due to poles where `cos(z) = 0`.

---

## Comparison of Holomorphic and Meromorphic Functions

| Property             | Holomorphic Functions                | Meromorphic Functions                   |
|----------------------|---------------------------------------|-----------------------------------------|
| Definition           | Differentiable everywhere in `U`     | Differentiable except at poles          |
| Singularity          | None                                 | Poles (isolated singularities)          |
| Examples             | `e^z, sin(z), z²`                    | `1/z, tan(z)`                           |
| Analyticity          | Always analytic                      | Analytic except at poles                |
