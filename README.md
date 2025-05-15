# Statistical Emulation of Complex Cardiac Models using Gaussian Processes

This code was developed as part of my master's thesis in Biomedical Engineering at Universidade NOVA de Lisboa. The full thesis titled *"Statistical Emulation of Complex Cardiac Models using Gaussian Processes"* is available at the [UNL Digital Repository](https://run.unl.pt/handle/10362/1042). This repository contains the complete implementation supporting all conclusions in the thesis, therefore reviewing both the code and document for full context is recommended.

## Theoretical Context

### Clinical Motivation
Cardiovascular diseases remain the leading global cause of mortality, accounting for ≈18 million deaths annually (WHO 2020). Current challenges in cardiac care include:

1. **Time-sensitive decisions**: Critical interventions often require parameter estimation within ≤15 minutes
2. **Model complexity**: High-fidelity cardiac models typically require >2<sup>11</sup> CPU hours per simulation
3. **Inter-patient variability**: Standard models fail to capture 27-42% of pathological hemodynamics (European Heart Journal, 2021)

### Technical Approach
This work addresses these challenges through the development of a twin cardiac model capable of replicating the functioning of the heart when submitted to abnormal conditions (sudden raise in ventricular pressure, disrupted heart beats, etc). With an individualized model it is possible to simulate some of this changes in the digital twin heart and understand the response of the heart in case it is submitted to that same change in a real case situation.
