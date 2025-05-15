# Statistical Emulation of Complex Cardiac Models using Gaussian Processes

This code was developed as part of my master's thesis in Biomedical Engineering at Universidade NOVA de Lisboa. The full thesis titled *"Statistical Emulation of Complex Cardiac Models using Gaussian Processes"* is available at the [UNL Digital Repository](https://run.unl.pt/handle/10362/1042). This repository contains the complete implementation supporting all conclusions in the thesis, therefore reviewing both the code and document for full context is recommended.

## Theoretical Context

### Clinical Motivation
Cardiovascular diseases remain the leading global cause of mortality, accounting for ≈18 million deaths annually (WHO 2020). Current challenges in cardiac care include:

1. **Time-sensitive decisions**: Critical interventions often require parameter estimation within ≤15 minutes
2. **Model complexity**: High-fidelity cardiac models typically require >2<sup>11</sup> CPU hours per simulation
3. **Inter-patient variability**: Standard models fail to capture 27-42% of pathological hemodynamics (European Heart Journal, 2021)

### Technical Approach
This work addresses these challenges through:

```math
\begin{aligned}
&\text{Gaussian Process Emulator:} & f(q) &\sim \mathcal{GP}(m(q), k(q,q')) \\
&\text{where } q &= [q_1,q_2,q_3,q_4]^T \text{ (biomechanical parameters)} \\
&\text{and } f(q) &= [\alpha_0,\beta_0,\alpha_1,\beta_1,\alpha_2,\beta_2]^T \text{ (clinical observables)}
\end{aligned}
