# Jets

### The primary objective of the provided code is to determine the de-fouling area of a membrane subjected to particle-laden flow. The model calculates the distance x at which the force due to fouling particles equals the force exerted by the permeate flux. This distance is a function of various parameters including particle diameter (d_p), membrane pore diameter (d_m), and other fluid dynamics properties such as the density (ρ) and viscosity (μ) of the feed, the impinging angle (φ), and the initial jet velocity (U_0).

### To find x, the find_x function employs a root-finding algorithm (root_scalar) that solves for x where the fouling force (F_D) balances the permeate flux force (F_j). The integration of x over the angle θ from 0 to 2π yields the de-fouling area. The sector area for each θ is calculated and summed to determine the total de-fouling area.

### The provided code includes detailed functions for calculating relevant parameters such as the Reynolds number (Re_D), wall shear stress (τ_wall), and other intermediary values essential for the root-finding process. Additionally, the script visualizes the de-fouling area by plotting x values as a function of θ, illustrating the de-fouling region. It also calculates and displays the major and minor axes of the area, providing a comprehensive analysis of the de-fouling pattern.
