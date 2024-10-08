# Data archive for equation discovery and recovery

Archive of data used to explore differential equation discovery approaches.

## Notes
Each folder contains data and explanatory documents. The title also contains an abbreviation for the data source. Synthetic data - s_d, Real data - r_d.

---
## Examples

<details>
<summary>1. Wave equation with one spatial variable </summary>

```math 
\frac{\partial^{2} u}{\partial t^{2}} - \frac{1}{25} \frac{\partial^{2} u}{\partial x^{2}} = 0,
```

```math 
\\ 100\times100, x \in [0; 1], t \in [0; 1].
```

```math 
\\ bc = \{u(0, t) = 0, u(1, t) = 0\}, \
\\ ic = \{u(x, 0) = 10000 \sin (\frac{1}{10}\cdot x \cdot (x-1))^2\}
```

</details>

<details>
<summary>2. Burgers' equation </summary>

```math 
 \frac{\partial u}{\partial t} +  u \frac{\partial u}{\partial x} = 0,
```
```math 
 \\ 256\times256, x \in [-4000; 4000], t \in [0; 4].
```
</details>

<details>
<summary>3. Burgers' equation (reduced grid) </summary>

```math 
 \frac{\partial u}{\partial t} +  u \frac{\partial u}{\partial x} = 0,
```
```math 
 \\ 100 \times100, x \in [-1000; 0], t \in [0; 1].
```
</details>

<details>
<summary>4. Lotka-Volterra equations </summary>

```math 
 \begin{equation*}
 \begin{cases}
  \frac{\partial u}{\partial t} = \normalsize 0.55 \cdot u - 0.028 \cdot u \cdot v, 
   \\
   \frac{\partial v}{\partial t} = \normalsize - 0.84 \cdot v + 0.026 \cdot u \cdot v.
 \end{cases}
\end{equation*}
```
```math 
 \\ t \in [0, 20],
 \\ u_0, \ v_0 = 30, 4.
```
</details>

### Algorithms under research:

- EPDE (Evolutionary Partial Differential Equations). Algorithm for the search of differential equations based on data (https://github.com/ITMO-NSS-team/EPDE)
- TEDEouS (Torch Exhaustive Differential Equation Solver). Algorithm for automated solution of differential equations based on neural networks (https://github.com/ITMO-NSS-team/torch_DE_solver)

---
