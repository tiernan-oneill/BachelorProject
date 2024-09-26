# BachelorProject
Mathematica code for the investigation of gravitational waveforms produced by an extreme mass ratio inspiral (EMRI) black hole system.
- We apply a first order self-force adiabatic approximation in order to study the orbital parameters via the black hole equations of motion.
- The Euler-Lagrange equations of motion for an EMRI are applied to a geodesic where the central BH is non-spinning (Schwarzschild), and the more complex case where the central BH is spinning (Kerr).
- The Chandrasekhar method is used in obtaining the energy and angular momentum of the orbit for the Kerr case.

We compute the fluxes of gravitational-wave energy for a point mass on a circular orbit in both these space-times.
- The Black Hole Perturbation Tooklit (https://bhptoolkit.org) is used here.
- The packages in the Toolkit are applied to compute the fluxes in the frequency domain using the Teukolsky formalism. The metric perturbation amplitudes are found from the amplitudes of the scalar curvature.
- We interpolate a list of flux values, consisting of the sum of the infinity and horizon fluxes. The gravitational flux at the horizon and infinity are the fluxes of the GWs emitted by the system at the horizon of the central BH and those received by an observer very far away.
- These fluxes are summed over a wide range of l and m modes (note that the mode sum is an exponentially converging one, so we stop a sufficiently large l).

Once this has been completed we obtain the inspiral solution by solving a set of three ODEs for Ω(t), r0(t) and ϕ0(t). These are the orbital angular frequency, radius, and phase respectively. 
- To construct the waveform, we multiply the amplitude by the phase.
- The waveforms are plotted and compared to one another, so that we may determine how the initial parameters of the system may affect the
nature of the obtained waveforms.
- We produce and compare the waveforms for five inspiral configurations (including retro- and pro-grade orbits).
