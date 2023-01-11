# Resonance_Lines
Calculate constant lines of E<sub>J</sub>.

## Derivation 

Starting from the Jacobi energy, rewrite the total energy, $E$, in terms of the circular and random energies,
```math
\begin{align}
    E_{J}(J_{r}= 0) &= E - \Omega_{b}L_{z} \\
    E_{J}(J_{r}= 0) &= (E_{c} + E_{r}) - \Omega_{b}L_{z}.
\end{align}
```

Solve for E<sub>r</sub>,

```math
    E_{r} = E_{J}(J_{r}= 0) - E_{c} + \Omega_{b}L_{z}.
```

Substitute in E<sub>r</sub> = J<sub>r</sub>&kappa; and solve for J<sub>r</sub>,

```math
\begin{align}
    J_{r}\kappa &= E_{J}(J_{r}= 0) - E_{c} + \Omega_{b}L_{z} \\
    J_{r} &= \frac{E_{J}(J_{r}= 0) - E_{c}}{\kappa} + \frac{\Omega_{b}}{\kappa}L_{z}.
\end{align}
```

This equation has the form of a linear equation. Find the y-intercept; this will align the line with the resonances. Let's set $b$ to
```math
\begin{equation}
  b = \frac{E_{J}(J_{r}=0)- E_{c}}{\kappa}.
\end{equation}
```
We can find the y-intercept in terms of the resonance radius and its corresponding circular velocities.

```math
\begin{align}
    b &= \frac{(E - \Omega_{b}L_{z}) - E_{c}}{\kappa} \\
    &= \frac{(E_{c} + E_{r} - \Omega_{b}L_{z}) - E_{c}}{\kappa} \\
    &= \frac{(J_{r}\kappa) - \Omega_{b}L_{z}}{\kappa} \\
    &= - \frac{\Omega_{b}L_{z}}{\kappa} \\
    &= - \frac{\Omega_{b}(R_{g} \cdot v_{c})}{\kappa} 
\end{align}
```

where R<sub>g</sub> is the resonance and v<sub>c</sub> is the circular velocity at R<sub>g</sub>.
