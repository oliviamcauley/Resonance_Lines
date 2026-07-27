*If you use this code, please link this repository (https://github.com/oliviamcauley/Resonance_Lines) along with http://github.com/jobovy/galpy in any publication.*

# Resonance Lines
Calculate constant lines of the Jacobi energy, E<sub>J</sub>.

## Derivation 

Starting from the Jacobi energy, rewrite the total energy, $E$, in terms of the circular ($E_{c}$) and radial ($E_{r}$) energies,
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

This equation has the form of a linear equation, $y=y_{0}+mx$. To align the line(s) with the resonances, find the y-intercept, $y_{0}$. 

Setting $y_{0}$ to,
```math
\begin{equation}
  y_{0} = \frac{E_{J}(J_{r}=0)- E_{c}}{\kappa},
\end{equation}
```
we can find the y-intercept in terms of the resonance radius and its corresponding circular velocities,

```math
\begin{align}
    y_{0} &= \frac{(E - \Omega_{b}L_{z}) - E_{c}}{\kappa} \\
    &= \frac{(E_{c} + E_{r} - \Omega_{b}L_{z}) - E_{c}}{\kappa} \\
    &= \frac{(J_{r}\kappa) - \Omega_{b}L_{z}}{\kappa}.
\end{align}
```
Remember that J<sub>r</sub> = 0,

```math
\begin{align}
    y_{0} &= - \frac{\Omega_{b}L_{z}}{\kappa} \\
    &= - \frac{\Omega_{b}(R_{g} \cdot v_{c})}{\kappa}, 
\end{align}
```

where R<sub>g</sub> is the guiding radius at the resonance and v<sub>c</sub> is the circular velocity at R<sub>g</sub>.

# Plot the Lines of Resonances for a Growing Dehnen Bar
<table>
  <tr>
    <td width="50%">
      <img width="1024" height="554" src="https://github.com/user-attachments/assets/db053274-b43e-42d0-8b09-c56b9406d183" alt="GrowBar_JphiAction">
    </td>
    <td width="50%" valign="top">
      <h3>Azimuthal Action in Barred Disk Galaxy</h3>
      <p>This plot describes the change in azimuthal action in action space after two rotations of the bar. The legend of the plot is read as follows:

The y-axis is the initial radial action.<br>
The x-axis is the initial azimuthal action.<br>

The dashed lines are the ultra harmonic resonances (UHR).<br>
The solid black line is the corotation resonance (CR).

The color bar is the change in the orbit sizes after two rotations of the bar. <br>
Red means that the stellar orbit is increasing in size. Blue means that the orbit is decreasing in size. <br>
***Take Away: The greatest changes in orbital sizes occur near corotation.*** </p>
    </td>
  </tr>
</table>

