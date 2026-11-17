# SDN-Based Cybersecurity Framework for Industrial Control Systems

## Project Description

This repository contains the MATLAB simulation source code and reproducibility artefacts for the research study titled **Development of a Software Defined Network Based Cybersecurity Framework for Industrial Control Systems**.

The study develops and evaluates an SDN-inspired cybersecurity framework for Industrial Control Systems (ICS) using a MATLAB-based simulation model.

## Software Environment

- MATLAB release used for the reported results: **MATLAB R2024b**
- Minimum stated source-code requirement: MATLAB R2020a or later
- MATLAB Base functions only
- No additional MATLAB toolboxes required

## Simulation Configuration

| Parameter | Value |
|---|---:|
| Simulation duration | 120 seconds |
| Simulation time step | 0.01 seconds |
| Monte Carlo runs | 30 |
| Base random seed | 2026 |
| Attack period | 45–90 seconds |
| Bottleneck capacity | 1,000 packets/second |
| Buffer capacity | 200 packets |

## Attack Scenarios

The simulation evaluates four attack scenarios:

1. TCP Port Scan
2. Modbus/TCP Flood
3. TCP SYN Flood (spoofed)
4. HTTP Flood

## Random-Seed Scheme

The Twister random-number generator is used. For Monte Carlo run \(r\) and attack scenario \(a\), the seed is calculated as:

`Seed = 2026 + 1000*r + a`

Runs are indexed from 1 to 30, and attack scenarios are indexed from 1 to 4.

## Repository Contents

The ZIP archive contains the following artefacts:

- MATLAB simulation source code
- Individual Monte Carlo run results
- Raw MATLAB simulation data
- Four exported Excel summary tables
- Nine generated PNG figures
- Reproducibility documentation

[Download the complete simulation package](SDN_ICS_Cybersecurity_Simulation_v1.0.zip)

## Running the Simulation

1. Download and extract the ZIP archive.
2. Open MATLAB.
3. Set the extracted `Appendix_B_Simulation_Artefacts` folder as the MATLAB Current Folder.
4. Run the following command:

`run(fullfile('01_Source_Code','sdn_Code_REPRODUCIBILITY.m'))`

The simulation generates the figures and summary tables in the current folder.

## Reproducibility Note

This work is based on a MATLAB simulation model. It does not represent a deployment involving a live SDN controller or a physical Industrial Control System testbed. The mitigation mechanism models SDN/OpenFlow-inspired behaviour.

The reported results correspond to the simulation configuration and random-seed scheme documented above.
