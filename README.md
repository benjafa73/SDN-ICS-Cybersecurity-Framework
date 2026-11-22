# SDN-Based Cybersecurity Framework for Industrial Control Systems

## Research Project

**Title:** Development of a Software Defined Network Based Cybersecurity Framework for Industrial Control Systems

**Authors:** Mupatiwa Zulu and Lukumba Phiri

**Institution:** University of Zambia, School of Engineering

## 1. Overview

This repository contains the MATLAB simulation source code, supporting datasets, figures and reproducibility artefacts for evaluating an SDN-based cybersecurity framework for Industrial Control Systems (ICS).

The simulation models an ICS environment involving a Human-Machine Interface (HMI), engineering workstation and Programmable Logic Controller (PLC).

## 2. Software Requirements

- MATLAB R2024b (used for the reported results).
- MATLAB R2020a or later.
- Base MATLAB functions.
- No additional MATLAB toolboxes required.

## 3. Simulation Configuration

- Simulation duration: 120 seconds.
- Simulation time step: 0.01 seconds.
- Monte Carlo runs: 30.
- Base random seed: 2026.
- Network bottleneck capacity: 1,000 packets/second.
- Buffer capacity: 200 packets.

## 4. Attack Scenarios

1. TCP SYN port scanning.
2. Modbus/TCP flooding.
3. TCP SYN flooding (spoofed).
4. HTTP flooding.

## 5. Comparison Modes

- **Baseline:** Network operation without a security application.
- **Static ACL:** Static Access Control List protection.
- **SDN-Sec:** SDN-based detection and dynamic mitigation.

The three modes are evaluated using identical simulated traffic conditions.

## 6. Evaluation Metrics

- Attack detection latency.
- Time to mitigation.
- Detection performance and false-positive rate.
- Legitimate HMI packet delivery.
- HMI packet loss.
- HMI communication latency and deadline misses.
- Threshold sensitivity.
- Controller resource utilisation.

## 7. Repository Releases

Two simulation releases are maintained:

- **V1.0:** Original MATLAB simulation package.
- **V2.0:** Updated MATLAB simulation package with the revised three-mode comparison, supporting results and reproducibility script.

The latest release is:

`SDN_ICS_Cybersecurity_Simulation_V2.0.zip`

## 8. Running the Simulation

### Requirements

MATLAB R2020a or later, with Base MATLAB.

### Instructions

1. Download the V2.0 ZIP package.
2. Extract all files into one project directory.
3. Open MATLAB.
4. Set the extracted project directory as the MATLAB Current Folder.
5. Execute:

```matlab
sdn_Code_REPRODUCIBILITY
```

The reproducibility script executes the authoritative simulation file, `sdn_Code.m`.

The simulation generates the corresponding figures, tables and datasets.

## 9. Simulation Limitations

This study uses a MATLAB-based simulation model. It does not represent deployment on a physical industrial network or a live SDN controller.

SDN monitoring, detection and mitigation operations are represented through simulated network and controller behaviour.

Results should therefore be interpreted within the assumptions and limitations of the simulation environment.

## 10. Reproducibility and Citation

The simulation source code and supporting research artefacts are provided in the repository.

The archived research release and its permanent Zenodo DOI will be added following publication of the updated Zenodo version.

## 11. Authors

**Mupatiwa Zulu**  
School of Engineering  
University of Zambia

**Lukumba Phiri**  
School of Engineering  
University of Zambia
